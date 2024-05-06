# Comparing `tmp/pynbody-2.0.0b8.tar.gz` & `tmp/pynbody-2.0.0b9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynbody-2.0.0b8.tar", last modified: Sat May  4 10:19:01 2024, max compression
+gzip compressed data, was "pynbody-2.0.0b9.tar", last modified: Sat May  4 19:39:20 2024, max compression
```

## Comparing `pynbody-2.0.0b8.tar` & `pynbody-2.0.0b9.tar`

### file list

```diff
@@ -1,218 +1,218 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 10:19:01.392221 pynbody-2.0.0b8/
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-04 10:18:55.000000 pynbody-2.0.0b8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3306 2024-05-04 10:19:01.392221 pynbody-2.0.0b8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2514 2024-05-04 10:18:55.000000 pynbody-2.0.0b8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 10:19:01.364221 pynbody-2.0.0b8/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     4597 2024-05-04 10:18:55.000000 pynbody-2.0.0b8/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 10:19:01.360221 pynbody-2.0.0b8/docs/_templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 10:19:01.364221 pynbody-2.0.0b8/docs/_templates/autosummary/
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-05-04 10:18:55.000000 pynbody-2.0.0b8/docs/_templates/autosummary/class.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-05-04 10:18:55.000000 pynbody-2.0.0b8/docs/_templates/autosummary/module.rst
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-05-04 10:18:55.000000 pynbody-2.0.0b8/docs/acknowledge.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-05-04 10:18:55.000000 pynbody-2.0.0b8/docs/bibliography.rst
--rw-r--r--   0 runner    (1001) docker     (127)     9768 2024-05-04 10:18:55.000000 pynbody-2.0.0b8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     3652 2024-05-04 10:18:55.000000 pynbody-2.0.0b8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7397 2024-05-04 10:18:55.000000 pynbody-2.0.0b8/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3475 2024-05-04 10:18:55.000000 pynbody-2.0.0b8/docs/loaders.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6911 2024-05-04 10:18:55.000000 pynbody-2.0.0b8/docs/pitfalls.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 10:19:01.364221 pynbody-2.0.0b8/docs/reference/
--rw-r--r--   0 runner    (1001) docker     (127)      948 2024-05-04 10:18:55.000000 pynbody-2.0.0b8/docs/reference/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 10:19:01.364221 pynbody-2.0.0b8/docs/tutorials/
--rw-r--r--   0 runner    (1001) docker     (127)    10514 2024-05-04 10:18:55.000000 pynbody-2.0.0b8/docs/tutorials/bridge.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1722 2024-05-04 10:18:55.000000 pynbody-2.0.0b8/docs/tutorials/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (127)    19402 2024-05-04 10:18:55.000000 pynbody-2.0.0b8/docs/tutorials/data_access.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5368 2024-05-04 10:18:55.000000 pynbody-2.0.0b8/docs/tutorials/derived.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 10:19:01.368221 pynbody-2.0.0b8/docs/tutorials/example_code/
--rw-r--r--   0 runner    (1001) docker     (127)      465 2024-05-04 10:18:55.000000 pynbody-2.0.0b8/docs/tutorials/example_code/density_integrated.py
--rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-05-04 10:18:55.000000 pynbody-2.0.0b8/docs/tutorials/example_code/density_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)      429 2024-05-04 10:18:55.000000 pynbody-2.0.0b8/docs/tutorials/example_code/density_slice.py
--rw-r--r--   0 runner    (1001) docker     (127)     2337 2024-05-04 10:18:55.000000 pynbody-2.0.0b8/docs/tutorials/example_code/do_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-05-04 10:18:55.000000 pynbody-2.0.0b8/docs/tutorials/example_code/do_images.py
--rw-r--r--   0 runner    (1001) docker     (127)     2055 2024-05-04 10:18:55.000000 pynbody-2.0.0b8/docs/tutorials/example_code/do_pictures.py
--rw-r--r--   0 runner    (1001) docker     (127)      958 2024-05-04 10:18:55.000000 pynbody-2.0.0b8/docs/tutorials/example_code/do_plots.py
--rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-05-04 10:18:55.000000 pynbody-2.0.0b8/docs/tutorials/example_code/do_preamble.py
--rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-05-04 10:18:55.000000 pynbody-2.0.0b8/docs/tutorials/example_code/rcs.py
--rw-r--r--   0 runner    (1001) docker     (127)      956 2024-05-04 10:18:55.000000 pynbody-2.0.0b8/docs/tutorials/example_code/rotcurve.py
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-05-04 10:18:55.000000 pynbody-2.0.0b8/docs/tutorials/example_code/star_render.py
--rw-r--r--   0 runner    (1001) docker     (127)      464 2024-05-04 10:18:55.000000 pynbody-2.0.0b8/docs/tutorials/example_code/temperature_slice.py
--rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-05-04 10:18:55.000000 pynbody-2.0.0b8/docs/tutorials/example_code/velocity_vectors.py
--rw-r--r--   0 runner    (1001) docker     (127)     6782 2024-05-04 10:18:55.000000 pynbody-2.0.0b8/docs/tutorials/filters.rst
--rw-r--r--   0 runner    (1001) docker     (127)    11931 2024-05-04 10:18:55.000000 pynbody-2.0.0b8/docs/tutorials/halos.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5431 2024-05-04 10:18:55.000000 pynbody-2.0.0b8/docs/tutorials/hmf.rst
--rw-r--r--   0 runner    (1001) docker     (127)     8744 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/docs/tutorials/performance.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3319 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/docs/tutorials/pictures.rst
--rw-r--r--   0 runner    (1001) docker     (127)    10348 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/docs/tutorials/profile.rst
--rw-r--r--   0 runner    (1001) docker     (127)    13890 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/docs/tutorials/quickstart.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5432 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/docs/tutorials/threads.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2570 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/docs/tutorials/tutorials.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 10:19:01.368221 pynbody-2.0.0b8/pynbody/
--rw-r--r--   0 runner    (1001) docker     (127)     1897 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/pynbody/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 10:19:01.376221 pynbody-2.0.0b8/pynbody/analysis/
--rw-r--r--   0 runner    (1001) docker     (127)    50000 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/pynbody/analysis/CAMB_Planck18
--rw-r--r--   0 runner    (1001) docker     (127)     4654 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/pynbody/analysis/CAMB_WMAP7
--rw-r--r--   0 runner    (1001) docker     (127)      806 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/pynbody/analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2510 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/pynbody/analysis/_com.pyx
--rw-r--r--   0 runner    (1001) docker     (127)     4177 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/pynbody/analysis/_interpolate3d.pyx
--rw-r--r--   0 runner    (1001) docker     (127)     9240 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/pynbody/analysis/angmom.py
--rw-r--r--   0 runner    (1001) docker     (127)     9838 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/pynbody/analysis/cambtemplate.ini
--rw-r--r--   0 runner    (1001) docker     (127)   103822 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/pynbody/analysis/cmdlum.npz
--rw-r--r--   0 runner    (1001) docker     (127)    12325 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/pynbody/analysis/cosmology.py
--rw-r--r--   0 runner    (1001) docker     (127)     7344 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/pynbody/analysis/decomp.py
--rw-r--r--   0 runner    (1001) docker     (127)     3264 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/pynbody/analysis/gravity.py
--rw-r--r--   0 runner    (1001) docker     (127)   872484 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/pynbody/analysis/h1.hdf5
--rw-r--r--   0 runner    (1001) docker     (127)    20567 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/pynbody/analysis/halo.py
--rw-r--r--   0 runner    (1001) docker     (127)     2851 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/pynbody/analysis/hifrac.py
--rw-r--r--   0 runner    (1001) docker     (127)    33570 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/pynbody/analysis/hmf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2170 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/pynbody/analysis/interpolate.py
--rw-r--r--   0 runner    (1001) docker     (127)     2014 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/pynbody/analysis/ionfrac.py
--rw-r--r--   0 runner    (1001) docker     (127)    96846 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/pynbody/analysis/ionfracs.npz
--rw-r--r--   0 runner    (1001) docker     (127)     6426 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/pynbody/analysis/luminosity.py
--rw-r--r--   0 runner    (1001) docker     (127)    11390 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/pynbody/analysis/pkdgrav_cosmo.py
--rw-r--r--   0 runner    (1001) docker     (127)    35128 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/pynbody/analysis/profile.py
--rw-r--r--   0 runner    (1001) docker     (127)    14279 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/pynbody/analysis/ramses_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     9404 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/pynbody/analysis/theoretical_profiles.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 10:19:01.376221 pynbody-2.0.0b8/pynbody/array/
--rw-r--r--   0 runner    (1001) docker     (127)    35806 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/pynbody/array/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8982 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/pynbody/array/shared.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 10:19:01.376221 pynbody-2.0.0b8/pynbody/bridge/
--rw-r--r--   0 runner    (1001) docker     (127)    20598 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/pynbody/bridge/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2038 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/pynbody/bridge/_bridge.pyx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 10:19:01.376221 pynbody-2.0.0b8/pynbody/chunk/
--rw-r--r--   0 runner    (1001) docker     (127)    14387 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/pynbody/chunk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/pynbody/chunk/scan.pyx
--rw-r--r--   0 runner    (1001) docker     (127)     4231 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/pynbody/configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)    12648 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/pynbody/default_config.ini
--rw-r--r--   0 runner    (1001) docker     (127)     3357 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/pynbody/dependencytracker.py
--rw-r--r--   0 runner    (1001) docker     (127)     8967 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/pynbody/derived.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 10:19:01.376221 pynbody-2.0.0b8/pynbody/extern/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/pynbody/extern/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12161 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/pynbody/extern/_cython_fortran_utils.pyx
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/pynbody/extern/cython_fortran_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4232 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/pynbody/family.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 10:19:01.376221 pynbody-2.0.0b8/pynbody/filt/
--rw-r--r--   0 runner    (1001) docker     (127)    20293 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/pynbody/filt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3776 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/pynbody/filt/geometry_selection.pyx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 10:19:01.376221 pynbody-2.0.0b8/pynbody/gravity/
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/pynbody/gravity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2186 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/pynbody/gravity/_gravity.pyx
--rw-r--r--   0 runner    (1001) docker     (127)     7245 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/pynbody/gravity/calc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 10:19:01.376221 pynbody-2.0.0b8/pynbody/halo/
--rw-r--r--   0 runner    (1001) docker     (127)    19880 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/pynbody/halo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17451 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/pynbody/halo/adaptahop.py
--rw-r--r--   0 runner    (1001) docker     (127)    19201 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/pynbody/halo/ahf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 10:19:01.380221 pynbody-2.0.0b8/pynbody/halo/details/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/pynbody/halo/details/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3443 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/pynbody/halo/details/iord_mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)     8344 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/pynbody/halo/details/number_mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)     2494 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/pynbody/halo/details/particle_indices.py
--rw-r--r--   0 runner    (1001) docker     (127)    11555 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/pynbody/halo/hbtplus.py
--rw-r--r--   0 runner    (1001) docker     (127)     3501 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/pynbody/halo/hop.py
--rw-r--r--   0 runner    (1001) docker     (127)     3625 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/pynbody/halo/number_array.py
--rw-r--r--   0 runner    (1001) docker     (127)    17216 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/pynbody/halo/rockstar.py
--rw-r--r--   0 runner    (1001) docker     (127)    17250 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/pynbody/halo/subfind.py
--rw-r--r--   0 runner    (1001) docker     (127)    25292 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/pynbody/halo/subfindhdf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1610 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/pynbody/halo/subhalo_catalogue.py
--rw-r--r--   0 runner    (1001) docker     (127)    10851 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/pynbody/halo/velociraptor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 10:19:01.380221 pynbody-2.0.0b8/pynbody/kdtree/
--rw-r--r--   0 runner    (1001) docker     (127)    19401 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/pynbody/kdtree/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7036 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/pynbody/kdtree/kd.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    10541 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/pynbody/kdtree/kd.h
--rw-r--r--   0 runner    (1001) docker     (127)    23690 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/pynbody/kdtree/kdmain.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     6076 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/pynbody/kdtree/pq.h
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/pynbody/kdtree/smooth.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    28997 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/pynbody/kdtree/smooth.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 10:19:01.380221 pynbody-2.0.0b8/pynbody/openmp/
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/pynbody/openmp/openmp_null.pyx
--rw-r--r--   0 runner    (1001) docker     (127)      549 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/pynbody/openmp/openmp_real.pyx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 10:19:01.380221 pynbody-2.0.0b8/pynbody/plot/
--rw-r--r--   0 runner    (1001) docker     (127)      530 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/pynbody/plot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3670 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/pynbody/plot/gas.py
--rw-r--r--   0 runner    (1001) docker     (127)    19212 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/pynbody/plot/generic.py
--rw-r--r--   0 runner    (1001) docker     (127)     1882 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/pynbody/plot/metals.py
--rw-r--r--   0 runner    (1001) docker     (127)     6769 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/pynbody/plot/profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     4702 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/pynbody/plot/quiverkey.py
--rw-r--r--   0 runner    (1001) docker     (127)    25811 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/pynbody/plot/sph.py
--rw-r--r--   0 runner    (1001) docker     (127)    44246 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/pynbody/plot/stars.py
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/pynbody/plot/tollerud2008mw
--rw-r--r--   0 runner    (1001) docker     (127)     6364 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/pynbody/plot/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     2417 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/pynbody/simdict.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 10:19:01.384221 pynbody-2.0.0b8/pynbody/snapshot/
--rw-r--r--   0 runner    (1001) docker     (127)     3157 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/pynbody/snapshot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3017 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/pynbody/snapshot/ascii.py
--rw-r--r--   0 runner    (1001) docker     (127)     2962 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/pynbody/snapshot/copy_on_access.py
--rw-r--r--   0 runner    (1001) docker     (127)    52755 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/pynbody/snapshot/gadget.py
--rw-r--r--   0 runner    (1001) docker     (127)    41232 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/pynbody/snapshot/gadgethdf.py
--rw-r--r--   0 runner    (1001) docker     (127)     9161 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/pynbody/snapshot/grafic.py
--rw-r--r--   0 runner    (1001) docker     (127)     2781 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/pynbody/snapshot/namemapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     7164 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/pynbody/snapshot/nchilada.py
--rw-r--r--   0 runner    (1001) docker     (127)    47425 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/pynbody/snapshot/ramses.py
--rw-r--r--   0 runner    (1001) docker     (127)    71116 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/pynbody/snapshot/simsnap.py
--rw-r--r--   0 runner    (1001) docker     (127)    15045 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/pynbody/snapshot/subsnap.py
--rw-r--r--   0 runner    (1001) docker     (127)    10866 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/pynbody/snapshot/swift.py
--rw-r--r--   0 runner    (1001) docker     (127)    63498 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/pynbody/snapshot/tipsy.py
--rw-r--r--   0 runner    (1001) docker     (127)     4972 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/pynbody/snapshot/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 10:19:01.384221 pynbody-2.0.0b8/pynbody/sph/
--rw-r--r--   0 runner    (1001) docker     (127)    31727 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/pynbody/sph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18653 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/pynbody/sph/_render.pyx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 10:19:01.384221 pynbody-2.0.0b8/pynbody/test_utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/pynbody/test_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9906 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/pynbody/test_utils/gadget4_subfind_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)    18964 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/pynbody/test_utils/pyread_gadget_hdf5.py
--rw-r--r--   0 runner    (1001) docker     (127)    16592 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/pynbody/transformation.py
--rw-r--r--   0 runner    (1001) docker     (127)    25347 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/pynbody/units.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 10:19:01.384221 pynbody-2.0.0b8/pynbody/util/
--rw-r--r--   0 runner    (1001) docker     (127)    19035 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/pynbody/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10035 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/pynbody/util/_util.pyx
--rw-r--r--   0 runner    (1001) docker     (127)     3296 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/pynbody/util/hdf_vds.py
--rw-r--r--   0 runner    (1001) docker     (127)     1830 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/pynbody/util/iter_subclasses.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 10:19:01.368221 pynbody-2.0.0b8/pynbody.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3306 2024-05-04 10:19:01.000000 pynbody-2.0.0b8/pynbody.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5173 2024-05-04 10:19:01.000000 pynbody-2.0.0b8/pynbody.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 10:19:01.000000 pynbody-2.0.0b8/pynbody.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-05-04 10:19:01.000000 pynbody-2.0.0b8/pynbody.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-05-04 10:19:01.000000 pynbody-2.0.0b8/pynbody.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-04 10:19:01.392221 pynbody-2.0.0b8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     8149 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 10:19:01.392221 pynbody-2.0.0b8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     8487 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/tests/adaptahop_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    12467 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/tests/ahf_halos_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     9374 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/tests/array_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     7408 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/tests/bridge_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4732 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/tests/copy_on_access_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/tests/cosmology_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     6358 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/tests/derived_arrays_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/tests/family_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     7081 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/tests/filter_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     7320 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/tests/gadget_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     5396 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/tests/gadgethdf_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1773 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/tests/grafic_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2919 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/tests/gravity_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    13591 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/tests/halos_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3471 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/tests/halotools_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    14383 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/tests/hbtplus_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2536 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/tests/hmf_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/tests/hop_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/tests/import_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    10743 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/tests/kdtree_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    11675 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/tests/nchilada_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/tests/partial_tipsy_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2350 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/tests/performance_kdtree.py
--rw-r--r--   0 runner    (1001) docker     (127)     7722 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/tests/ramses_new_ptcl_format_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    21598 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/tests/ramses_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3549 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/tests/rockstar_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/tests/simsnap_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     7072 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/tests/snapshot_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     5151 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/tests/sph_image_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/tests/subarray_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     6121 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/tests/subfind_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     5751 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/tests/subfindhdf_gadget4_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     9653 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/tests/subfindhdf_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     8681 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/tests/swift_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2773 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/tests/test_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     4717 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/tests/theoretical_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)    19416 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/tests/tipsy_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     5223 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/tests/transformation_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3872 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/tests/units_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     6558 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/tests/utils_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4536 2024-05-04 10:18:56.000000 pynbody-2.0.0b8/tests/velociraptor_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 19:39:20.312846 pynbody-2.0.0b9/
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-04 19:39:14.000000 pynbody-2.0.0b9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3306 2024-05-04 19:39:20.312846 pynbody-2.0.0b9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2514 2024-05-04 19:39:14.000000 pynbody-2.0.0b9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 19:39:20.284846 pynbody-2.0.0b9/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     4597 2024-05-04 19:39:14.000000 pynbody-2.0.0b9/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 19:39:20.280846 pynbody-2.0.0b9/docs/_templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 19:39:20.284846 pynbody-2.0.0b9/docs/_templates/autosummary/
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-05-04 19:39:14.000000 pynbody-2.0.0b9/docs/_templates/autosummary/class.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-05-04 19:39:14.000000 pynbody-2.0.0b9/docs/_templates/autosummary/module.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-05-04 19:39:14.000000 pynbody-2.0.0b9/docs/acknowledge.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-05-04 19:39:14.000000 pynbody-2.0.0b9/docs/bibliography.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     9768 2024-05-04 19:39:14.000000 pynbody-2.0.0b9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3652 2024-05-04 19:39:14.000000 pynbody-2.0.0b9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7397 2024-05-04 19:39:14.000000 pynbody-2.0.0b9/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3475 2024-05-04 19:39:14.000000 pynbody-2.0.0b9/docs/loaders.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6911 2024-05-04 19:39:14.000000 pynbody-2.0.0b9/docs/pitfalls.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 19:39:20.284846 pynbody-2.0.0b9/docs/reference/
+-rw-r--r--   0 runner    (1001) docker     (127)      948 2024-05-04 19:39:14.000000 pynbody-2.0.0b9/docs/reference/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 19:39:20.284846 pynbody-2.0.0b9/docs/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (127)    10514 2024-05-04 19:39:14.000000 pynbody-2.0.0b9/docs/tutorials/bridge.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1722 2024-05-04 19:39:14.000000 pynbody-2.0.0b9/docs/tutorials/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    19402 2024-05-04 19:39:14.000000 pynbody-2.0.0b9/docs/tutorials/data_access.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5368 2024-05-04 19:39:14.000000 pynbody-2.0.0b9/docs/tutorials/derived.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 19:39:20.288846 pynbody-2.0.0b9/docs/tutorials/example_code/
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-05-04 19:39:14.000000 pynbody-2.0.0b9/docs/tutorials/example_code/density_integrated.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-05-04 19:39:14.000000 pynbody-2.0.0b9/docs/tutorials/example_code/density_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)      429 2024-05-04 19:39:14.000000 pynbody-2.0.0b9/docs/tutorials/example_code/density_slice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2337 2024-05-04 19:39:14.000000 pynbody-2.0.0b9/docs/tutorials/example_code/do_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-05-04 19:39:14.000000 pynbody-2.0.0b9/docs/tutorials/example_code/do_images.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2055 2024-05-04 19:39:14.000000 pynbody-2.0.0b9/docs/tutorials/example_code/do_pictures.py
+-rw-r--r--   0 runner    (1001) docker     (127)      958 2024-05-04 19:39:14.000000 pynbody-2.0.0b9/docs/tutorials/example_code/do_plots.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-05-04 19:39:14.000000 pynbody-2.0.0b9/docs/tutorials/example_code/do_preamble.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-05-04 19:39:14.000000 pynbody-2.0.0b9/docs/tutorials/example_code/rcs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      956 2024-05-04 19:39:14.000000 pynbody-2.0.0b9/docs/tutorials/example_code/rotcurve.py
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-05-04 19:39:14.000000 pynbody-2.0.0b9/docs/tutorials/example_code/star_render.py
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-05-04 19:39:14.000000 pynbody-2.0.0b9/docs/tutorials/example_code/temperature_slice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-05-04 19:39:14.000000 pynbody-2.0.0b9/docs/tutorials/example_code/velocity_vectors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6782 2024-05-04 19:39:14.000000 pynbody-2.0.0b9/docs/tutorials/filters.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    11931 2024-05-04 19:39:14.000000 pynbody-2.0.0b9/docs/tutorials/halos.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5431 2024-05-04 19:39:14.000000 pynbody-2.0.0b9/docs/tutorials/hmf.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     8744 2024-05-04 19:39:14.000000 pynbody-2.0.0b9/docs/tutorials/performance.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3319 2024-05-04 19:39:14.000000 pynbody-2.0.0b9/docs/tutorials/pictures.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    10348 2024-05-04 19:39:14.000000 pynbody-2.0.0b9/docs/tutorials/profile.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    13890 2024-05-04 19:39:14.000000 pynbody-2.0.0b9/docs/tutorials/quickstart.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5432 2024-05-04 19:39:14.000000 pynbody-2.0.0b9/docs/tutorials/threads.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2570 2024-05-04 19:39:14.000000 pynbody-2.0.0b9/docs/tutorials/tutorials.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 19:39:20.288846 pynbody-2.0.0b9/pynbody/
+-rw-r--r--   0 runner    (1001) docker     (127)     1897 2024-05-04 19:39:14.000000 pynbody-2.0.0b9/pynbody/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 19:39:20.296846 pynbody-2.0.0b9/pynbody/analysis/
+-rw-r--r--   0 runner    (1001) docker     (127)    50000 2024-05-04 19:39:14.000000 pynbody-2.0.0b9/pynbody/analysis/CAMB_Planck18
+-rw-r--r--   0 runner    (1001) docker     (127)     4654 2024-05-04 19:39:14.000000 pynbody-2.0.0b9/pynbody/analysis/CAMB_WMAP7
+-rw-r--r--   0 runner    (1001) docker     (127)      806 2024-05-04 19:39:14.000000 pynbody-2.0.0b9/pynbody/analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2510 2024-05-04 19:39:14.000000 pynbody-2.0.0b9/pynbody/analysis/_com.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)     4177 2024-05-04 19:39:14.000000 pynbody-2.0.0b9/pynbody/analysis/_interpolate3d.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)     9240 2024-05-04 19:39:14.000000 pynbody-2.0.0b9/pynbody/analysis/angmom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9838 2024-05-04 19:39:14.000000 pynbody-2.0.0b9/pynbody/analysis/cambtemplate.ini
+-rw-r--r--   0 runner    (1001) docker     (127)   103822 2024-05-04 19:39:14.000000 pynbody-2.0.0b9/pynbody/analysis/cmdlum.npz
+-rw-r--r--   0 runner    (1001) docker     (127)    12325 2024-05-04 19:39:14.000000 pynbody-2.0.0b9/pynbody/analysis/cosmology.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7344 2024-05-04 19:39:14.000000 pynbody-2.0.0b9/pynbody/analysis/decomp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3264 2024-05-04 19:39:14.000000 pynbody-2.0.0b9/pynbody/analysis/gravity.py
+-rw-r--r--   0 runner    (1001) docker     (127)   872484 2024-05-04 19:39:14.000000 pynbody-2.0.0b9/pynbody/analysis/h1.hdf5
+-rw-r--r--   0 runner    (1001) docker     (127)    20567 2024-05-04 19:39:14.000000 pynbody-2.0.0b9/pynbody/analysis/halo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2851 2024-05-04 19:39:14.000000 pynbody-2.0.0b9/pynbody/analysis/hifrac.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33570 2024-05-04 19:39:14.000000 pynbody-2.0.0b9/pynbody/analysis/hmf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2170 2024-05-04 19:39:14.000000 pynbody-2.0.0b9/pynbody/analysis/interpolate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2014 2024-05-04 19:39:14.000000 pynbody-2.0.0b9/pynbody/analysis/ionfrac.py
+-rw-r--r--   0 runner    (1001) docker     (127)    96846 2024-05-04 19:39:14.000000 pynbody-2.0.0b9/pynbody/analysis/ionfracs.npz
+-rw-r--r--   0 runner    (1001) docker     (127)     6426 2024-05-04 19:39:14.000000 pynbody-2.0.0b9/pynbody/analysis/luminosity.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11390 2024-05-04 19:39:14.000000 pynbody-2.0.0b9/pynbody/analysis/pkdgrav_cosmo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35128 2024-05-04 19:39:14.000000 pynbody-2.0.0b9/pynbody/analysis/profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14279 2024-05-04 19:39:14.000000 pynbody-2.0.0b9/pynbody/analysis/ramses_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9404 2024-05-04 19:39:14.000000 pynbody-2.0.0b9/pynbody/analysis/theoretical_profiles.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 19:39:20.296846 pynbody-2.0.0b9/pynbody/array/
+-rw-r--r--   0 runner    (1001) docker     (127)    35806 2024-05-04 19:39:14.000000 pynbody-2.0.0b9/pynbody/array/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8982 2024-05-04 19:39:14.000000 pynbody-2.0.0b9/pynbody/array/shared.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 19:39:20.296846 pynbody-2.0.0b9/pynbody/bridge/
+-rw-r--r--   0 runner    (1001) docker     (127)    20598 2024-05-04 19:39:14.000000 pynbody-2.0.0b9/pynbody/bridge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2038 2024-05-04 19:39:14.000000 pynbody-2.0.0b9/pynbody/bridge/_bridge.pyx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 19:39:20.296846 pynbody-2.0.0b9/pynbody/chunk/
+-rw-r--r--   0 runner    (1001) docker     (127)    14387 2024-05-04 19:39:14.000000 pynbody-2.0.0b9/pynbody/chunk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-05-04 19:39:14.000000 pynbody-2.0.0b9/pynbody/chunk/scan.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)     4231 2024-05-04 19:39:14.000000 pynbody-2.0.0b9/pynbody/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12648 2024-05-04 19:39:14.000000 pynbody-2.0.0b9/pynbody/default_config.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     3357 2024-05-04 19:39:14.000000 pynbody-2.0.0b9/pynbody/dependencytracker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8967 2024-05-04 19:39:14.000000 pynbody-2.0.0b9/pynbody/derived.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 19:39:20.296846 pynbody-2.0.0b9/pynbody/extern/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 19:39:14.000000 pynbody-2.0.0b9/pynbody/extern/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12161 2024-05-04 19:39:14.000000 pynbody-2.0.0b9/pynbody/extern/_cython_fortran_utils.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-04 19:39:14.000000 pynbody-2.0.0b9/pynbody/extern/cython_fortran_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4232 2024-05-04 19:39:14.000000 pynbody-2.0.0b9/pynbody/family.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 19:39:20.296846 pynbody-2.0.0b9/pynbody/filt/
+-rw-r--r--   0 runner    (1001) docker     (127)    20293 2024-05-04 19:39:14.000000 pynbody-2.0.0b9/pynbody/filt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3776 2024-05-04 19:39:14.000000 pynbody-2.0.0b9/pynbody/filt/geometry_selection.pyx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 19:39:20.296846 pynbody-2.0.0b9/pynbody/gravity/
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-04 19:39:14.000000 pynbody-2.0.0b9/pynbody/gravity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2186 2024-05-04 19:39:14.000000 pynbody-2.0.0b9/pynbody/gravity/_gravity.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)     7245 2024-05-04 19:39:14.000000 pynbody-2.0.0b9/pynbody/gravity/calc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 19:39:20.300846 pynbody-2.0.0b9/pynbody/halo/
+-rw-r--r--   0 runner    (1001) docker     (127)    19880 2024-05-04 19:39:14.000000 pynbody-2.0.0b9/pynbody/halo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17451 2024-05-04 19:39:14.000000 pynbody-2.0.0b9/pynbody/halo/adaptahop.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19201 2024-05-04 19:39:14.000000 pynbody-2.0.0b9/pynbody/halo/ahf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 19:39:20.300846 pynbody-2.0.0b9/pynbody/halo/details/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 19:39:14.000000 pynbody-2.0.0b9/pynbody/halo/details/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3443 2024-05-04 19:39:14.000000 pynbody-2.0.0b9/pynbody/halo/details/iord_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8344 2024-05-04 19:39:14.000000 pynbody-2.0.0b9/pynbody/halo/details/number_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2494 2024-05-04 19:39:14.000000 pynbody-2.0.0b9/pynbody/halo/details/particle_indices.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11555 2024-05-04 19:39:14.000000 pynbody-2.0.0b9/pynbody/halo/hbtplus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3501 2024-05-04 19:39:14.000000 pynbody-2.0.0b9/pynbody/halo/hop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3625 2024-05-04 19:39:14.000000 pynbody-2.0.0b9/pynbody/halo/number_array.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17216 2024-05-04 19:39:14.000000 pynbody-2.0.0b9/pynbody/halo/rockstar.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17250 2024-05-04 19:39:14.000000 pynbody-2.0.0b9/pynbody/halo/subfind.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25292 2024-05-04 19:39:14.000000 pynbody-2.0.0b9/pynbody/halo/subfindhdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1610 2024-05-04 19:39:14.000000 pynbody-2.0.0b9/pynbody/halo/subhalo_catalogue.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10851 2024-05-04 19:39:14.000000 pynbody-2.0.0b9/pynbody/halo/velociraptor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 19:39:20.300846 pynbody-2.0.0b9/pynbody/kdtree/
+-rw-r--r--   0 runner    (1001) docker     (127)    19401 2024-05-04 19:39:14.000000 pynbody-2.0.0b9/pynbody/kdtree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7036 2024-05-04 19:39:14.000000 pynbody-2.0.0b9/pynbody/kdtree/kd.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    10541 2024-05-04 19:39:14.000000 pynbody-2.0.0b9/pynbody/kdtree/kd.h
+-rw-r--r--   0 runner    (1001) docker     (127)    23690 2024-05-04 19:39:14.000000 pynbody-2.0.0b9/pynbody/kdtree/kdmain.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     6076 2024-05-04 19:39:14.000000 pynbody-2.0.0b9/pynbody/kdtree/pq.h
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-04 19:39:14.000000 pynbody-2.0.0b9/pynbody/kdtree/smooth.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    28997 2024-05-04 19:39:14.000000 pynbody-2.0.0b9/pynbody/kdtree/smooth.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 19:39:20.300846 pynbody-2.0.0b9/pynbody/openmp/
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-05-04 19:39:14.000000 pynbody-2.0.0b9/pynbody/openmp/openmp_null.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)      549 2024-05-04 19:39:14.000000 pynbody-2.0.0b9/pynbody/openmp/openmp_real.pyx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 19:39:20.304846 pynbody-2.0.0b9/pynbody/plot/
+-rw-r--r--   0 runner    (1001) docker     (127)      530 2024-05-04 19:39:14.000000 pynbody-2.0.0b9/pynbody/plot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3670 2024-05-04 19:39:14.000000 pynbody-2.0.0b9/pynbody/plot/gas.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19212 2024-05-04 19:39:14.000000 pynbody-2.0.0b9/pynbody/plot/generic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1882 2024-05-04 19:39:14.000000 pynbody-2.0.0b9/pynbody/plot/metals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6769 2024-05-04 19:39:14.000000 pynbody-2.0.0b9/pynbody/plot/profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4702 2024-05-04 19:39:14.000000 pynbody-2.0.0b9/pynbody/plot/quiverkey.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25811 2024-05-04 19:39:14.000000 pynbody-2.0.0b9/pynbody/plot/sph.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44246 2024-05-04 19:39:14.000000 pynbody-2.0.0b9/pynbody/plot/stars.py
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-04 19:39:14.000000 pynbody-2.0.0b9/pynbody/plot/tollerud2008mw
+-rw-r--r--   0 runner    (1001) docker     (127)     6364 2024-05-04 19:39:14.000000 pynbody-2.0.0b9/pynbody/plot/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2417 2024-05-04 19:39:14.000000 pynbody-2.0.0b9/pynbody/simdict.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 19:39:20.304846 pynbody-2.0.0b9/pynbody/snapshot/
+-rw-r--r--   0 runner    (1001) docker     (127)     3157 2024-05-04 19:39:14.000000 pynbody-2.0.0b9/pynbody/snapshot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3017 2024-05-04 19:39:14.000000 pynbody-2.0.0b9/pynbody/snapshot/ascii.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2962 2024-05-04 19:39:14.000000 pynbody-2.0.0b9/pynbody/snapshot/copy_on_access.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52755 2024-05-04 19:39:14.000000 pynbody-2.0.0b9/pynbody/snapshot/gadget.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41232 2024-05-04 19:39:14.000000 pynbody-2.0.0b9/pynbody/snapshot/gadgethdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9161 2024-05-04 19:39:14.000000 pynbody-2.0.0b9/pynbody/snapshot/grafic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2781 2024-05-04 19:39:14.000000 pynbody-2.0.0b9/pynbody/snapshot/namemapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7164 2024-05-04 19:39:14.000000 pynbody-2.0.0b9/pynbody/snapshot/nchilada.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47425 2024-05-04 19:39:14.000000 pynbody-2.0.0b9/pynbody/snapshot/ramses.py
+-rw-r--r--   0 runner    (1001) docker     (127)    71327 2024-05-04 19:39:14.000000 pynbody-2.0.0b9/pynbody/snapshot/simsnap.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15111 2024-05-04 19:39:14.000000 pynbody-2.0.0b9/pynbody/snapshot/subsnap.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10866 2024-05-04 19:39:14.000000 pynbody-2.0.0b9/pynbody/snapshot/swift.py
+-rw-r--r--   0 runner    (1001) docker     (127)    63498 2024-05-04 19:39:14.000000 pynbody-2.0.0b9/pynbody/snapshot/tipsy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4972 2024-05-04 19:39:14.000000 pynbody-2.0.0b9/pynbody/snapshot/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 19:39:20.304846 pynbody-2.0.0b9/pynbody/sph/
+-rw-r--r--   0 runner    (1001) docker     (127)    31727 2024-05-04 19:39:14.000000 pynbody-2.0.0b9/pynbody/sph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18653 2024-05-04 19:39:14.000000 pynbody-2.0.0b9/pynbody/sph/_render.pyx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 19:39:20.304846 pynbody-2.0.0b9/pynbody/test_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 19:39:14.000000 pynbody-2.0.0b9/pynbody/test_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9906 2024-05-04 19:39:14.000000 pynbody-2.0.0b9/pynbody/test_utils/gadget4_subfind_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18964 2024-05-04 19:39:14.000000 pynbody-2.0.0b9/pynbody/test_utils/pyread_gadget_hdf5.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16592 2024-05-04 19:39:14.000000 pynbody-2.0.0b9/pynbody/transformation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25347 2024-05-04 19:39:14.000000 pynbody-2.0.0b9/pynbody/units.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 19:39:20.308846 pynbody-2.0.0b9/pynbody/util/
+-rw-r--r--   0 runner    (1001) docker     (127)    19035 2024-05-04 19:39:14.000000 pynbody-2.0.0b9/pynbody/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10035 2024-05-04 19:39:14.000000 pynbody-2.0.0b9/pynbody/util/_util.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)     3296 2024-05-04 19:39:14.000000 pynbody-2.0.0b9/pynbody/util/hdf_vds.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1830 2024-05-04 19:39:14.000000 pynbody-2.0.0b9/pynbody/util/iter_subclasses.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 19:39:20.292846 pynbody-2.0.0b9/pynbody.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3306 2024-05-04 19:39:20.000000 pynbody-2.0.0b9/pynbody.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5173 2024-05-04 19:39:20.000000 pynbody-2.0.0b9/pynbody.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 19:39:20.000000 pynbody-2.0.0b9/pynbody.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-05-04 19:39:20.000000 pynbody-2.0.0b9/pynbody.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-05-04 19:39:20.000000 pynbody-2.0.0b9/pynbody.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-05-04 19:39:14.000000 pynbody-2.0.0b9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-04 19:39:20.312846 pynbody-2.0.0b9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     8149 2024-05-04 19:39:14.000000 pynbody-2.0.0b9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 19:39:20.312846 pynbody-2.0.0b9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     8487 2024-05-04 19:39:14.000000 pynbody-2.0.0b9/tests/adaptahop_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12467 2024-05-04 19:39:14.000000 pynbody-2.0.0b9/tests/ahf_halos_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9374 2024-05-04 19:39:14.000000 pynbody-2.0.0b9/tests/array_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7408 2024-05-04 19:39:14.000000 pynbody-2.0.0b9/tests/bridge_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4732 2024-05-04 19:39:14.000000 pynbody-2.0.0b9/tests/copy_on_access_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-05-04 19:39:14.000000 pynbody-2.0.0b9/tests/cosmology_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6358 2024-05-04 19:39:14.000000 pynbody-2.0.0b9/tests/derived_arrays_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-05-04 19:39:14.000000 pynbody-2.0.0b9/tests/family_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7081 2024-05-04 19:39:14.000000 pynbody-2.0.0b9/tests/filter_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7320 2024-05-04 19:39:14.000000 pynbody-2.0.0b9/tests/gadget_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5396 2024-05-04 19:39:14.000000 pynbody-2.0.0b9/tests/gadgethdf_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1773 2024-05-04 19:39:14.000000 pynbody-2.0.0b9/tests/grafic_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2919 2024-05-04 19:39:14.000000 pynbody-2.0.0b9/tests/gravity_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13591 2024-05-04 19:39:14.000000 pynbody-2.0.0b9/tests/halos_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3471 2024-05-04 19:39:14.000000 pynbody-2.0.0b9/tests/halotools_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14383 2024-05-04 19:39:14.000000 pynbody-2.0.0b9/tests/hbtplus_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2536 2024-05-04 19:39:14.000000 pynbody-2.0.0b9/tests/hmf_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-05-04 19:39:14.000000 pynbody-2.0.0b9/tests/hop_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-04 19:39:14.000000 pynbody-2.0.0b9/tests/import_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10743 2024-05-04 19:39:14.000000 pynbody-2.0.0b9/tests/kdtree_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11675 2024-05-04 19:39:14.000000 pynbody-2.0.0b9/tests/nchilada_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-05-04 19:39:14.000000 pynbody-2.0.0b9/tests/partial_tipsy_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2350 2024-05-04 19:39:14.000000 pynbody-2.0.0b9/tests/performance_kdtree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7722 2024-05-04 19:39:14.000000 pynbody-2.0.0b9/tests/ramses_new_ptcl_format_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21598 2024-05-04 19:39:14.000000 pynbody-2.0.0b9/tests/ramses_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3549 2024-05-04 19:39:14.000000 pynbody-2.0.0b9/tests/rockstar_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-05-04 19:39:14.000000 pynbody-2.0.0b9/tests/simsnap_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8174 2024-05-04 19:39:14.000000 pynbody-2.0.0b9/tests/snapshot_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5151 2024-05-04 19:39:14.000000 pynbody-2.0.0b9/tests/sph_image_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-05-04 19:39:14.000000 pynbody-2.0.0b9/tests/subarray_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6121 2024-05-04 19:39:14.000000 pynbody-2.0.0b9/tests/subfind_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5751 2024-05-04 19:39:14.000000 pynbody-2.0.0b9/tests/subfindhdf_gadget4_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9653 2024-05-04 19:39:14.000000 pynbody-2.0.0b9/tests/subfindhdf_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8681 2024-05-04 19:39:14.000000 pynbody-2.0.0b9/tests/swift_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2773 2024-05-04 19:39:14.000000 pynbody-2.0.0b9/tests/test_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4717 2024-05-04 19:39:14.000000 pynbody-2.0.0b9/tests/theoretical_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19416 2024-05-04 19:39:14.000000 pynbody-2.0.0b9/tests/tipsy_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5223 2024-05-04 19:39:14.000000 pynbody-2.0.0b9/tests/transformation_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3872 2024-05-04 19:39:14.000000 pynbody-2.0.0b9/tests/units_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6558 2024-05-04 19:39:14.000000 pynbody-2.0.0b9/tests/utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4536 2024-05-04 19:39:14.000000 pynbody-2.0.0b9/tests/velociraptor_test.py
```

### Comparing `pynbody-2.0.0b8/PKG-INFO` & `pynbody-2.0.0b9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynbody
-Version: 2.0.0b8
+Version: 2.0.0b9
 Summary: Light-weight astronomical N-body/SPH analysis for python
 Home-page: https://github.com/pynbody/pynbody/releases
 Author: The pynbody team
 Author-email: pynbody@googlegroups.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pynbody-2.0.0b8/README.md` & `pynbody-2.0.0b9/README.md`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b8/docs/Makefile` & `pynbody-2.0.0b9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b8/docs/_templates/autosummary/module.rst` & `pynbody-2.0.0b9/docs/_templates/autosummary/module.rst`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b8/docs/bibliography.rst` & `pynbody-2.0.0b9/docs/bibliography.rst`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b8/docs/conf.py` & `pynbody-2.0.0b9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b8/docs/index.rst` & `pynbody-2.0.0b9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b8/docs/installation.rst` & `pynbody-2.0.0b9/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b8/docs/loaders.rst` & `pynbody-2.0.0b9/docs/loaders.rst`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b8/docs/pitfalls.rst` & `pynbody-2.0.0b9/docs/pitfalls.rst`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b8/docs/reference/index.rst` & `pynbody-2.0.0b9/docs/reference/index.rst`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b8/docs/tutorials/bridge.rst` & `pynbody-2.0.0b9/docs/tutorials/bridge.rst`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b8/docs/tutorials/configuration.rst` & `pynbody-2.0.0b9/docs/tutorials/configuration.rst`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b8/docs/tutorials/data_access.rst` & `pynbody-2.0.0b9/docs/tutorials/data_access.rst`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b8/docs/tutorials/derived.rst` & `pynbody-2.0.0b9/docs/tutorials/derived.rst`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b8/docs/tutorials/example_code/density_profile.py` & `pynbody-2.0.0b9/docs/tutorials/example_code/density_profile.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b8/docs/tutorials/example_code/do_data.py` & `pynbody-2.0.0b9/docs/tutorials/example_code/do_data.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b8/docs/tutorials/example_code/do_images.py` & `pynbody-2.0.0b9/docs/tutorials/example_code/do_images.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b8/docs/tutorials/example_code/do_pictures.py` & `pynbody-2.0.0b9/docs/tutorials/example_code/do_pictures.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b8/docs/tutorials/example_code/do_plots.py` & `pynbody-2.0.0b9/docs/tutorials/example_code/do_plots.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b8/docs/tutorials/example_code/do_preamble.py` & `pynbody-2.0.0b9/docs/tutorials/example_code/do_preamble.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b8/docs/tutorials/example_code/rcs.py` & `pynbody-2.0.0b9/docs/tutorials/example_code/rcs.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b8/docs/tutorials/example_code/rotcurve.py` & `pynbody-2.0.0b9/docs/tutorials/example_code/rotcurve.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b8/docs/tutorials/example_code/velocity_vectors.py` & `pynbody-2.0.0b9/docs/tutorials/example_code/velocity_vectors.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b8/docs/tutorials/filters.rst` & `pynbody-2.0.0b9/docs/tutorials/filters.rst`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b8/docs/tutorials/halos.rst` & `pynbody-2.0.0b9/docs/tutorials/halos.rst`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b8/docs/tutorials/hmf.rst` & `pynbody-2.0.0b9/docs/tutorials/hmf.rst`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b8/docs/tutorials/performance.rst` & `pynbody-2.0.0b9/docs/tutorials/performance.rst`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b8/docs/tutorials/pictures.rst` & `pynbody-2.0.0b9/docs/tutorials/pictures.rst`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b8/docs/tutorials/profile.rst` & `pynbody-2.0.0b9/docs/tutorials/profile.rst`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b8/docs/tutorials/quickstart.rst` & `pynbody-2.0.0b9/docs/tutorials/quickstart.rst`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b8/docs/tutorials/threads.rst` & `pynbody-2.0.0b9/docs/tutorials/threads.rst`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b8/docs/tutorials/tutorials.rst` & `pynbody-2.0.0b9/docs/tutorials/tutorials.rst`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b8/pynbody/__init__.py` & `pynbody-2.0.0b9/pynbody/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -71,10 +71,10 @@
 
 plot = PlotModuleProxy()
 
 from .snapshot import load, new
 
 derived_array = snapshot.simsnap.SimSnap.derived_array
 
-__version__ = '2.0.0-beta.8'
+__version__ = '2.0.0-beta.9'
 
 __all__ = ['load', 'new', 'derived_array']
```

