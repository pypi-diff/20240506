# Comparing `tmp/ydata-synthetic-1.3.2.tar.gz` & `tmp/ydata-synthetic-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ydata-synthetic-1.3.2.tar", last modified: Fri Dec  8 22:53:48 2023, max compression
+gzip compressed data, was "ydata-synthetic-1.4.0.tar", last modified: Mon May  6 02:52:05 2024, max compression
```

## Comparing `ydata-synthetic-1.3.2.tar` & `ydata-synthetic-1.4.0.tar`

### file list

```diff
@@ -1,109 +1,111 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 22:53:48.611849 ydata-synthetic-1.3.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2023-12-08 22:53:43.000000 ydata-synthetic-1.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      134 2023-12-08 22:53:43.000000 ydata-synthetic-1.3.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    10740 2023-12-08 22:53:48.611849 ydata-synthetic-1.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8197 2023-12-08 22:53:43.000000 ydata-synthetic-1.3.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        6 2023-12-08 22:53:47.000000 ydata-synthetic-1.3.2/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)      111 2023-12-08 22:53:43.000000 ydata-synthetic-1.3.2/requirements-docs.txt
--rw-r--r--   0 runner    (1001) docker     (127)      205 2023-12-08 22:53:43.000000 ydata-synthetic-1.3.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-08 22:53:48.611849 ydata-synthetic-1.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2424 2023-12-08 22:53:43.000000 ydata-synthetic-1.3.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 22:53:48.599849 ydata-synthetic-1.3.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 22:53:48.603849 ydata-synthetic-1.3.2/src/ydata_synthetic/
--rw-r--r--   0 runner    (1001) docker     (127)       33 2023-12-08 22:53:43.000000 ydata-synthetic-1.3.2/src/ydata_synthetic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 22:53:48.603849 ydata-synthetic-1.3.2/src/ydata_synthetic/evaluation/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-08 22:53:43.000000 ydata-synthetic-1.3.2/src/ydata_synthetic/evaluation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 22:53:48.599849 ydata-synthetic-1.3.2/src/ydata_synthetic/postprocessing/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 22:53:48.603849 ydata-synthetic-1.3.2/src/ydata_synthetic/postprocessing/regular/
--rw-r--r--   0 runner    (1001) docker     (127)     2453 2023-12-08 22:53:43.000000 ydata-synthetic-1.3.2/src/ydata_synthetic/postprocessing/regular/inverse_preprocesser.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 22:53:48.603849 ydata-synthetic-1.3.2/src/ydata_synthetic/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (127)      251 2023-12-08 22:53:43.000000 ydata-synthetic-1.3.2/src/ydata_synthetic/preprocessing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5464 2023-12-08 22:53:43.000000 ydata-synthetic-1.3.2/src/ydata_synthetic/preprocessing/base_processor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 22:53:48.607849 ydata-synthetic-1.3.2/src/ydata_synthetic/preprocessing/regular/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-08 22:53:43.000000 ydata-synthetic-1.3.2/src/ydata_synthetic/preprocessing/regular/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8210 2023-12-08 22:53:43.000000 ydata-synthetic-1.3.2/src/ydata_synthetic/preprocessing/regular/ctgan_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)     4526 2023-12-08 22:53:43.000000 ydata-synthetic-1.3.2/src/ydata_synthetic/preprocessing/regular/processor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 22:53:48.607849 ydata-synthetic-1.3.2/src/ydata_synthetic/preprocessing/timeseries/
--rw-r--r--   0 runner    (1001) docker     (127)      132 2023-12-08 22:53:43.000000 ydata-synthetic-1.3.2/src/ydata_synthetic/preprocessing/timeseries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13469 2023-12-08 22:53:43.000000 ydata-synthetic-1.3.2/src/ydata_synthetic/preprocessing/timeseries/doppelganger_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)      577 2023-12-08 22:53:43.000000 ydata-synthetic-1.3.2/src/ydata_synthetic/preprocessing/timeseries/stock.py
--rw-r--r--   0 runner    (1001) docker     (127)      581 2023-12-08 22:53:43.000000 ydata-synthetic-1.3.2/src/ydata_synthetic/preprocessing/timeseries/timeseries_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1166 2023-12-08 22:53:43.000000 ydata-synthetic-1.3.2/src/ydata_synthetic/preprocessing/timeseries/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 22:53:48.607849 ydata-synthetic-1.3.2/src/ydata_synthetic/streamlit_app/
--rw-r--r--   0 runner    (1001) docker     (127)     4196 2023-12-08 22:53:43.000000 ydata-synthetic-1.3.2/src/ydata_synthetic/streamlit_app/About.py
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-08 22:53:43.000000 ydata-synthetic-1.3.2/src/ydata_synthetic/streamlit_app/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 22:53:48.607849 ydata-synthetic-1.3.2/src/ydata_synthetic/streamlit_app/pages/
--rw-r--r--   0 runner    (1001) docker     (127)     5723 2023-12-08 22:53:43.000000 ydata-synthetic-1.3.2/src/ydata_synthetic/streamlit_app/pages/1_Train_a_synthesizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2947 2023-12-08 22:53:43.000000 ydata-synthetic-1.3.2/src/ydata_synthetic/streamlit_app/pages/2_Generate_synthetic_data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 22:53:48.607849 ydata-synthetic-1.3.2/src/ydata_synthetic/streamlit_app/pages/functions/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-08 22:53:43.000000 ydata-synthetic-1.3.2/src/ydata_synthetic/streamlit_app/pages/functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      789 2023-12-08 22:53:43.000000 ydata-synthetic-1.3.2/src/ydata_synthetic/streamlit_app/pages/functions/generate.py
--rw-r--r--   0 runner    (1001) docker     (127)      694 2023-12-08 22:53:43.000000 ydata-synthetic-1.3.2/src/ydata_synthetic/streamlit_app/pages/functions/load_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1843 2023-12-08 22:53:43.000000 ydata-synthetic-1.3.2/src/ydata_synthetic/streamlit_app/pages/functions/train.py
--rw-r--r--   0 runner    (1001) docker     (127)      363 2023-12-08 22:53:43.000000 ydata-synthetic-1.3.2/src/ydata_synthetic/streamlit_app/run.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 22:53:48.607849 ydata-synthetic-1.3.2/src/ydata_synthetic/synthesizers/
--rw-r--r--   0 runner    (1001) docker     (127)      138 2023-12-08 22:53:43.000000 ydata-synthetic-1.3.2/src/ydata_synthetic/synthesizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13300 2023-12-08 22:53:43.000000 ydata-synthetic-1.3.2/src/ydata_synthetic/synthesizers/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2849 2023-12-08 22:53:43.000000 ydata-synthetic-1.3.2/src/ydata_synthetic/synthesizers/loss.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 22:53:48.607849 ydata-synthetic-1.3.2/src/ydata_synthetic/synthesizers/regular/
--rw-r--r--   0 runner    (1001) docker     (127)      115 2023-12-08 22:53:43.000000 ydata-synthetic-1.3.2/src/ydata_synthetic/synthesizers/regular/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 22:53:48.607849 ydata-synthetic-1.3.2/src/ydata_synthetic/synthesizers/regular/cgan/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-08 22:53:43.000000 ydata-synthetic-1.3.2/src/ydata_synthetic/synthesizers/regular/cgan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9612 2023-12-08 22:53:43.000000 ydata-synthetic-1.3.2/src/ydata_synthetic/synthesizers/regular/cgan/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 22:53:48.607849 ydata-synthetic-1.3.2/src/ydata_synthetic/synthesizers/regular/cramergan/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-08 22:53:43.000000 ydata-synthetic-1.3.2/src/ydata_synthetic/synthesizers/regular/cramergan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10646 2023-12-08 22:53:43.000000 ydata-synthetic-1.3.2/src/ydata_synthetic/synthesizers/regular/cramergan/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 22:53:48.607849 ydata-synthetic-1.3.2/src/ydata_synthetic/synthesizers/regular/ctgan/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2023-12-08 22:53:43.000000 ydata-synthetic-1.3.2/src/ydata_synthetic/synthesizers/regular/ctgan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14122 2023-12-08 22:53:43.000000 ydata-synthetic-1.3.2/src/ydata_synthetic/synthesizers/regular/ctgan/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5343 2023-12-08 22:53:43.000000 ydata-synthetic-1.3.2/src/ydata_synthetic/synthesizers/regular/ctgan/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 22:53:48.607849 ydata-synthetic-1.3.2/src/ydata_synthetic/synthesizers/regular/cwgangp/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-08 22:53:43.000000 ydata-synthetic-1.3.2/src/ydata_synthetic/synthesizers/regular/cwgangp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10283 2023-12-08 22:53:43.000000 ydata-synthetic-1.3.2/src/ydata_synthetic/synthesizers/regular/cwgangp/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 22:53:48.611849 ydata-synthetic-1.3.2/src/ydata_synthetic/synthesizers/regular/dragan/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-08 22:53:43.000000 ydata-synthetic-1.3.2/src/ydata_synthetic/synthesizers/regular/dragan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10062 2023-12-08 22:53:43.000000 ydata-synthetic-1.3.2/src/ydata_synthetic/synthesizers/regular/dragan/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 22:53:48.611849 ydata-synthetic-1.3.2/src/ydata_synthetic/synthesizers/regular/gmm/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-08 22:53:43.000000 ydata-synthetic-1.3.2/src/ydata_synthetic/synthesizers/regular/gmm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3804 2023-12-08 22:53:43.000000 ydata-synthetic-1.3.2/src/ydata_synthetic/synthesizers/regular/gmm/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2408 2023-12-08 22:53:43.000000 ydata-synthetic-1.3.2/src/ydata_synthetic/synthesizers/regular/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 22:53:48.611849 ydata-synthetic-1.3.2/src/ydata_synthetic/synthesizers/regular/vanillagan/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-08 22:53:43.000000 ydata-synthetic-1.3.2/src/ydata_synthetic/synthesizers/regular/vanillagan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8162 2023-12-08 22:53:43.000000 ydata-synthetic-1.3.2/src/ydata_synthetic/synthesizers/regular/vanillagan/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 22:53:48.611849 ydata-synthetic-1.3.2/src/ydata_synthetic/synthesizers/regular/wgan/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-08 22:53:43.000000 ydata-synthetic-1.3.2/src/ydata_synthetic/synthesizers/regular/wgan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9741 2023-12-08 22:53:43.000000 ydata-synthetic-1.3.2/src/ydata_synthetic/synthesizers/regular/wgan/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 22:53:48.611849 ydata-synthetic-1.3.2/src/ydata_synthetic/synthesizers/regular/wgangp/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-08 22:53:43.000000 ydata-synthetic-1.3.2/src/ydata_synthetic/synthesizers/regular/wgangp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10518 2023-12-08 22:53:43.000000 ydata-synthetic-1.3.2/src/ydata_synthetic/synthesizers/regular/wgangp/model.py
--rw-r--r--   0 runner    (1001) docker     (127)      802 2023-12-08 22:53:43.000000 ydata-synthetic-1.3.2/src/ydata_synthetic/synthesizers/saving_keras.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 22:53:48.611849 ydata-synthetic-1.3.2/src/ydata_synthetic/synthesizers/timeseries/
--rw-r--r--   0 runner    (1001) docker     (127)      123 2023-12-08 22:53:43.000000 ydata-synthetic-1.3.2/src/ydata_synthetic/synthesizers/timeseries/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 22:53:48.611849 ydata-synthetic-1.3.2/src/ydata_synthetic/synthesizers/timeseries/doppelganger/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-08 22:53:43.000000 ydata-synthetic-1.3.2/src/ydata_synthetic/synthesizers/timeseries/doppelganger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    27896 2023-12-08 22:53:43.000000 ydata-synthetic-1.3.2/src/ydata_synthetic/synthesizers/timeseries/doppelganger/doppelganger.py
--rw-r--r--   0 runner    (1001) docker     (127)     9148 2023-12-08 22:53:43.000000 ydata-synthetic-1.3.2/src/ydata_synthetic/synthesizers/timeseries/doppelganger/model.py
--rw-r--r--   0 runner    (1001) docker     (127)    21210 2023-12-08 22:53:43.000000 ydata-synthetic-1.3.2/src/ydata_synthetic/synthesizers/timeseries/doppelganger/network.py
--rw-r--r--   0 runner    (1001) docker     (127)     1430 2023-12-08 22:53:43.000000 ydata-synthetic-1.3.2/src/ydata_synthetic/synthesizers/timeseries/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 22:53:48.611849 ydata-synthetic-1.3.2/src/ydata_synthetic/synthesizers/timeseries/timegan/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-08 22:53:43.000000 ydata-synthetic-1.3.2/src/ydata_synthetic/synthesizers/timeseries/timegan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15136 2023-12-08 22:53:43.000000 ydata-synthetic-1.3.2/src/ydata_synthetic/synthesizers/timeseries/timegan/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 22:53:48.603849 ydata-synthetic-1.3.2/src/ydata_synthetic/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 22:53:48.611849 ydata-synthetic-1.3.2/src/ydata_synthetic/tests/custom_layers/
--rw-r--r--   0 runner    (1001) docker     (127)     3315 2023-12-08 22:53:43.000000 ydata-synthetic-1.3.2/src/ydata_synthetic/tests/custom_layers/test_gumbel_softmax_activation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2714 2023-12-08 22:53:43.000000 ydata-synthetic-1.3.2/src/ydata_synthetic/tests/custom_layers/test_gumbel_softmax_layer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 22:53:48.611849 ydata-synthetic-1.3.2/src/ydata_synthetic/tests/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (127)     3368 2023-12-08 22:53:43.000000 ydata-synthetic-1.3.2/src/ydata_synthetic/tests/preprocessing/test_regular_data_processor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 22:53:48.611849 ydata-synthetic-1.3.2/src/ydata_synthetic/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-08 22:53:43.000000 ydata-synthetic-1.3.2/src/ydata_synthetic/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2050 2023-12-08 22:53:43.000000 ydata-synthetic-1.3.2/src/ydata_synthetic/utils/cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     4346 2023-12-08 22:53:43.000000 ydata-synthetic-1.3.2/src/ydata_synthetic/utils/gumbel_softmax.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 22:53:48.611849 ydata-synthetic-1.3.2/src/ydata_synthetic/utils/misc/
--rw-r--r--   0 runner    (1001) docker     (127)     1145 2023-12-08 22:53:43.000000 ydata-synthetic-1.3.2/src/ydata_synthetic/utils/misc/colormaps.py
--rw-r--r--   0 runner    (1001) docker     (127)       21 2023-12-08 22:53:48.000000 ydata-synthetic-1.3.2/src/ydata_synthetic/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 22:53:48.603849 ydata-synthetic-1.3.2/src/ydata_synthetic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10740 2023-12-08 22:53:48.000000 ydata-synthetic-1.3.2/src/ydata_synthetic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3828 2023-12-08 22:53:48.000000 ydata-synthetic-1.3.2/src/ydata_synthetic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-08 22:53:48.000000 ydata-synthetic-1.3.2/src/ydata_synthetic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      335 2023-12-08 22:53:48.000000 ydata-synthetic-1.3.2/src/ydata_synthetic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2023-12-08 22:53:48.000000 ydata-synthetic-1.3.2/src/ydata_synthetic.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 02:52:05.106477 ydata-synthetic-1.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-06 02:52:01.000000 ydata-synthetic-1.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-06 02:52:01.000000 ydata-synthetic-1.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     9611 2024-05-06 02:52:05.106477 ydata-synthetic-1.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8197 2024-05-06 02:52:01.000000 ydata-synthetic-1.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-06 02:52:04.000000 ydata-synthetic-1.4.0/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-06 02:52:01.000000 ydata-synthetic-1.4.0/requirements-docs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-06 02:52:01.000000 ydata-synthetic-1.4.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 02:52:05.106477 ydata-synthetic-1.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2420 2024-05-06 02:52:01.000000 ydata-synthetic-1.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 02:52:05.094477 ydata-synthetic-1.4.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 02:52:05.098477 ydata-synthetic-1.4.0/src/ydata_synthetic/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-06 02:52:01.000000 ydata-synthetic-1.4.0/src/ydata_synthetic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 02:52:05.098477 ydata-synthetic-1.4.0/src/ydata_synthetic/evaluation/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 02:52:01.000000 ydata-synthetic-1.4.0/src/ydata_synthetic/evaluation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 02:52:05.094477 ydata-synthetic-1.4.0/src/ydata_synthetic/postprocessing/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 02:52:05.098477 ydata-synthetic-1.4.0/src/ydata_synthetic/postprocessing/regular/
+-rw-r--r--   0 runner    (1001) docker     (127)     2453 2024-05-06 02:52:01.000000 ydata-synthetic-1.4.0/src/ydata_synthetic/postprocessing/regular/inverse_preprocesser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 02:52:05.098477 ydata-synthetic-1.4.0/src/ydata_synthetic/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-05-06 02:52:01.000000 ydata-synthetic-1.4.0/src/ydata_synthetic/preprocessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5464 2024-05-06 02:52:01.000000 ydata-synthetic-1.4.0/src/ydata_synthetic/preprocessing/base_processor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 02:52:05.098477 ydata-synthetic-1.4.0/src/ydata_synthetic/preprocessing/regular/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 02:52:01.000000 ydata-synthetic-1.4.0/src/ydata_synthetic/preprocessing/regular/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8210 2024-05-06 02:52:01.000000 ydata-synthetic-1.4.0/src/ydata_synthetic/preprocessing/regular/ctgan_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4526 2024-05-06 02:52:01.000000 ydata-synthetic-1.4.0/src/ydata_synthetic/preprocessing/regular/processor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 02:52:05.098477 ydata-synthetic-1.4.0/src/ydata_synthetic/preprocessing/timeseries/
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-06 02:52:01.000000 ydata-synthetic-1.4.0/src/ydata_synthetic/preprocessing/timeseries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13469 2024-05-06 02:52:01.000000 ydata-synthetic-1.4.0/src/ydata_synthetic/preprocessing/timeseries/doppelganger_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      577 2024-05-06 02:52:01.000000 ydata-synthetic-1.4.0/src/ydata_synthetic/preprocessing/timeseries/stock.py
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-05-06 02:52:01.000000 ydata-synthetic-1.4.0/src/ydata_synthetic/preprocessing/timeseries/timeseries_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-05-06 02:52:01.000000 ydata-synthetic-1.4.0/src/ydata_synthetic/preprocessing/timeseries/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 02:52:05.098477 ydata-synthetic-1.4.0/src/ydata_synthetic/streamlit_app/
+-rw-r--r--   0 runner    (1001) docker     (127)     4196 2024-05-06 02:52:01.000000 ydata-synthetic-1.4.0/src/ydata_synthetic/streamlit_app/About.py
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-06 02:52:01.000000 ydata-synthetic-1.4.0/src/ydata_synthetic/streamlit_app/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 02:52:05.098477 ydata-synthetic-1.4.0/src/ydata_synthetic/streamlit_app/pages/
+-rw-r--r--   0 runner    (1001) docker     (127)     5950 2024-05-06 02:52:01.000000 ydata-synthetic-1.4.0/src/ydata_synthetic/streamlit_app/pages/1_Train_a_synthesizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2947 2024-05-06 02:52:01.000000 ydata-synthetic-1.4.0/src/ydata_synthetic/streamlit_app/pages/2_Generate_synthetic_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 02:52:05.102477 ydata-synthetic-1.4.0/src/ydata_synthetic/streamlit_app/pages/functions/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 02:52:01.000000 ydata-synthetic-1.4.0/src/ydata_synthetic/streamlit_app/pages/functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      789 2024-05-06 02:52:01.000000 ydata-synthetic-1.4.0/src/ydata_synthetic/streamlit_app/pages/functions/generate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-05-06 02:52:01.000000 ydata-synthetic-1.4.0/src/ydata_synthetic/streamlit_app/pages/functions/load_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1857 2024-05-06 02:52:01.000000 ydata-synthetic-1.4.0/src/ydata_synthetic/streamlit_app/pages/functions/train.py
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-05-06 02:52:01.000000 ydata-synthetic-1.4.0/src/ydata_synthetic/streamlit_app/run.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 02:52:05.102477 ydata-synthetic-1.4.0/src/ydata_synthetic/synthesizers/
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-06 02:52:01.000000 ydata-synthetic-1.4.0/src/ydata_synthetic/synthesizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13300 2024-05-06 02:52:01.000000 ydata-synthetic-1.4.0/src/ydata_synthetic/synthesizers/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2849 2024-05-06 02:52:01.000000 ydata-synthetic-1.4.0/src/ydata_synthetic/synthesizers/loss.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 02:52:05.102477 ydata-synthetic-1.4.0/src/ydata_synthetic/synthesizers/regular/
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-06 02:52:01.000000 ydata-synthetic-1.4.0/src/ydata_synthetic/synthesizers/regular/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 02:52:05.102477 ydata-synthetic-1.4.0/src/ydata_synthetic/synthesizers/regular/cgan/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 02:52:01.000000 ydata-synthetic-1.4.0/src/ydata_synthetic/synthesizers/regular/cgan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9612 2024-05-06 02:52:01.000000 ydata-synthetic-1.4.0/src/ydata_synthetic/synthesizers/regular/cgan/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 02:52:05.102477 ydata-synthetic-1.4.0/src/ydata_synthetic/synthesizers/regular/cramergan/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 02:52:01.000000 ydata-synthetic-1.4.0/src/ydata_synthetic/synthesizers/regular/cramergan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10646 2024-05-06 02:52:01.000000 ydata-synthetic-1.4.0/src/ydata_synthetic/synthesizers/regular/cramergan/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 02:52:05.102477 ydata-synthetic-1.4.0/src/ydata_synthetic/synthesizers/regular/ctgan/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-06 02:52:01.000000 ydata-synthetic-1.4.0/src/ydata_synthetic/synthesizers/regular/ctgan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14122 2024-05-06 02:52:01.000000 ydata-synthetic-1.4.0/src/ydata_synthetic/synthesizers/regular/ctgan/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5343 2024-05-06 02:52:01.000000 ydata-synthetic-1.4.0/src/ydata_synthetic/synthesizers/regular/ctgan/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 02:52:05.102477 ydata-synthetic-1.4.0/src/ydata_synthetic/synthesizers/regular/cwgangp/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 02:52:01.000000 ydata-synthetic-1.4.0/src/ydata_synthetic/synthesizers/regular/cwgangp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10283 2024-05-06 02:52:01.000000 ydata-synthetic-1.4.0/src/ydata_synthetic/synthesizers/regular/cwgangp/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 02:52:05.102477 ydata-synthetic-1.4.0/src/ydata_synthetic/synthesizers/regular/dragan/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 02:52:01.000000 ydata-synthetic-1.4.0/src/ydata_synthetic/synthesizers/regular/dragan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10062 2024-05-06 02:52:01.000000 ydata-synthetic-1.4.0/src/ydata_synthetic/synthesizers/regular/dragan/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 02:52:05.102477 ydata-synthetic-1.4.0/src/ydata_synthetic/synthesizers/regular/gmm/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 02:52:01.000000 ydata-synthetic-1.4.0/src/ydata_synthetic/synthesizers/regular/gmm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3804 2024-05-06 02:52:01.000000 ydata-synthetic-1.4.0/src/ydata_synthetic/synthesizers/regular/gmm/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2625 2024-05-06 02:52:01.000000 ydata-synthetic-1.4.0/src/ydata_synthetic/synthesizers/regular/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 02:52:05.102477 ydata-synthetic-1.4.0/src/ydata_synthetic/synthesizers/regular/vanillagan/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 02:52:01.000000 ydata-synthetic-1.4.0/src/ydata_synthetic/synthesizers/regular/vanillagan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8162 2024-05-06 02:52:01.000000 ydata-synthetic-1.4.0/src/ydata_synthetic/synthesizers/regular/vanillagan/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 02:52:05.102477 ydata-synthetic-1.4.0/src/ydata_synthetic/synthesizers/regular/wgan/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 02:52:01.000000 ydata-synthetic-1.4.0/src/ydata_synthetic/synthesizers/regular/wgan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9741 2024-05-06 02:52:01.000000 ydata-synthetic-1.4.0/src/ydata_synthetic/synthesizers/regular/wgan/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 02:52:05.102477 ydata-synthetic-1.4.0/src/ydata_synthetic/synthesizers/regular/wgangp/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 02:52:01.000000 ydata-synthetic-1.4.0/src/ydata_synthetic/synthesizers/regular/wgangp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10518 2024-05-06 02:52:01.000000 ydata-synthetic-1.4.0/src/ydata_synthetic/synthesizers/regular/wgangp/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      853 2024-05-06 02:52:01.000000 ydata-synthetic-1.4.0/src/ydata_synthetic/synthesizers/saving_keras.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 02:52:05.106477 ydata-synthetic-1.4.0/src/ydata_synthetic/synthesizers/timeseries/
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-06 02:52:01.000000 ydata-synthetic-1.4.0/src/ydata_synthetic/synthesizers/timeseries/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 02:52:05.106477 ydata-synthetic-1.4.0/src/ydata_synthetic/synthesizers/timeseries/doppelganger/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 02:52:01.000000 ydata-synthetic-1.4.0/src/ydata_synthetic/synthesizers/timeseries/doppelganger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27896 2024-05-06 02:52:01.000000 ydata-synthetic-1.4.0/src/ydata_synthetic/synthesizers/timeseries/doppelganger/doppelganger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9148 2024-05-06 02:52:01.000000 ydata-synthetic-1.4.0/src/ydata_synthetic/synthesizers/timeseries/doppelganger/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21210 2024-05-06 02:52:01.000000 ydata-synthetic-1.4.0/src/ydata_synthetic/synthesizers/timeseries/doppelganger/network.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1648 2024-05-06 02:52:01.000000 ydata-synthetic-1.4.0/src/ydata_synthetic/synthesizers/timeseries/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 02:52:05.106477 ydata-synthetic-1.4.0/src/ydata_synthetic/synthesizers/timeseries/timegan/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 02:52:01.000000 ydata-synthetic-1.4.0/src/ydata_synthetic/synthesizers/timeseries/timegan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15136 2024-05-06 02:52:01.000000 ydata-synthetic-1.4.0/src/ydata_synthetic/synthesizers/timeseries/timegan/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 02:52:05.094477 ydata-synthetic-1.4.0/src/ydata_synthetic/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 02:52:05.106477 ydata-synthetic-1.4.0/src/ydata_synthetic/tests/custom_layers/
+-rw-r--r--   0 runner    (1001) docker     (127)     3315 2024-05-06 02:52:01.000000 ydata-synthetic-1.4.0/src/ydata_synthetic/tests/custom_layers/test_gumbel_softmax_activation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2714 2024-05-06 02:52:01.000000 ydata-synthetic-1.4.0/src/ydata_synthetic/tests/custom_layers/test_gumbel_softmax_layer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 02:52:05.106477 ydata-synthetic-1.4.0/src/ydata_synthetic/tests/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (127)     3368 2024-05-06 02:52:01.000000 ydata-synthetic-1.4.0/src/ydata_synthetic/tests/preprocessing/test_regular_data_processor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 02:52:05.106477 ydata-synthetic-1.4.0/src/ydata_synthetic/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 02:52:01.000000 ydata-synthetic-1.4.0/src/ydata_synthetic/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2050 2024-05-06 02:52:01.000000 ydata-synthetic-1.4.0/src/ydata_synthetic/utils/cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4346 2024-05-06 02:52:01.000000 ydata-synthetic-1.4.0/src/ydata_synthetic/utils/gumbel_softmax.py
+-rw-r--r--   0 runner    (1001) docker     (127)      627 2024-05-06 02:52:01.000000 ydata-synthetic-1.4.0/src/ydata_synthetic/utils/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 02:52:05.106477 ydata-synthetic-1.4.0/src/ydata_synthetic/utils/misc/
+-rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-05-06 02:52:01.000000 ydata-synthetic-1.4.0/src/ydata_synthetic/utils/misc/colormaps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-05-06 02:52:01.000000 ydata-synthetic-1.4.0/src/ydata_synthetic/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-06 02:52:04.000000 ydata-synthetic-1.4.0/src/ydata_synthetic/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 02:52:05.098477 ydata-synthetic-1.4.0/src/ydata_synthetic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9611 2024-05-06 02:52:05.000000 ydata-synthetic-1.4.0/src/ydata_synthetic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3899 2024-05-06 02:52:05.000000 ydata-synthetic-1.4.0/src/ydata_synthetic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 02:52:05.000000 ydata-synthetic-1.4.0/src/ydata_synthetic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      305 2024-05-06 02:52:05.000000 ydata-synthetic-1.4.0/src/ydata_synthetic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-06 02:52:05.000000 ydata-synthetic-1.4.0/src/ydata_synthetic.egg-info/top_level.txt
```

### Comparing `ydata-synthetic-1.3.2/LICENSE` & `ydata-synthetic-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ydata-synthetic-1.3.2/PKG-INFO` & `ydata-synthetic-1.4.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,158 +1,16 @@
 Metadata-Version: 2.1
 Name: ydata-synthetic