### Comparing `pynbody-2.0.0b8/pynbody/analysis/CAMB_Planck18` & `pynbody-2.0.0b9/pynbody/analysis/CAMB_Planck18`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b8/pynbody/analysis/CAMB_WMAP7` & `pynbody-2.0.0b9/pynbody/analysis/CAMB_WMAP7`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b8/pynbody/analysis/__init__.py` & `pynbody-2.0.0b9/pynbody/analysis/__init__.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b8/pynbody/analysis/_com.pyx` & `pynbody-2.0.0b9/pynbody/analysis/_com.pyx`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b8/pynbody/analysis/_interpolate3d.pyx` & `pynbody-2.0.0b9/pynbody/analysis/_interpolate3d.pyx`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b8/pynbody/analysis/angmom.py` & `pynbody-2.0.0b9/pynbody/analysis/angmom.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b8/pynbody/analysis/cambtemplate.ini` & `pynbody-2.0.0b9/pynbody/analysis/cambtemplate.ini`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b8/pynbody/analysis/cmdlum.npz` & `pynbody-2.0.0b9/pynbody/analysis/cmdlum.npz`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b8/pynbody/analysis/cosmology.py` & `pynbody-2.0.0b9/pynbody/analysis/cosmology.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b8/pynbody/analysis/decomp.py` & `pynbody-2.0.0b9/pynbody/analysis/decomp.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b8/pynbody/analysis/gravity.py` & `pynbody-2.0.0b9/pynbody/analysis/gravity.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b8/pynbody/analysis/h1.hdf5` & `pynbody-2.0.0b9/pynbody/analysis/h1.hdf5`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b8/pynbody/analysis/halo.py` & `pynbody-2.0.0b9/pynbody/analysis/halo.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b8/pynbody/analysis/hifrac.py` & `pynbody-2.0.0b9/pynbody/analysis/hifrac.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b8/pynbody/analysis/hmf.py` & `pynbody-2.0.0b9/pynbody/analysis/hmf.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b8/pynbody/analysis/interpolate.py` & `pynbody-2.0.0b9/pynbody/analysis/interpolate.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b8/pynbody/analysis/ionfrac.py` & `pynbody-2.0.0b9/pynbody/analysis/ionfrac.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b8/pynbody/analysis/ionfracs.npz` & `pynbody-2.0.0b9/pynbody/analysis/ionfracs.npz`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b8/pynbody/analysis/luminosity.py` & `pynbody-2.0.0b9/pynbody/analysis/luminosity.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b8/pynbody/analysis/pkdgrav_cosmo.py` & `pynbody-2.0.0b9/pynbody/analysis/pkdgrav_cosmo.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b8/pynbody/analysis/profile.py` & `pynbody-2.0.0b9/pynbody/analysis/profile.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b8/pynbody/analysis/ramses_util.py` & `pynbody-2.0.0b9/pynbody/analysis/ramses_util.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b8/pynbody/analysis/theoretical_profiles.py` & `pynbody-2.0.0b9/pynbody/analysis/theoretical_profiles.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b8/pynbody/array/__init__.py` & `pynbody-2.0.0b9/pynbody/array/__init__.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b8/pynbody/array/shared.py` & `pynbody-2.0.0b9/pynbody/array/shared.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b8/pynbody/bridge/__init__.py` & `pynbody-2.0.0b9/pynbody/bridge/__init__.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b8/pynbody/bridge/_bridge.pyx` & `pynbody-2.0.0b9/pynbody/bridge/_bridge.pyx`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b8/pynbody/chunk/__init__.py` & `pynbody-2.0.0b9/pynbody/chunk/__init__.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b8/pynbody/chunk/scan.pyx` & `pynbody-2.0.0b9/pynbody/chunk/scan.pyx`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b8/pynbody/configuration.py` & `pynbody-2.0.0b9/pynbody/configuration.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b8/pynbody/default_config.ini` & `pynbody-2.0.0b9/pynbody/default_config.ini`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b8/pynbody/dependencytracker.py` & `pynbody-2.0.0b9/pynbody/dependencytracker.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b8/pynbody/derived.py` & `pynbody-2.0.0b9/pynbody/derived.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b8/pynbody/extern/_cython_fortran_utils.pyx` & `pynbody-2.0.0b9/pynbody/extern/_cython_fortran_utils.pyx`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b8/pynbody/family.py` & `pynbody-2.0.0b9/pynbody/family.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b8/pynbody/filt/__init__.py` & `pynbody-2.0.0b9/pynbody/filt/__init__.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b8/pynbody/filt/geometry_selection.pyx` & `pynbody-2.0.0b9/pynbody/filt/geometry_selection.pyx`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b8/pynbody/gravity/_gravity.pyx` & `pynbody-2.0.0b9/pynbody/gravity/_gravity.pyx`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b8/pynbody/gravity/calc.py` & `pynbody-2.0.0b9/pynbody/gravity/calc.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b8/pynbody/halo/__init__.py` & `pynbody-2.0.0b9/pynbody/halo/__init__.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b8/pynbody/halo/adaptahop.py` & `pynbody-2.0.0b9/pynbody/halo/adaptahop.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b8/pynbody/halo/ahf.py` & `pynbody-2.0.0b9/pynbody/halo/ahf.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b8/pynbody/halo/details/iord_mapping.py` & `pynbody-2.0.0b9/pynbody/halo/details/iord_mapping.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b8/pynbody/halo/details/number_mapping.py` & `pynbody-2.0.0b9/pynbody/halo/details/number_mapping.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b8/pynbody/halo/details/particle_indices.py` & `pynbody-2.0.0b9/pynbody/halo/details/particle_indices.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b8/pynbody/halo/hbtplus.py` & `pynbody-2.0.0b9/pynbody/halo/hbtplus.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b8/pynbody/halo/hop.py` & `pynbody-2.0.0b9/pynbody/halo/hop.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b8/pynbody/halo/number_array.py` & `pynbody-2.0.0b9/pynbody/halo/number_array.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b8/pynbody/halo/rockstar.py` & `pynbody-2.0.0b9/pynbody/halo/rockstar.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b8/pynbody/halo/subfind.py` & `pynbody-2.0.0b9/pynbody/halo/subfind.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b8/pynbody/halo/subfindhdf.py` & `pynbody-2.0.0b9/pynbody/halo/subfindhdf.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b8/pynbody/halo/subhalo_catalogue.py` & `pynbody-2.0.0b9/pynbody/halo/subhalo_catalogue.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b8/pynbody/halo/velociraptor.py` & `pynbody-2.0.0b9/pynbody/halo/velociraptor.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b8/pynbody/kdtree/__init__.py` & `pynbody-2.0.0b9/pynbody/kdtree/__init__.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b8/pynbody/kdtree/kd.cpp` & `pynbody-2.0.0b9/pynbody/kdtree/kd.cpp`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b8/pynbody/kdtree/kd.h` & `pynbody-2.0.0b9/pynbody/kdtree/kd.h`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b8/pynbody/kdtree/kdmain.cpp` & `pynbody-2.0.0b9/pynbody/kdtree/kdmain.cpp`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b8/pynbody/kdtree/pq.h` & `pynbody-2.0.0b9/pynbody/kdtree/pq.h`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b8/pynbody/kdtree/smooth.h` & `pynbody-2.0.0b9/pynbody/kdtree/smooth.h`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b8/pynbody/openmp/openmp_real.pyx` & `pynbody-2.0.0b9/pynbody/openmp/openmp_real.pyx`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b8/pynbody/plot/__init__.py` & `pynbody-2.0.0b9/pynbody/plot/__init__.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b8/pynbody/plot/gas.py` & `pynbody-2.0.0b9/pynbody/plot/gas.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b8/pynbody/plot/generic.py` & `pynbody-2.0.0b9/pynbody/plot/generic.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b8/pynbody/plot/metals.py` & `pynbody-2.0.0b9/pynbody/plot/metals.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b8/pynbody/plot/profile.py` & `pynbody-2.0.0b9/pynbody/plot/profile.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b8/pynbody/plot/quiverkey.py` & `pynbody-2.0.0b9/pynbody/plot/quiverkey.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b8/pynbody/plot/sph.py` & `pynbody-2.0.0b9/pynbody/plot/sph.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b8/pynbody/plot/stars.py` & `pynbody-2.0.0b9/pynbody/plot/stars.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b8/pynbody/plot/util.py` & `pynbody-2.0.0b9/pynbody/plot/util.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b8/pynbody/simdict.py` & `pynbody-2.0.0b9/pynbody/simdict.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b8/pynbody/snapshot/__init__.py` & `pynbody-2.0.0b9/pynbody/snapshot/__init__.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b8/pynbody/snapshot/ascii.py` & `pynbody-2.0.0b9/pynbody/snapshot/ascii.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b8/pynbody/snapshot/copy_on_access.py` & `pynbody-2.0.0b9/pynbody/snapshot/copy_on_access.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b8/pynbody/snapshot/gadget.py` & `pynbody-2.0.0b9/pynbody/snapshot/gadget.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b8/pynbody/snapshot/gadgethdf.py` & `pynbody-2.0.0b9/pynbody/snapshot/gadgethdf.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b8/pynbody/snapshot/grafic.py` & `pynbody-2.0.0b9/pynbody/snapshot/grafic.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b8/pynbody/snapshot/namemapper.py` & `pynbody-2.0.0b9/pynbody/snapshot/namemapper.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b8/pynbody/snapshot/nchilada.py` & `pynbody-2.0.0b9/pynbody/snapshot/nchilada.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b8/pynbody/snapshot/ramses.py` & `pynbody-2.0.0b9/pynbody/snapshot/ramses.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b8/pynbody/snapshot/simsnap.py` & `pynbody-2.0.0b9/pynbody/snapshot/simsnap.py`

 * *Files 1% similar despite different names*