-Version: 1.3.2
+Version: 1.4.0
 Summary: Synthetic data generation methods with different synthetization methods.
 Home-page: https://github.com/ydataai/ydata-synthetic
 Author: YData
 Author-email: community@ydata.ai
 License: https://github.com/ydataai/ydata-synthetic/blob/master/LICENSE
-Description: ![](https://img.shields.io/github/workflow/status/ydataai/ydata-synthetic/prerelease)
-        ![](https://img.shields.io/pypi/status/ydata-synthetic)
-        [![](https://pepy.tech/badge/ydata-synthetic)](https://pypi.org/project/ydata-synthetic/)
-        ![](https://img.shields.io/badge/python-3.9%20%7C%203.10-blue)
-        [![](https://img.shields.io/pypi/v/ydata-synthetic)](https://pypi.org/project/ydata-synthetic/)
-        ![](https://img.shields.io/github/license/ydataai/ydata-synthetic)
-        
-        <p align="center"><img width="300" src="https://assets.ydata.ai/oss/ydata-synthetic_black.png" alt="YData Synthetic Logo"></p>
-        
-        Join us on [![Discord](https://img.shields.io/badge/Discord-7289DA?style=for-the-badge&logo=discord&logoColor=white)](https://tiny.ydata.ai/dcai-ydata-synthetic)
-        
-        # YData Synthetic
-        A package to generate synthetic tabular and time-series data leveraging the state of the art generative models.
-        
-        ## 🎊 The exciting features:
-        > These are must try features when it comes to synthetic data generation:
-          > - A new streamlit app that delivers the synthetic data generation experience with a UI interface. A low code experience for the quick generation of synthetic data
-          > - A new fast synthetic data generation model based on Gaussian Mixture. So you can quickstart in the world of synthetic data generation without the need for a GPU.
-          > - A conditional architecture for tabular data: CTGAN, which will make the process of synthetic data generation easier and with higher quality!
-          
-        ## Synthetic data
-        ### What is synthetic data?
-        Synthetic data is artificially generated data that is not collected from real world events. It replicates the statistical components of real data without containing any identifiable information, ensuring individuals' privacy.
-        
-        ### Why Synthetic Data?
-        Synthetic data can be used for many applications:
-          - Privacy compliance for data-sharing and Machine Learning development
-          - Remove bias
-          - Balance datasets
-          - Augment datasets
-        
-        > **Looking for an end-to-end solution to Synthetic Data Generation?**<br>
-        > [YData Fabric](https://ydata.ai/products/synthetic_data) enables the generation of high-quality datasets within a full UI experience, from data preparation to synthetic data generation and evaluation.<br>
-        > Check out the [Community Version](https://ydata.ai/ydata-fabric-free-trial).
-        
-        
-        # ydata-synthetic
-        This repository contains material related with architectures and models for synthetic data, from Generative Adversarial Networks (GANs) to Gaussian Mixtures.
-        The repo includes a full ecosystem for synthetic data generation, that includes different models for the generation of synthetic structure data and time-series.
-        All the Deep Learning models are implemented leveraging Tensorflow 2.0.
-        Several example Jupyter Notebooks and Python scripts are included, to show how to use the different architectures.
-        
-        Are you ready to learn more about synthetic data and the bext-practices for synthetic data generation?
-        
-        ## Quickstart
-        The source code is currently hosted on GitHub at: https://github.com/ydataai/ydata-synthetic
-        
-        Binary installers for the latest released version are available at the [Python Package Index (PyPI).](https://pypi.org/project/ydata-synthetic/)
-        ```commandline
-        pip install ydata-synthetic
-        ```
-        
-        ### The UI guide for synthetic data generation
-        
-        YData synthetic has now a UI interface to guide you through the steps and inputs to generate structure tabular data.
-        The streamlit app is available form *v1.0.0* onwards, and supports the following flows:
-        - Train a synthesizer model
-        - Generate & profile synthetic data samples
-        
-        #### Installation
-        
-        ```commandline
-        pip install ydata-synthetic[streamlit]
-        ```
-        #### Quickstart
-        Use the code snippet below in a python file (Jupyter Notebooks are not supported):
-        ```python
-        from ydata_synthetic import streamlit_app
-        
-        streamlit_app.run()
-        ```
-        
-        Or use the file streamlit_app.py that can be found in the [examples folder](https://github.com/ydataai/ydata-synthetic/tree/master/examples/streamlit_app.py).
-        
-        ```commandline
-        python -m streamlit_app
-        ```
-        
-        The below models are supported:
-          - CGAN
-          - WGAN
-          - WGANGP
-          - DRAGAN
-          - CRAMER
-          - CTGAN
-        
-        [![Watch the video](assets/streamlit_app.png)](https://youtu.be/ep0PhwsFx0A)
-        
-        ### Examples
-        Here you can find usage examples of the package and models to synthesize tabular data.
-          - Fast tabular data synthesis on adult census income dataset [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/ydataai/ydata-synthetic/blob/master/examples/regular/models/Fast_Adult_Census_Income_Data.ipynb)
-          - Tabular synthetic data generation with CTGAN on adult census income dataset [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/ydataai/ydata-synthetic/blob/master/examples/regular/models/CTGAN_Adult_Census_Income_Data.ipynb)
-          - Time Series synthetic data generation with TimeGAN on stock dataset [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/ydataai/ydata-synthetic/blob/master/examples/timeseries/TimeGAN_Synthetic_stock_data.ipynb)
-          - Time Series synthetic data generation with DoppelGANger on FCC MBA dataset [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/ydataai/ydata-synthetic/blob/master/examples/timeseries/DoppelGANger_FCC_MBA_Dataset.ipynb)
-          - More examples are continuously added and can be found in `/examples` directory.
-        
-        ### Datasets for you to experiment
-        Here are some example datasets for you to try with the synthesizers:
-        #### Tabular datasets
-        - [Adult Census Income](https://www.kaggle.com/datasets/uciml/adult-census-income)
-        - [Credit card fraud](https://www.kaggle.com/mlg-ulb/creditcardfraud)
-        - [Cardiovascular Disease dataset](https://www.kaggle.com/datasets/sulianova/cardiovascular-disease-dataset)
-        
-        #### Sequential datasets
-        - [Stock data](https://github.com/ydataai/ydata-synthetic/tree/master/data)
-        - [FCC MBA data](https://github.com/ydataai/ydata-synthetic/tree/master/data)
-        
-        ## Project Resources
-        
-        In this repository you can find the several GAN architectures that are used to create synthesizers:
-        
-        ### Tabular data
-          - [GAN](https://arxiv.org/abs/1406.2661)
-          - [CGAN (Conditional GAN)](https://arxiv.org/abs/1411.1784)
-          - [WGAN (Wasserstein GAN)](https://arxiv.org/abs/1701.07875)
-          - [WGAN-GP (Wassertein GAN with Gradient Penalty)](https://arxiv.org/abs/1704.00028)
-          - [DRAGAN (On Convergence and stability of GANS)](https://arxiv.org/pdf/1705.07215.pdf)
-          - [Cramer GAN (The Cramer Distance as a Solution to Biased Wasserstein Gradients)](https://arxiv.org/abs/1705.10743)
-          - [CWGAN-GP (Conditional Wassertein GAN with Gradient Penalty)](https://cameronfabbri.github.io/papers/conditionalWGAN.pdf)
-          - [CTGAN (Conditional Tabular GAN)](https://arxiv.org/pdf/1907.00503.pdf)
-          - [Gaussian Mixture](https://towardsdatascience.com/gaussian-mixture-models-explained-6986aaf5a95)
-        
-        ### Sequential data
-          - [TimeGAN](https://papers.nips.cc/paper/2019/file/c9efe5f26cd17ba6216bbe2a7d26d490-Paper.pdf)
-          - [DoppelGANger](https://dl.acm.org/doi/pdf/10.1145/3419394.3423643)
-        
-        ## Contributing
-        We are open to collaboration! If you want to start contributing you only need to:
-          1. Search for an issue in which you would like to work. Issues for newcomers are labeled with good first issue.
-          2. Create a PR solving the issue.
-          3. We would review every PRs and either accept or ask for revisions.
-        
-        ## Support
-        For support in using this library, please join our Discord server. Our Discord community is very friendly and great about quickly answering questions about the use and development of the library. [Click here to join our Discord community!](https://tiny.ydata.ai/dcai-ydata-synthetic)
-        
-        ## FAQs
-        Have a question? Check out the [Frequently Asked Questions](https://ydata.ai/resources/10-most-asked-questions-on-ydata-synthetic) about `ydata-synthetic`. If you feel something is missing, feel free to [book a beary informal chat with us](https://meetings.hubspot.com/fabiana-clemente).
-        
-        ## License
-        [MIT License](https://github.com/ydataai/ydata-synthetic/blob/master/LICENSE)
-        
 Keywords: data science ydata
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: Intended Audience :: Healthcare Industry
 Classifier: Intended Audience :: Science/Research
@@ -162,10 +20,152 @@
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.9, <3.11
+Requires-Python: >=3.9, <3.12
 Description-Content-Type: text/markdown
 Provides-Extra: streamlit
+License-File: LICENSE
+
+![](https://img.shields.io/github/workflow/status/ydataai/ydata-synthetic/prerelease)
+![](https://img.shields.io/pypi/status/ydata-synthetic)
+[![](https://pepy.tech/badge/ydata-synthetic)](https://pypi.org/project/ydata-synthetic/)
+![](https://img.shields.io/badge/python-3.9%20%7C%203.10-blue)
+[![](https://img.shields.io/pypi/v/ydata-synthetic)](https://pypi.org/project/ydata-synthetic/)
+![](https://img.shields.io/github/license/ydataai/ydata-synthetic)
+
+<p align="center"><img width="300" src="https://assets.ydata.ai/oss/ydata-synthetic_black.png" alt="YData Synthetic Logo"></p>
+
+Join us on [![Discord](https://img.shields.io/badge/Discord-7289DA?style=for-the-badge&logo=discord&logoColor=white)](https://tiny.ydata.ai/dcai-ydata-synthetic)
+
+# YData Synthetic
+A package to generate synthetic tabular and time-series data leveraging the state of the art generative models.
+
+## 🎊 The exciting features:
+> These are must try features when it comes to synthetic data generation:
+  > - A new streamlit app that delivers the synthetic data generation experience with a UI interface. A low code experience for the quick generation of synthetic data
+  > - A new fast synthetic data generation model based on Gaussian Mixture. So you can quickstart in the world of synthetic data generation without the need for a GPU.
+  > - A conditional architecture for tabular data: CTGAN, which will make the process of synthetic data generation easier and with higher quality!
+  
+## Synthetic data
+### What is synthetic data?
+Synthetic data is artificially generated data that is not collected from real world events. It replicates the statistical components of real data without containing any identifiable information, ensuring individuals' privacy.
+
+### Why Synthetic Data?
+Synthetic data can be used for many applications:
+  - Privacy compliance for data-sharing and Machine Learning development
+  - Remove bias
+  - Balance datasets
+  - Augment datasets
+
+> **Looking for an end-to-end solution to Synthetic Data Generation?**<br>
+> [YData Fabric](https://ydata.ai/products/synthetic_data) enables the generation of high-quality datasets within a full UI experience, from data preparation to synthetic data generation and evaluation.<br>
+> Check out the [Community Version](https://ydata.ai/ydata-fabric-free-trial).
+
+
+# ydata-synthetic
+This repository contains material related with architectures and models for synthetic data, from Generative Adversarial Networks (GANs) to Gaussian Mixtures.
+The repo includes a full ecosystem for synthetic data generation, that includes different models for the generation of synthetic structure data and time-series.
+All the Deep Learning models are implemented leveraging Tensorflow 2.0.
+Several example Jupyter Notebooks and Python scripts are included, to show how to use the different architectures.
+
+Are you ready to learn more about synthetic data and the bext-practices for synthetic data generation?
+
+## Quickstart
+The source code is currently hosted on GitHub at: https://github.com/ydataai/ydata-synthetic
+
+Binary installers for the latest released version are available at the [Python Package Index (PyPI).](https://pypi.org/project/ydata-synthetic/)
+```commandline
+pip install ydata-synthetic
+```
+
+### The UI guide for synthetic data generation
+
+YData synthetic has now a UI interface to guide you through the steps and inputs to generate structure tabular data.
+The streamlit app is available form *v1.0.0* onwards, and supports the following flows:
+- Train a synthesizer model
+- Generate & profile synthetic data samples
+
+#### Installation
+
+```commandline
+pip install ydata-synthetic[streamlit]
+```
+#### Quickstart
+Use the code snippet below in a python file (Jupyter Notebooks are not supported):
+```python
+from ydata_synthetic import streamlit_app
+
+streamlit_app.run()
+```
+
+Or use the file streamlit_app.py that can be found in the [examples folder](https://github.com/ydataai/ydata-synthetic/tree/master/examples/streamlit_app.py).
+
+```commandline
+python -m streamlit_app
+```
+
+The below models are supported:
+  - CGAN
+  - WGAN
+  - WGANGP
+  - DRAGAN
+  - CRAMER
+  - CTGAN
+
+[![Watch the video](assets/streamlit_app.png)](https://youtu.be/ep0PhwsFx0A)
+
+### Examples
+Here you can find usage examples of the package and models to synthesize tabular data.
+  - Fast tabular data synthesis on adult census income dataset [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/ydataai/ydata-synthetic/blob/master/examples/regular/models/Fast_Adult_Census_Income_Data.ipynb)
+  - Tabular synthetic data generation with CTGAN on adult census income dataset [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/ydataai/ydata-synthetic/blob/master/examples/regular/models/CTGAN_Adult_Census_Income_Data.ipynb)
+  - Time Series synthetic data generation with TimeGAN on stock dataset [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/ydataai/ydata-synthetic/blob/master/examples/timeseries/TimeGAN_Synthetic_stock_data.ipynb)
+  - Time Series synthetic data generation with DoppelGANger on FCC MBA dataset [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/ydataai/ydata-synthetic/blob/master/examples/timeseries/DoppelGANger_FCC_MBA_Dataset.ipynb)
+  - More examples are continuously added and can be found in `/examples` directory.
+
+### Datasets for you to experiment
+Here are some example datasets for you to try with the synthesizers:
+#### Tabular datasets
+- [Adult Census Income](https://www.kaggle.com/datasets/uciml/adult-census-income)
+- [Credit card fraud](https://www.kaggle.com/mlg-ulb/creditcardfraud)
+- [Cardiovascular Disease dataset](https://www.kaggle.com/datasets/sulianova/cardiovascular-disease-dataset)
+
+#### Sequential datasets
+- [Stock data](https://github.com/ydataai/ydata-synthetic/tree/master/data)
+- [FCC MBA data](https://github.com/ydataai/ydata-synthetic/tree/master/data)
+
+## Project Resources
+
+In this repository you can find the several GAN architectures that are used to create synthesizers:
+
+### Tabular data
+  - [GAN](https://arxiv.org/abs/1406.2661)
+  - [CGAN (Conditional GAN)](https://arxiv.org/abs/1411.1784)
+  - [WGAN (Wasserstein GAN)](https://arxiv.org/abs/1701.07875)
+  - [WGAN-GP (Wassertein GAN with Gradient Penalty)](https://arxiv.org/abs/1704.00028)
+  - [DRAGAN (On Convergence and stability of GANS)](https://arxiv.org/pdf/1705.07215.pdf)
+  - [Cramer GAN (The Cramer Distance as a Solution to Biased Wasserstein Gradients)](https://arxiv.org/abs/1705.10743)
+  - [CWGAN-GP (Conditional Wassertein GAN with Gradient Penalty)](https://cameronfabbri.github.io/papers/conditionalWGAN.pdf)
+  - [CTGAN (Conditional Tabular GAN)](https://arxiv.org/pdf/1907.00503.pdf)
+  - [Gaussian Mixture](https://towardsdatascience.com/gaussian-mixture-models-explained-6986aaf5a95)
+
+### Sequential data
+  - [TimeGAN](https://papers.nips.cc/paper/2019/file/c9efe5f26cd17ba6216bbe2a7d26d490-Paper.pdf)
+  - [DoppelGANger](https://dl.acm.org/doi/pdf/10.1145/3419394.3423643)
+
+## Contributing
+We are open to collaboration! If you want to start contributing you only need to:
+  1. Search for an issue in which you would like to work. Issues for newcomers are labeled with good first issue.
+  2. Create a PR solving the issue.
+  3. We would review every PRs and either accept or ask for revisions.
+
+## Support
+For support in using this library, please join our Discord server. Our Discord community is very friendly and great about quickly answering questions about the use and development of the library. [Click here to join our Discord community!](https://tiny.ydata.ai/dcai-ydata-synthetic)
+
+## FAQs
+Have a question? Check out the [Frequently Asked Questions](https://ydata.ai/resources/10-most-asked-questions-on-ydata-synthetic) about `ydata-synthetic`. If you feel something is missing, feel free to [book a beary informal chat with us](https://meetings.hubspot.com/fabiana-clemente).
+
+## License
+[MIT License](https://github.com/ydataai/ydata-synthetic/blob/master/LICENSE)
```

### Comparing `ydata-synthetic-1.3.2/README.md` & `ydata-synthetic-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `ydata-synthetic-1.3.2/setup.py` & `ydata-synthetic-1.4.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,23 +38,23 @@
         'Topic :: Scientific/Engineering :: Artificial Intelligence',
         'Topic :: Software Development',
         'Topic :: Software Development :: Libraries :: Python Modules'
       ],
       keywords='data science ydata',
       url='https://github.com/ydataai/ydata-synthetic',
       license="https://github.com/ydataai/ydata-synthetic/blob/master/LICENSE",
-      python_requires=">=3.9, <3.11",
+      python_requires=">=3.9, <3.12",
       packages=find_namespace_packages('src'),
       package_dir={'':'src'},
       include_package_data=True,
       options={"bdist_wheel": {"universal": True}},
       install_requires=requirements,
       extras_require={
           "streamlit": [
               "streamlit==1.29.0",
               "typing-extensions>=3.10.0",
               "streamlit_pandas_profiling==0.1.3",
-              "ydata-profiling==4.6.3",
-              "ydata-sdk>=0.2.1"
+              "ydata-profiling<5",
+              "ydata-sdk>=0.2.1",
           ],
       },
       )
```

### Comparing `ydata-synthetic-1.3.2/src/ydata_synthetic/postprocessing/regular/inverse_preprocesser.py` & `ydata-synthetic-1.4.0/src/ydata_synthetic/postprocessing/regular/inverse_preprocesser.py`

 * *Files identical despite different names*

### Comparing `ydata-synthetic-1.3.2/src/ydata_synthetic/preprocessing/base_processor.py` & `ydata-synthetic-1.4.0/src/ydata_synthetic/preprocessing/base_processor.py`

 * *Files identical despite different names*

### Comparing `ydata-synthetic-1.3.2/src/ydata_synthetic/preprocessing/regular/ctgan_processor.py` & `ydata-synthetic-1.4.0/src/ydata_synthetic/preprocessing/regular/ctgan_processor.py`

 * *Files identical despite different names*

### Comparing `ydata-synthetic-1.3.2/src/ydata_synthetic/preprocessing/regular/processor.py` & `ydata-synthetic-1.4.0/src/ydata_synthetic/preprocessing/regular/processor.py`

 * *Files identical despite different names*

### Comparing `ydata-synthetic-1.3.2/src/ydata_synthetic/preprocessing/timeseries/doppelganger_processor.py` & `ydata-synthetic-1.4.0/src/ydata_synthetic/preprocessing/timeseries/doppelganger_processor.py`

 * *Files identical despite different names*

### Comparing `ydata-synthetic-1.3.2/src/ydata_synthetic/preprocessing/timeseries/stock.py` & `ydata-synthetic-1.4.0/src/ydata_synthetic/preprocessing/timeseries/stock.py`

 * *Files identical despite different names*

### Comparing `ydata-synthetic-1.3.2/src/ydata_synthetic/preprocessing/timeseries/timeseries_processor.py` & `ydata-synthetic-1.4.0/src/ydata_synthetic/preprocessing/timeseries/timeseries_processor.py`

 * *Files identical despite different names*

### Comparing `ydata-synthetic-1.3.2/src/ydata_synthetic/preprocessing/timeseries/utils.py` & `ydata-synthetic-1.4.0/src/ydata_synthetic/preprocessing/timeseries/utils.py`

 * *Files identical despite different names*

### Comparing `ydata-synthetic-1.3.2/src/ydata_synthetic/streamlit_app/About.py` & `ydata-synthetic-1.4.0/src/ydata_synthetic/streamlit_app/About.py`

 * *Files identical despite different names*

### Comparing `ydata-synthetic-1.3.2/src/ydata_synthetic/streamlit_app/pages/1_Train_a_synthesizer.py` & `ydata-synthetic-1.4.0/src/ydata_synthetic/streamlit_app/pages/1_Train_a_synthesizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,28 @@
 from typing import Union
 import os
 import json
+import logging
+
 import streamlit as st
 
 from ydata.sdk.synthesizers import RegularSynthesizer
 from ydata.sdk.common.client import get_client
 
+from ydata_synthetic.utils.logger import SynthesizersLogger
 from ydata_synthetic.synthesizers import ModelParameters, TrainParameters
 from ydata_synthetic.synthesizers.regular.model import Model
 
 from ydata_synthetic.streamlit_app.pages.functions.load_data import upload_file
 from ydata_synthetic.streamlit_app.pages.functions.train import DataType, __CONDITIONAL_MODELS
 from ydata_synthetic.streamlit_app.pages.functions.train import init_synth, advanced_setttings, training_parameters
 
+logger = SynthesizersLogger(name='streamlitSynthesizer.logger')
+logger.setLevel(logging.INFO)
+
 def get_available_models(type: Union[str, DataType]):
 
     dtype = DataType(type)
     if dtype == DataType.TABULAR:
         models_list = [e.value.upper() for e in Model if e.value not in ['cgan', 'cwgangp']] + ['ydata-sdk Synthesizer']
     else:
         st.warning('Time-Series models are not yet supported .')
@@ -110,14 +116,16 @@
                 
 
             with st.expander('**More settings**'):
                 model_path = st.text_input("Saved trained model to path:", value="trained_synth.pkl")
             
             st.subheader("3. Train your synthesizer")
             if st.button('Click here to start the training process', disabled=not valid_token):
+
+                logger.info_def_report(model='fabric')
                 model = RegularSynthesizer()
                 with st.spinner("Please wait while your synthesizer trains..."):
                     dtypes = {}
                     for c in num_cols:
                         dtypes[c] = 'numerical'
                     for c in cat_cols:
                         dtypes[c] = 'categorical'
```

### Comparing `ydata-synthetic-1.3.2/src/ydata_synthetic/streamlit_app/pages/2_Generate_synthetic_data.py` & `ydata-synthetic-1.4.0/src/ydata_synthetic/streamlit_app/pages/2_Generate_synthetic_data.py`

 * *Files identical despite different names*

### Comparing `ydata-synthetic-1.3.2/src/ydata_synthetic/streamlit_app/pages/functions/generate.py` & `ydata-synthetic-1.4.0/src/ydata_synthetic/streamlit_app/pages/functions/generate.py`

 * *Files identical despite different names*

### Comparing `ydata-synthetic-1.3.2/src/ydata_synthetic/streamlit_app/pages/functions/load_data.py` & `ydata-synthetic-1.4.0/src/ydata_synthetic/streamlit_app/pages/functions/load_data.py`

 * *Files identical despite different names*

### Comparing `ydata-synthetic-1.3.2/src/ydata_synthetic/streamlit_app/pages/functions/train.py` & `ydata-synthetic-1.4.0/src/ydata_synthetic/streamlit_app/pages/functions/train.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
     Auxiliary functions for synthetic data training
 """
 from enum import Enum
 import streamlit as st
 
 from ydata_synthetic.synthesizers.regular import RegularSynthesizer
-from ydata_synthetic.synthesizers.timeseries import TimeGAN
+from ydata_synthetic.synthesizers.timeseries.timegan.model import TimeGAN
 from ydata_synthetic.synthesizers import ModelParameters
 
 __MODEL_MAPPING = {'tabular': RegularSynthesizer, 'timeseries': TimeGAN}
 __CONDITIONAL_MODELS = ['CGAN', 'CWGANGP']
 
 class DataType(Enum):
     TABULAR = 'tabular'
```

### Comparing `ydata-synthetic-1.3.2/src/ydata_synthetic/synthesizers/base.py` & `ydata-synthetic-1.4.0/src/ydata_synthetic/synthesizers/base.py`

 * *Files identical despite different names*

### Comparing `ydata-synthetic-1.3.2/src/ydata_synthetic/synthesizers/loss.py` & `ydata-synthetic-1.4.0/src/ydata_synthetic/synthesizers/loss.py`

 * *Files identical despite different names*

### Comparing `ydata-synthetic-1.3.2/src/ydata_synthetic/synthesizers/regular/cgan/model.py` & `ydata-synthetic-1.4.0/src/ydata_synthetic/synthesizers/regular/cgan/model.py`

 * *Files identical despite different names*

### Comparing `ydata-synthetic-1.3.2/src/ydata_synthetic/synthesizers/regular/cramergan/model.py` & `ydata-synthetic-1.4.0/src/ydata_synthetic/synthesizers/regular/cramergan/model.py`

 * *Files identical despite different names*

### Comparing `ydata-synthetic-1.3.2/src/ydata_synthetic/synthesizers/regular/ctgan/model.py` & `ydata-synthetic-1.4.0/src/ydata_synthetic/synthesizers/regular/ctgan/model.py`

 * *Files identical despite different names*

### Comparing `ydata-synthetic-1.3.2/src/ydata_synthetic/synthesizers/regular/ctgan/utils.py` & `ydata-synthetic-1.4.0/src/ydata_synthetic/synthesizers/regular/ctgan/utils.py`

 * *Files identical despite different names*

### Comparing `ydata-synthetic-1.3.2/src/ydata_synthetic/synthesizers/regular/cwgangp/model.py` & `ydata-synthetic-1.4.0/src/ydata_synthetic/synthesizers/regular/cwgangp/model.py`

 * *Files identical despite different names*

### Comparing `ydata-synthetic-1.3.2/src/ydata_synthetic/synthesizers/regular/dragan/model.py` & `ydata-synthetic-1.4.0/src/ydata_synthetic/synthesizers/regular/dragan/model.py`

 * *Files identical despite different names*

### Comparing `ydata-synthetic-1.3.2/src/ydata_synthetic/synthesizers/regular/gmm/model.py` & `ydata-synthetic-1.4.0/src/ydata_synthetic/synthesizers/regular/gmm/model.py`

 * *Files identical despite different names*

### Comparing `ydata-synthetic-1.3.2/src/ydata_synthetic/synthesizers/regular/model.py` & `ydata-synthetic-1.4.0/src/ydata_synthetic/synthesizers/regular/model.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
     Main synthesizer class
 """
 from enum import Enum, unique
+import logging
 
 from joblib import load
 
 from tensorflow import config as tfconfig
 
 from ydata_synthetic.synthesizers.regular.vanillagan.model import VanilllaGAN
 from ydata_synthetic.synthesizers.regular.cgan.model import CGAN
@@ -13,14 +14,18 @@
 from ydata_synthetic.synthesizers.regular.wgangp.model import WGAN_GP
 from ydata_synthetic.synthesizers.regular.cwgangp.model import CWGANGP
 from ydata_synthetic.synthesizers.regular.cramergan.model import CRAMERGAN
 from ydata_synthetic.synthesizers.regular.dragan.model import DRAGAN
 from ydata_synthetic.synthesizers.regular.ctgan.model import CTGAN
 from ydata_synthetic.synthesizers.regular.gmm.model import GMM
 
+from ydata_synthetic.utils.logger import SynthesizersLogger
+
+logger = SynthesizersLogger(name='regularsynthesizer.logger')
+logger.setLevel(logging.INFO)
 
 @unique
 class Model(Enum):
     VANILLA = 'gan'
     CONDITIONAL = 'cgan'
     WASSERTEIN =  'wgan'
     WASSERTEINGP ='wgangp'
@@ -50,14 +55,16 @@
     "Abstraction class "
     def __new__(cls, modelname: str, model_parameters =None, **kwargs):
         model = None
         if Model(modelname) == Model.FAST:
             model=Model(modelname).function(**kwargs)
         else:
             model=Model(modelname).function(model_parameters, **kwargs)
+
+        logger.info_def_report(model=modelname)
         return model
 
     @staticmethod
     def load(path):
         """
         ### Description:
         Loads a saved synthesizer from a pickle.
```

### Comparing `ydata-synthetic-1.3.2/src/ydata_synthetic/synthesizers/regular/vanillagan/model.py` & `ydata-synthetic-1.4.0/src/ydata_synthetic/synthesizers/regular/vanillagan/model.py`

 * *Files identical despite different names*

### Comparing `ydata-synthetic-1.3.2/src/ydata_synthetic/synthesizers/regular/wgan/model.py` & `ydata-synthetic-1.4.0/src/ydata_synthetic/synthesizers/regular/wgan/model.py`

 * *Files identical despite different names*

### Comparing `ydata-synthetic-1.3.2/src/ydata_synthetic/synthesizers/regular/wgangp/model.py` & `ydata-synthetic-1.4.0/src/ydata_synthetic/synthesizers/regular/wgangp/model.py`

 * *Files identical despite different names*

### Comparing `ydata-synthetic-1.3.2/src/ydata_synthetic/synthesizers/saving_keras.py` & `ydata-synthetic-1.4.0/src/ydata_synthetic/synthesizers/saving_keras.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,21 +1,23 @@
+import tensorflow.python.keras as tf_keras
+from keras import __version__
+tf_keras.__version__ = __version__
+
 from tensorflow.keras import Model
-from tensorflow.python.keras.layers import deserialize, serialize
-from tensorflow.python.keras.saving import saving_utils
 
 def unpack(model, training_config, weights):
-    restored_model = deserialize(model)
+    restored_model = tf_keras.layers.deserialize(model)
     if training_config is not None:
-        restored_model.compile(**saving_utils.compile_args_from_training_config(training_config))
+        restored_model.compile(**tf_keras.saving.saving_utils.compile_args_from_training_config(training_config))
     restored_model.set_weights(weights)
     return restored_model
 
 def make_keras_picklable():
     def __reduce__(self):
-        model_metadata = saving_utils.model_metadata(self)
+        model_metadata = tf_keras.saving.saving_utils.model_metadata(self)
         training_config = model_metadata.get("training_config", None)
-        model = serialize(self)
+        model = tf_keras.layers.serialize(self)
         weights = self.get_weights()
         return (unpack, (model, training_config, weights))
 
     cls = Model
     cls.__reduce__=__reduce__
```

### Comparing `ydata-synthetic-1.3.2/src/ydata_synthetic/synthesizers/timeseries/doppelganger/doppelganger.py` & `ydata-synthetic-1.4.0/src/ydata_synthetic/synthesizers/timeseries/doppelganger/doppelganger.py`

 * *Files identical despite different names*

### Comparing `ydata-synthetic-1.3.2/src/ydata_synthetic/synthesizers/timeseries/doppelganger/model.py` & `ydata-synthetic-1.4.0/src/ydata_synthetic/synthesizers/timeseries/doppelganger/model.py`

 * *Files identical despite different names*

### Comparing `ydata-synthetic-1.3.2/src/ydata_synthetic/synthesizers/timeseries/doppelganger/network.py` & `ydata-synthetic-1.4.0/src/ydata_synthetic/synthesizers/timeseries/doppelganger/network.py`

 * *Files identical despite different names*

### Comparing `ydata-synthetic-1.3.2/src/ydata_synthetic/synthesizers/timeseries/model.py` & `ydata-synthetic-1.4.0/src/ydata_synthetic/synthesizers/timeseries/model.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,24 @@
 """
     Main time-series synthesizer class
 """
 from enum import Enum, unique
 import os
+import logging
 from joblib import load
 
 from tensorflow import config as tfconfig
 
 from ydata_synthetic.synthesizers.timeseries.timegan.model import TimeGAN
 from ydata_synthetic.synthesizers.timeseries.doppelganger.model import DoppelGANger
 
+from ydata_synthetic.utils.logger import SynthesizersLogger
+
+logger = SynthesizersLogger(name='timseriesSynthesizer.logger')
+logger.setLevel(logging.INFO)
 
 @unique
 class Model(Enum):
     TIMEGAN = 'timegan'
     DOPPELGANGER = 'doppelganger'
 
     __MAPPING__ = {
@@ -24,14 +29,15 @@
     @property
     def function(self):
         return self.__MAPPING__[self.value]
 
 class TimeSeriesSynthesizer():
     "Abstraction class "
     def __new__(cls, modelname: str, model_parameters=None, **kwargs):
+        logger.info_def_report(model=modelname)
         return Model(modelname).function(model_parameters, **kwargs)
 
     @staticmethod
     def load(path):
         """
         ### Description:
         Loads a saved synthesizer from a pickle.
```

### Comparing `ydata-synthetic-1.3.2/src/ydata_synthetic/synthesizers/timeseries/timegan/model.py` & `ydata-synthetic-1.4.0/src/ydata_synthetic/synthesizers/timeseries/timegan/model.py`

 * *Files identical despite different names*

### Comparing `ydata-synthetic-1.3.2/src/ydata_synthetic/tests/custom_layers/test_gumbel_softmax_activation.py` & `ydata-synthetic-1.4.0/src/ydata_synthetic/tests/custom_layers/test_gumbel_softmax_activation.py`

 * *Files identical despite different names*

### Comparing `ydata-synthetic-1.3.2/src/ydata_synthetic/tests/custom_layers/test_gumbel_softmax_layer.py` & `ydata-synthetic-1.4.0/src/ydata_synthetic/tests/custom_layers/test_gumbel_softmax_layer.py`

 * *Files identical despite different names*

### Comparing `ydata-synthetic-1.3.2/src/ydata_synthetic/tests/preprocessing/test_regular_data_processor.py` & `ydata-synthetic-1.4.0/src/ydata_synthetic/tests/preprocessing/test_regular_data_processor.py`

 * *Files identical despite different names*

### Comparing `ydata-synthetic-1.3.2/src/ydata_synthetic/utils/cache.py` & `ydata-synthetic-1.4.0/src/ydata_synthetic/utils/cache.py`

 * *Files identical despite different names*

### Comparing `ydata-synthetic-1.3.2/src/ydata_synthetic/utils/gumbel_softmax.py` & `ydata-synthetic-1.4.0/src/ydata_synthetic/utils/gumbel_softmax.py`

 * *Files identical despite different names*

### Comparing `ydata-synthetic-1.3.2/src/ydata_synthetic/utils/misc/colormaps.py` & `ydata-synthetic-1.4.0/src/ydata_synthetic/utils/misc/colormaps.py`

 * *Files identical despite different names*

### Comparing `ydata-synthetic-1.3.2/src/ydata_synthetic.egg-info/PKG-INFO` & `ydata-synthetic-1.4.0/src/ydata_synthetic.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,158 +1,16 @@
 Metadata-Version: 2.1
 Name: ydata-synthetic
-Version: 1.3.2
+Version: 1.4.0
 Summary: Synthetic data generation methods with different synthetization methods.
 Home-page: https://github.com/ydataai/ydata-synthetic
 Author: YData
 Author-email: community@ydata.ai
 License: https://github.com/ydataai/ydata-synthetic/blob/master/LICENSE
-Description: ![](https://img.shields.io/github/workflow/status/ydataai/ydata-synthetic/prerelease)
-        ![](https://img.shields.io/pypi/status/ydata-synthetic)
-        [![](https://pepy.tech/badge/ydata-synthetic)](https://pypi.org/project/ydata-synthetic/)
-        ![](https://img.shields.io/badge/python-3.9%20%7C%203.10-blue)
-        [![](https://img.shields.io/pypi/v/ydata-synthetic)](https://pypi.org/project/ydata-synthetic/)
-        ![](https://img.shields.io/github/license/ydataai/ydata-synthetic)
-        
-        <p align="center"><img width="300" src="https://assets.ydata.ai/oss/ydata-synthetic_black.png" alt="YData Synthetic Logo"></p>
-        
-        Join us on [![Discord](https://img.shields.io/badge/Discord-7289DA?style=for-the-badge&logo=discord&logoColor=white)](https://tiny.ydata.ai/dcai-ydata-synthetic)
-        
-        # YData Synthetic
-        A package to generate synthetic tabular and time-series data leveraging the state of the art generative models.
-        
-        ## 🎊 The exciting features:
-        > These are must try features when it comes to synthetic data generation:
-          > - A new streamlit app that delivers the synthetic data generation experience with a UI interface. A low code experience for the quick generation of synthetic data
-          > - A new fast synthetic data generation model based on Gaussian Mixture. So you can quickstart in the world of synthetic data generation without the need for a GPU.
-          > - A conditional architecture for tabular data: CTGAN, which will make the process of synthetic data generation easier and with higher quality!
-          
-        ## Synthetic data
-        ### What is synthetic data?
-        Synthetic data is artificially generated data that is not collected from real world events. It replicates the statistical components of real data without containing any identifiable information, ensuring individuals' privacy.
-        
-        ### Why Synthetic Data?
-        Synthetic data can be used for many applications:
-          - Privacy compliance for data-sharing and Machine Learning development
-          - Remove bias
-          - Balance datasets
-          - Augment datasets
-        
-        > **Looking for an end-to-end solution to Synthetic Data Generation?**<br>
-        > [YData Fabric](https://ydata.ai/products/synthetic_data) enables the generation of high-quality datasets within a full UI experience, from data preparation to synthetic data generation and evaluation.<br>
-        > Check out the [Community Version](https://ydata.ai/ydata-fabric-free-trial).
-        
-        
-        # ydata-synthetic
-        This repository contains material related with architectures and models for synthetic data, from Generative Adversarial Networks (GANs) to Gaussian Mixtures.
-        The repo includes a full ecosystem for synthetic data generation, that includes different models for the generation of synthetic structure data and time-series.
-        All the Deep Learning models are implemented leveraging Tensorflow 2.0.
-        Several example Jupyter Notebooks and Python scripts are included, to show how to use the different architectures.
-        
-        Are you ready to learn more about synthetic data and the bext-practices for synthetic data generation?
-        
-        ## Quickstart
-        The source code is currently hosted on GitHub at: https://github.com/ydataai/ydata-synthetic
-        
-        Binary installers for the latest released version are available at the [Python Package Index (PyPI).](https://pypi.org/project/ydata-synthetic/)
-        ```commandline
-        pip install ydata-synthetic
-        ```
-        
-        ### The UI guide for synthetic data generation
-        
-        YData synthetic has now a UI interface to guide you through the steps and inputs to generate structure tabular data.
-        The streamlit app is available form *v1.0.0* onwards, and supports the following flows:
-        - Train a synthesizer model
-        - Generate & profile synthetic data samples
-        
-        #### Installation
-        
-        ```commandline
-        pip install ydata-synthetic[streamlit]
-        ```
-        #### Quickstart
-        Use the code snippet below in a python file (Jupyter Notebooks are not supported):
-        ```python
-        from ydata_synthetic import streamlit_app
-        
-        streamlit_app.run()
-        ```
-        
-        Or use the file streamlit_app.py that can be found in the [examples folder](https://github.com/ydataai/ydata-synthetic/tree/master/examples/streamlit_app.py).
-        
-        ```commandline
-        python -m streamlit_app
-        ```
-        
-        The below models are supported:
-          - CGAN
-          - WGAN
-          - WGANGP
-          - DRAGAN
-          - CRAMER
-          - CTGAN
-        
-        [![Watch the video](assets/streamlit_app.png)](https://youtu.be/ep0PhwsFx0A)
-        
-        ### Examples
-        Here you can find usage examples of the package and models to synthesize tabular data.
-          - Fast tabular data synthesis on adult census income dataset [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/ydataai/ydata-synthetic/blob/master/examples/regular/models/Fast_Adult_Census_Income_Data.ipynb)
-          - Tabular synthetic data generation with CTGAN on adult census income dataset [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/ydataai/ydata-synthetic/blob/master/examples/regular/models/CTGAN_Adult_Census_Income_Data.ipynb)
-          - Time Series synthetic data generation with TimeGAN on stock dataset [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/ydataai/ydata-synthetic/blob/master/examples/timeseries/TimeGAN_Synthetic_stock_data.ipynb)
-          - Time Series synthetic data generation with DoppelGANger on FCC MBA dataset [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/ydataai/ydata-synthetic/blob/master/examples/timeseries/DoppelGANger_FCC_MBA_Dataset.ipynb)
-          - More examples are continuously added and can be found in `/examples` directory.
-        
-        ### Datasets for you to experiment
-        Here are some example datasets for you to try with the synthesizers:
-        #### Tabular datasets
-        - [Adult Census Income](https://www.kaggle.com/datasets/uciml/adult-census-income)
-        - [Credit card fraud](https://www.kaggle.com/mlg-ulb/creditcardfraud)
-        - [Cardiovascular Disease dataset](https://www.kaggle.com/datasets/sulianova/cardiovascular-disease-dataset)
-        
-        #### Sequential datasets
-        - [Stock data](https://github.com/ydataai/ydata-synthetic/tree/master/data)
-        - [FCC MBA data](https://github.com/ydataai/ydata-synthetic/tree/master/data)
-        
-        ## Project Resources
-        
-        In this repository you can find the several GAN architectures that are used to create synthesizers:
-        
-        ### Tabular data
-          - [GAN](https://arxiv.org/abs/1406.2661)
-          - [CGAN (Conditional GAN)](https://arxiv.org/abs/1411.1784)
-          - [WGAN (Wasserstein GAN)](https://arxiv.org/abs/1701.07875)
-          - [WGAN-GP (Wassertein GAN with Gradient Penalty)](https://arxiv.org/abs/1704.00028)
-          - [DRAGAN (On Convergence and stability of GANS)](https://arxiv.org/pdf/1705.07215.pdf)
-          - [Cramer GAN (The Cramer Distance as a Solution to Biased Wasserstein Gradients)](https://arxiv.org/abs/1705.10743)
-          - [CWGAN-GP (Conditional Wassertein GAN with Gradient Penalty)](https://cameronfabbri.github.io/papers/conditionalWGAN.pdf)
-          - [CTGAN (Conditional Tabular GAN)](https://arxiv.org/pdf/1907.00503.pdf)
-          - [Gaussian Mixture](https://towardsdatascience.com/gaussian-mixture-models-explained-6986aaf5a95)
-        
-        ### Sequential data
-          - [TimeGAN](https://papers.nips.cc/paper/2019/file/c9efe5f26cd17ba6216bbe2a7d26d490-Paper.pdf)
-          - [DoppelGANger](https://dl.acm.org/doi/pdf/10.1145/3419394.3423643)
-        
-        ## Contributing
-        We are open to collaboration! If you want to start contributing you only need to:
-          1. Search for an issue in which you would like to work. Issues for newcomers are labeled with good first issue.
-          2. Create a PR solving the issue.
-          3. We would review every PRs and either accept or ask for revisions.
-        
-        ## Support
-        For support in using this library, please join our Discord server. Our Discord community is very friendly and great about quickly answering questions about the use and development of the library. [Click here to join our Discord community!](https://tiny.ydata.ai/dcai-ydata-synthetic)
-        
-        ## FAQs
-        Have a question? Check out the [Frequently Asked Questions](https://ydata.ai/resources/10-most-asked-questions-on-ydata-synthetic) about `ydata-synthetic`. If you feel something is missing, feel free to [book a beary informal chat with us](https://meetings.hubspot.com/fabiana-clemente).
-        
-        ## License
-        [MIT License](https://github.com/ydataai/ydata-synthetic/blob/master/LICENSE)
-        
 Keywords: data science ydata
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: Intended Audience :: Healthcare Industry
 Classifier: Intended Audience :: Science/Research
@@ -162,10 +20,152 @@
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.9, <3.11
+Requires-Python: >=3.9, <3.12
 Description-Content-Type: text/markdown
 Provides-Extra: streamlit
+License-File: LICENSE
+
+![](https://img.shields.io/github/workflow/status/ydataai/ydata-synthetic/prerelease)
+![](https://img.shields.io/pypi/status/ydata-synthetic)
+[![](https://pepy.tech/badge/ydata-synthetic)](https://pypi.org/project/ydata-synthetic/)
+![](https://img.shields.io/badge/python-3.9%20%7C%203.10-blue)
+[![](https://img.shields.io/pypi/v/ydata-synthetic)](https://pypi.org/project/ydata-synthetic/)
+![](https://img.shields.io/github/license/ydataai/ydata-synthetic)
+
+<p align="center"><img width="300" src="https://assets.ydata.ai/oss/ydata-synthetic_black.png" alt="YData Synthetic Logo"></p>
+
+Join us on [![Discord](https://img.shields.io/badge/Discord-7289DA?style=for-the-badge&logo=discord&logoColor=white)](https://tiny.ydata.ai/dcai-ydata-synthetic)
+
+# YData Synthetic
+A package to generate synthetic tabular and time-series data leveraging the state of the art generative models.
+
+## 🎊 The exciting features:
+> These are must try features when it comes to synthetic data generation:
+  > - A new streamlit app that delivers the synthetic data generation experience with a UI interface. A low code experience for the quick generation of synthetic data
+  > - A new fast synthetic data generation model based on Gaussian Mixture. So you can quickstart in the world of synthetic data generation without the need for a GPU.
+  > - A conditional architecture for tabular data: CTGAN, which will make the process of synthetic data generation easier and with higher quality!
+  
+## Synthetic data
+### What is synthetic data?
+Synthetic data is artificially generated data that is not collected from real world events. It replicates the statistical components of real data without containing any identifiable information, ensuring individuals' privacy.
+
+### Why Synthetic Data?
+Synthetic data can be used for many applications:
+  - Privacy compliance for data-sharing and Machine Learning development
+  - Remove bias
+  - Balance datasets
+  - Augment datasets
+
+> **Looking for an end-to-end solution to Synthetic Data Generation?**<br>
+> [YData Fabric](https://ydata.ai/products/synthetic_data) enables the generation of high-quality datasets within a full UI experience, from data preparation to synthetic data generation and evaluation.<br>
+> Check out the [Community Version](https://ydata.ai/ydata-fabric-free-trial).
+
+
+# ydata-synthetic
+This repository contains material related with architectures and models for synthetic data, from Generative Adversarial Networks (GANs) to Gaussian Mixtures.
+The repo includes a full ecosystem for synthetic data generation, that includes different models for the generation of synthetic structure data and time-series.
+All the Deep Learning models are implemented leveraging Tensorflow 2.0.
+Several example Jupyter Notebooks and Python scripts are included, to show how to use the different architectures.
+
+Are you ready to learn more about synthetic data and the bext-practices for synthetic data generation?
+
+## Quickstart
+The source code is currently hosted on GitHub at: https://github.com/ydataai/ydata-synthetic
+
+Binary installers for the latest released version are available at the [Python Package Index (PyPI).](https://pypi.org/project/ydata-synthetic/)
+```commandline
+pip install ydata-synthetic
+```
+
+### The UI guide for synthetic data generation
+
+YData synthetic has now a UI interface to guide you through the steps and inputs to generate structure tabular data.
+The streamlit app is available form *v1.0.0* onwards, and supports the following flows:
+- Train a synthesizer model
+- Generate & profile synthetic data samples
+
+#### Installation
+
+```commandline
+pip install ydata-synthetic[streamlit]
+```
+#### Quickstart
+Use the code snippet below in a python file (Jupyter Notebooks are not supported):
+```python
+from ydata_synthetic import streamlit_app
+
+streamlit_app.run()
+```
+
+Or use the file streamlit_app.py that can be found in the [examples folder](https://github.com/ydataai/ydata-synthetic/tree/master/examples/streamlit_app.py).
+
+```commandline
+python -m streamlit_app
+```
+
+The below models are supported:
+  - CGAN
+  - WGAN
+  - WGANGP
+  - DRAGAN
+  - CRAMER
+  - CTGAN
+
+[![Watch the video](assets/streamlit_app.png)](https://youtu.be/ep0PhwsFx0A)
+
+### Examples
+Here you can find usage examples of the package and models to synthesize tabular data.
+  - Fast tabular data synthesis on adult census income dataset [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/ydataai/ydata-synthetic/blob/master/examples/regular/models/Fast_Adult_Census_Income_Data.ipynb)
+  - Tabular synthetic data generation with CTGAN on adult census income dataset [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/ydataai/ydata-synthetic/blob/master/examples/regular/models/CTGAN_Adult_Census_Income_Data.ipynb)
+  - Time Series synthetic data generation with TimeGAN on stock dataset [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/ydataai/ydata-synthetic/blob/master/examples/timeseries/TimeGAN_Synthetic_stock_data.ipynb)
+  - Time Series synthetic data generation with DoppelGANger on FCC MBA dataset [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/ydataai/ydata-synthetic/blob/master/examples/timeseries/DoppelGANger_FCC_MBA_Dataset.ipynb)
+  - More examples are continuously added and can be found in `/examples` directory.
+
+### Datasets for you to experiment
+Here are some example datasets for you to try with the synthesizers:
+#### Tabular datasets
+- [Adult Census Income](https://www.kaggle.com/datasets/uciml/adult-census-income)
+- [Credit card fraud](https://www.kaggle.com/mlg-ulb/creditcardfraud)
+- [Cardiovascular Disease dataset](https://www.kaggle.com/datasets/sulianova/cardiovascular-disease-dataset)
+
+#### Sequential datasets
+- [Stock data](https://github.com/ydataai/ydata-synthetic/tree/master/data)
+- [FCC MBA data](https://github.com/ydataai/ydata-synthetic/tree/master/data)
+
+## Project Resources
+
+In this repository you can find the several GAN architectures that are used to create synthesizers:
+
+### Tabular data
+  - [GAN](https://arxiv.org/abs/1406.2661)
+  - [CGAN (Conditional GAN)](https://arxiv.org/abs/1411.1784)
+  - [WGAN (Wasserstein GAN)](https://arxiv.org/abs/1701.07875)
+  - [WGAN-GP (Wassertein GAN with Gradient Penalty)](https://arxiv.org/abs/1704.00028)
+  - [DRAGAN (On Convergence and stability of GANS)](https://arxiv.org/pdf/1705.07215.pdf)
+  - [Cramer GAN (The Cramer Distance as a Solution to Biased Wasserstein Gradients)](https://arxiv.org/abs/1705.10743)
+  - [CWGAN-GP (Conditional Wassertein GAN with Gradient Penalty)](https://cameronfabbri.github.io/papers/conditionalWGAN.pdf)
+  - [CTGAN (Conditional Tabular GAN)](https://arxiv.org/pdf/1907.00503.pdf)
+  - [Gaussian Mixture](https://towardsdatascience.com/gaussian-mixture-models-explained-6986aaf5a95)
+
+### Sequential data
+  - [TimeGAN](https://papers.nips.cc/paper/2019/file/c9efe5f26cd17ba6216bbe2a7d26d490-Paper.pdf)
+  - [DoppelGANger](https://dl.acm.org/doi/pdf/10.1145/3419394.3423643)
+
+## Contributing
+We are open to collaboration! If you want to start contributing you only need to:
+  1. Search for an issue in which you would like to work. Issues for newcomers are labeled with good first issue.
+  2. Create a PR solving the issue.
+  3. We would review every PRs and either accept or ask for revisions.
+
+## Support
+For support in using this library, please join our Discord server. Our Discord community is very friendly and great about quickly answering questions about the use and development of the library. [Click here to join our Discord community!](https://tiny.ydata.ai/dcai-ydata-synthetic)
+
+## FAQs
+Have a question? Check out the [Frequently Asked Questions](https://ydata.ai/resources/10-most-asked-questions-on-ydata-synthetic) about `ydata-synthetic`. If you feel something is missing, feel free to [book a beary informal chat with us](https://meetings.hubspot.com/fabiana-clemente).
+
+## License
+[MIT License](https://github.com/ydataai/ydata-synthetic/blob/master/LICENSE)
```

### Comparing `ydata-synthetic-1.3.2/src/ydata_synthetic.egg-info/SOURCES.txt` & `ydata-synthetic-1.4.0/src/ydata_synthetic.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -68,8 +68,10 @@
 src/ydata_synthetic/synthesizers/timeseries/timegan/model.py
 src/ydata_synthetic/tests/custom_layers/test_gumbel_softmax_activation.py
 src/ydata_synthetic/tests/custom_layers/test_gumbel_softmax_layer.py
 src/ydata_synthetic/tests/preprocessing/test_regular_data_processor.py
 src/ydata_synthetic/utils/__init__.py
 src/ydata_synthetic/utils/cache.py
 src/ydata_synthetic/utils/gumbel_softmax.py
+src/ydata_synthetic/utils/logger.py
+src/ydata_synthetic/utils/utils.py
 src/ydata_synthetic/utils/misc/colormaps.py
```