```diff
@@ -137,14 +137,15 @@
 
         self._arrays = {}
         self._num_particles = 0
         self._family_slice = {}
         self._family_arrays = {}
         self._derived_array_names = []
         self._family_derived_array_names = {}
+        self._get_array_lock = threading.RLock()
         for i in family._registry:
             self._family_derived_array_names[i] = []
 
         self._dependency_tracker = dependencytracker.DependencyTracker()
         self._immediate_cache_lock = threading.RLock()
 
         self._persistent_objects = {}
@@ -307,45 +308,47 @@
         if len(mask_array.shape) > 1 or mask_array.shape[0] > len(self):
             raise ValueError("Incorrect shape for masking array")
         else:
             return self[np.where(mask_array)]
 
     def _get_array_with_lazy_actions(self, name):
         """Get an array by the given name; if it's not available, attempt to load or derive it first"""
-        if name in list(self.keys()):
-            self._dependency_tracker.touching(name)
 
-            # Ensure that any underlying dependencies on 1D positions and velocities
-            # are forwarded to 3D dependencies as well
-            nd_name = self._array_name_1D_to_ND(name)
-            if nd_name is not None:
-                self._dependency_tracker.touching(nd_name)
-
-        elif not self.lazy_off:
-            # The array is not currently in memory at the level we need it, and there is a possibility
-            # of getting it into memory using lazy derivation or loading. First, if there is a family level
-            # array by the same name, dispose of it. (Note if this is being called on a FamilySubSnap, the below
-            # has no effect, and anyway we wouldn't reach this point in the code if the family array were available.)
-            self.__resolve_obscuring_family_array(name)
-
-            # Now, we'll try to load the array...
-            did_load = False
-            if not self.lazy_load_off:
-                # Note that we don't want this to be inside _dependency_tracker.calculating(name), because there is a
-                # small possibility the load will be mapped into a derivation by the loader class. Specifically this
-                # happens in ramses snapshots for the mass array (which is derived from the density array for gas cells).
-                self.__load_if_required(name)
-
-            if name in self:
-                # We managed to load it. Note the dependency.
+        # the below is not thread-safe, so we lock
+        with self._get_array_lock:
+            if name in list(self.keys()):
                 self._dependency_tracker.touching(name)
-            elif not self.lazy_derive_off:
-                # Try deriving instead
-                with self._dependency_tracker.calculating(name):
-                    self.__derive_if_required(name)
+
+                # Ensure that any underlying dependencies on 1D positions and velocities
+                # are forwarded to 3D dependencies as well
+                nd_name = self._array_name_1D_to_ND(name)
+                if nd_name is not None:
+                    self._dependency_tracker.touching(nd_name)
+
+            elif not self.lazy_off:
+                # The array is not currently in memory at the level we need it, and there is a possibility
+                # of getting it into memory using lazy derivation or loading. First, if there is a family level
+                # array by the same name, dispose of it. (Note if this is being called on a FamilySubSnap, the below
+                # has no effect, and anyway we wouldn't reach this point in the code if the family array were available.)
+                self.__resolve_obscuring_family_array(name)
+
+                # Now, we'll try to load the array...
+                if not self.lazy_load_off:
+                    # Note that we don't want this to be inside _dependency_tracker.calculating(name), because there is a
+                    # small possibility the load will be mapped into a derivation by the loader class. Specifically this
+                    # happens in ramses snapshots for the mass array (which is derived from the density array for gas cells).
+                    self.__load_if_required(name)
+
+                if name in self:
+                    # We managed to load it. Note the dependency.
+                    self._dependency_tracker.touching(name)
+                elif not self.lazy_derive_off:
+                    # Try deriving instead
+                    with self._dependency_tracker.calculating(name):
+                        self.__derive_if_required(name)
 
         # At this point we've done everything we can to get the array into memory. If it's still not there, we'll
         # get a KeyError from the below.
         return self._get_array(name)
```

### Comparing `pynbody-2.0.0b8/pynbody/snapshot/subsnap.py` & `pynbody-2.0.0b9/pynbody/snapshot/subsnap.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,21 +7,22 @@
 class ExposedBaseSnapshotMixin:
     # The following will be objects common to a SimSnap and all its SubSnaps
     _inherited = ["_immediate_cache_lock",
                   "lazy_off", "lazy_derive_off", "lazy_load_off", "auto_propagate_off",
                   "properties", "_derived_array_names", "_family_derived_array_names",
                   "_dependency_tracker", "immediate_mode", "delay_promotion"]
 
-    def __init__(self, base, *args, **kwargs):
+    def __init__(self, base: SimSnap, *args, **kwargs):
         self.base = base
         super().__init__(base, *args, **kwargs)
 
     def _inherit(self):
         self._file_units_system = self.base._file_units_system
         self._unifamily = self.base._unifamily
+        self._get_array_lock = self.base._get_array_lock
 
         for x in self._inherited:
             setattr(self, x, getattr(self.base, x))
 
 class SubSnapBase(SimSnap):
     def __init__(self, base):
         self._subsnap_base = base
```

### Comparing `pynbody-2.0.0b8/pynbody/snapshot/swift.py` & `pynbody-2.0.0b9/pynbody/snapshot/swift.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b8/pynbody/snapshot/tipsy.py` & `pynbody-2.0.0b9/pynbody/snapshot/tipsy.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b8/pynbody/snapshot/util.py` & `pynbody-2.0.0b9/pynbody/snapshot/util.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b8/pynbody/sph/__init__.py` & `pynbody-2.0.0b9/pynbody/sph/__init__.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b8/pynbody/sph/_render.pyx` & `pynbody-2.0.0b9/pynbody/sph/_render.pyx`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b8/pynbody/test_utils/gadget4_subfind_reader.py` & `pynbody-2.0.0b9/pynbody/test_utils/gadget4_subfind_reader.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b8/pynbody/test_utils/pyread_gadget_hdf5.py` & `pynbody-2.0.0b9/pynbody/test_utils/pyread_gadget_hdf5.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b8/pynbody/transformation.py` & `pynbody-2.0.0b9/pynbody/transformation.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b8/pynbody/units.py` & `pynbody-2.0.0b9/pynbody/units.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b8/pynbody/util/__init__.py` & `pynbody-2.0.0b9/pynbody/util/__init__.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b8/pynbody/util/_util.pyx` & `pynbody-2.0.0b9/pynbody/util/_util.pyx`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b8/pynbody/util/hdf_vds.py` & `pynbody-2.0.0b9/pynbody/util/hdf_vds.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b8/pynbody/util/iter_subclasses.py` & `pynbody-2.0.0b9/pynbody/util/iter_subclasses.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b8/pynbody.egg-info/PKG-INFO` & `pynbody-2.0.0b9/pynbody.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynbody
-Version: 2.0.0b8
+Version: 2.0.0b9
 Summary: Light-weight astronomical N-body/SPH analysis for python
 Home-page: https://github.com/pynbody/pynbody/releases
 Author: The pynbody team
 Author-email: pynbody@googlegroups.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pynbody-2.0.0b8/pynbody.egg-info/SOURCES.txt` & `pynbody-2.0.0b9/pynbody.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b8/pyproject.toml` & `pynbody-2.0.0b9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b8/setup.py` & `pynbody-2.0.0b9/setup.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b8/tests/adaptahop_test.py` & `pynbody-2.0.0b9/tests/adaptahop_test.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b8/tests/ahf_halos_test.py` & `pynbody-2.0.0b9/tests/ahf_halos_test.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b8/tests/array_test.py` & `pynbody-2.0.0b9/tests/array_test.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b8/tests/bridge_test.py` & `pynbody-2.0.0b9/tests/bridge_test.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b8/tests/copy_on_access_test.py` & `pynbody-2.0.0b9/tests/copy_on_access_test.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b8/tests/cosmology_test.py` & `pynbody-2.0.0b9/tests/cosmology_test.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b8/tests/derived_arrays_test.py` & `pynbody-2.0.0b9/tests/derived_arrays_test.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b8/tests/family_test.py` & `pynbody-2.0.0b9/tests/family_test.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b8/tests/filter_test.py` & `pynbody-2.0.0b9/tests/filter_test.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b8/tests/gadget_test.py` & `pynbody-2.0.0b9/tests/gadget_test.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b8/tests/gadgethdf_test.py` & `pynbody-2.0.0b9/tests/gadgethdf_test.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b8/tests/grafic_test.py` & `pynbody-2.0.0b9/tests/grafic_test.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b8/tests/gravity_test.py` & `pynbody-2.0.0b9/tests/gravity_test.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b8/tests/halos_test.py` & `pynbody-2.0.0b9/tests/halos_test.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b8/tests/halotools_test.py` & `pynbody-2.0.0b9/tests/halotools_test.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b8/tests/hbtplus_test.py` & `pynbody-2.0.0b9/tests/hbtplus_test.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b8/tests/hmf_test.py` & `pynbody-2.0.0b9/tests/hmf_test.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b8/tests/hop_test.py` & `pynbody-2.0.0b9/tests/hop_test.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b8/tests/kdtree_test.py` & `pynbody-2.0.0b9/tests/kdtree_test.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b8/tests/nchilada_test.py` & `pynbody-2.0.0b9/tests/nchilada_test.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b8/tests/partial_tipsy_test.py` & `pynbody-2.0.0b9/tests/partial_tipsy_test.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b8/tests/performance_kdtree.py` & `pynbody-2.0.0b9/tests/performance_kdtree.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b8/tests/ramses_new_ptcl_format_test.py` & `pynbody-2.0.0b9/tests/ramses_new_ptcl_format_test.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b8/tests/ramses_test.py` & `pynbody-2.0.0b9/tests/ramses_test.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b8/tests/rockstar_test.py` & `pynbody-2.0.0b9/tests/rockstar_test.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b8/tests/snapshot_test.py` & `pynbody-2.0.0b9/tests/snapshot_test.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import threading
+import time
 import weakref
 
 import numpy as np
 import pytest
 
 import pynbody
 
@@ -264,7 +266,40 @@
 
     f['test_array'] = np.arange(2000)
 
     f = f[np.arange(1000)] # test on a subsnap for generality
 
     np.testing.assert_allclose(f.mean_by_mass('test_array'),
                                (f['test_array'][:500]*2./3 + f['test_array'][500:1000]*1./3).mean())
+
+
+class SlowLoadingSnapshot(pynbody.snapshot.simsnap.SimSnap):
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        self._has_entered = False
+        self._has_exited = False
+        self._filename = "test"
+
+    def _load_array(self, array_name, fam=None):
+        if self._has_entered:
+            raise RuntimeError("Entered twice")
+        if self._has_exited:
+            raise RuntimeError("Entered after exiting")
+        self._has_entered=True
+        time.sleep(0.1)
+        self[array_name] = np.arange(len(self))
+        self._has_entered=False
+        self._has_exited=True
+
+def test_race_condition():
+    """There was a race condition where if multiple threads tried to load the same array at once, strange errors
+    would result. This has been fixed by a lock on deriving/loading data."""
+    f = SlowLoadingSnapshot()
+
+    def load_array():
+        f['anyarray'] # noqa
+
+    threads = [threading.Thread(target=load_array) for i in range(5)]
+    for t in threads:
+        t.start()
+    for t in threads:
+        t.join()
```

### Comparing `pynbody-2.0.0b8/tests/sph_image_test.py` & `pynbody-2.0.0b9/tests/sph_image_test.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b8/tests/subarray_test.py` & `pynbody-2.0.0b9/tests/subarray_test.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b8/tests/subfind_test.py` & `pynbody-2.0.0b9/tests/subfind_test.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b8/tests/subfindhdf_gadget4_test.py` & `pynbody-2.0.0b9/tests/subfindhdf_gadget4_test.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b8/tests/subfindhdf_test.py` & `pynbody-2.0.0b9/tests/subfindhdf_test.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b8/tests/swift_test.py` & `pynbody-2.0.0b9/tests/swift_test.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b8/tests/test_profile.py` & `pynbody-2.0.0b9/tests/test_profile.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b8/tests/theoretical_profile.py` & `pynbody-2.0.0b9/tests/theoretical_profile.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b8/tests/tipsy_test.py` & `pynbody-2.0.0b9/tests/tipsy_test.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b8/tests/transformation_test.py` & `pynbody-2.0.0b9/tests/transformation_test.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b8/tests/units_test.py` & `pynbody-2.0.0b9/tests/units_test.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b8/tests/utils_test.py` & `pynbody-2.0.0b9/tests/utils_test.py`

 * *Files identical despite different names*

### Comparing `pynbody-2.0.0b8/tests/velociraptor_test.py` & `pynbody-2.0.0b9/tests/velociraptor_test.py`

 * *Files identical despite different names*

