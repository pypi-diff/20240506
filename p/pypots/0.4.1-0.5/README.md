# Comparing `tmp/pypots-0.4.1.tar.gz` & `tmp/pypots-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypots-0.4.1.tar", last modified: Wed Apr 17 16:06:57 2024, max compression
+gzip compressed data, was "pypots-0.5.tar", last modified: Mon May  6 14:24:30 2024, max compression
```

## Comparing `pypots-0.4.1.tar` & `pypots-0.5.tar`

### file list

```diff
@@ -1,282 +1,313 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:06:57.847941 pypots-0.4.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-04-17 16:04:57.000000 pypots-0.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-17 16:04:57.000000 pypots-0.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    27877 2024-04-17 16:06:57.847941 pypots-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    26062 2024-04-17 16:04:57.000000 pypots-0.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:06:57.815940 pypots-0.4.1/pypots/
--rw-r--r--   0 runner    (1001) docker     (127)      784 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22426 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:06:57.815940 pypots-0.4.1/pypots/classification/
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/classification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17970 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/classification/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:06:57.815940 pypots-0.4.1/pypots/classification/brits/
--rw-r--r--   0 runner    (1001) docker     (127)      546 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/classification/brits/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3164 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/classification/brits/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     2070 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/classification/brits/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     9871 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/classification/brits/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:06:57.815940 pypots-0.4.1/pypots/classification/grud/
--rw-r--r--   0 runner    (1001) docker     (127)      485 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/classification/grud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/classification/grud/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     5340 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/classification/grud/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     8923 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/classification/grud/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:06:57.815940 pypots-0.4.1/pypots/classification/raindrop/
--rw-r--r--   0 runner    (1001) docker     (127)      446 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/classification/raindrop/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3708 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/classification/raindrop/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     2011 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/classification/raindrop/data.py
--rw-r--r--   0 runner    (1001) docker     (127)    10093 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/classification/raindrop/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:06:57.819940 pypots-0.4.1/pypots/cli/
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2552 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/cli/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     6268 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/cli/dev.py
--rw-r--r--   0 runner    (1001) docker     (127)     7915 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/cli/doc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4534 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/cli/env.py
--rw-r--r--   0 runner    (1001) docker     (127)      969 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/cli/pypots_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     9149 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/cli/tuning.py
--rw-r--r--   0 runner    (1001) docker     (127)      658 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/cli/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:06:57.819940 pypots-0.4.1/pypots/clustering/
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/clustering/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17064 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/clustering/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:06:57.819940 pypots-0.4.1/pypots/clustering/crli/
--rw-r--r--   0 runner    (1001) docker     (127)      446 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/clustering/crli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3430 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/clustering/crli/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     2237 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/clustering/crli/data.py
--rw-r--r--   0 runner    (1001) docker     (127)    18627 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/clustering/crli/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:06:57.819940 pypots-0.4.1/pypots/clustering/vader/
--rw-r--r--   0 runner    (1001) docker     (127)      615 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/clustering/vader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5289 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/clustering/vader/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     2239 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/clustering/vader/data.py
--rw-r--r--   0 runner    (1001) docker     (127)    20790 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/clustering/vader/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:06:57.819940 pypots-0.4.1/pypots/data/
--rw-r--r--   0 runner    (1001) docker     (127)      998 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12298 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/data/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      459 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/data/checking.py
--rw-r--r--   0 runner    (1001) docker     (127)    13939 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/data/generating.py
--rw-r--r--   0 runner    (1001) docker     (127)     1822 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/data/load_preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (127)     2107 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/data/load_specific_datasets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:06:57.819940 pypots-0.4.1/pypots/data/saving/
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/data/saving/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4518 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/data/saving/h5.py
--rw-r--r--   0 runner    (1001) docker     (127)     1434 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/data/saving/pickle.py
--rw-r--r--   0 runner    (1001) docker     (127)     7426 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/data/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:06:57.823940 pypots-0.4.1/pypots/forecasting/
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/forecasting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17631 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/forecasting/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:06:57.823940 pypots-0.4.1/pypots/forecasting/bttf/
--rw-r--r--   0 runner    (1001) docker     (127)      449 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/forecasting/bttf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9305 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/forecasting/bttf/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     4963 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/forecasting/bttf/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6620 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/forecasting/bttf/submodules.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:06:57.823940 pypots-0.4.1/pypots/imputation/
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/imputation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:06:57.823940 pypots-0.4.1/pypots/imputation/autoformer/
--rw-r--r--   0 runner    (1001) docker     (127)      604 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/imputation/autoformer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3478 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/imputation/autoformer/core.py
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/imputation/autoformer/data.py
--rw-r--r--   0 runner    (1001) docker     (127)    11416 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/imputation/autoformer/model.py
--rw-r--r--   0 runner    (1001) docker     (127)    17827 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/imputation/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:06:57.823940 pypots-0.4.1/pypots/imputation/brits/
--rw-r--r--   0 runner    (1001) docker     (127)      542 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/imputation/brits/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2267 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/imputation/brits/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     6836 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/imputation/brits/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     9725 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/imputation/brits/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:06:57.823940 pypots-0.4.1/pypots/imputation/crossformer/
--rw-r--r--   0 runner    (1001) docker     (127)      450 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/imputation/crossformer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4104 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/imputation/crossformer/core.py
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/imputation/crossformer/data.py
--rw-r--r--   0 runner    (1001) docker     (127)    11476 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/imputation/crossformer/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:06:57.823940 pypots-0.4.1/pypots/imputation/csdi/
--rw-r--r--   0 runner    (1001) docker     (127)      508 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/imputation/csdi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2994 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/imputation/csdi/core.py
--rw-r--r--   0 runner    (1001) docker     (127)    10673 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/imputation/csdi/data.py
--rw-r--r--   0 runner    (1001) docker     (127)    17276 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/imputation/csdi/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:06:57.827940 pypots-0.4.1/pypots/imputation/dlinear/
--rw-r--r--   0 runner    (1001) docker     (127)      458 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/imputation/dlinear/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3533 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/imputation/dlinear/core.py
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/imputation/dlinear/data.py
--rw-r--r--   0 runner    (1001) docker     (127)    10933 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/imputation/dlinear/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:06:57.827940 pypots-0.4.1/pypots/imputation/etsformer/
--rw-r--r--   0 runner    (1001) docker     (127)      446 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/imputation/etsformer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3588 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/imputation/etsformer/core.py
--rw-r--r--   0 runner    (1001) docker     (127)      578 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/imputation/etsformer/data.py
--rw-r--r--   0 runner    (1001) docker     (127)    11171 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/imputation/etsformer/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:06:57.827940 pypots-0.4.1/pypots/imputation/fedformer/
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/imputation/fedformer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3010 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/imputation/fedformer/core.py
--rw-r--r--   0 runner    (1001) docker     (127)      578 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/imputation/fedformer/data.py
--rw-r--r--   0 runner    (1001) docker     (127)    11853 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/imputation/fedformer/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:06:57.827940 pypots-0.4.1/pypots/imputation/gpvae/
--rw-r--r--   0 runner    (1001) docker     (127)      518 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/imputation/gpvae/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2577 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/imputation/gpvae/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     5147 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/imputation/gpvae/data.py
--rw-r--r--   0 runner    (1001) docker     (127)    18004 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/imputation/gpvae/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:06:57.827940 pypots-0.4.1/pypots/imputation/informer/
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/imputation/informer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3514 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/imputation/informer/core.py
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/imputation/informer/data.py
--rw-r--r--   0 runner    (1001) docker     (127)    11232 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/imputation/informer/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:06:57.827940 pypots-0.4.1/pypots/imputation/locf/
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/imputation/locf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6908 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/imputation/locf/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     6225 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/imputation/locf/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:06:57.827940 pypots-0.4.1/pypots/imputation/mean/
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/imputation/mean/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4817 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/imputation/mean/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:06:57.827940 pypots-0.4.1/pypots/imputation/median/
--rw-r--r--   0 runner    (1001) docker     (127)      210 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/imputation/median/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4847 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/imputation/median/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:06:57.831941 pypots-0.4.1/pypots/imputation/mrnn/
--rw-r--r--   0 runner    (1001) docker     (127)      490 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/imputation/mrnn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1276 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/imputation/mrnn/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     6834 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/imputation/mrnn/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     9708 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/imputation/mrnn/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:06:57.831941 pypots-0.4.1/pypots/imputation/patchtst/
--rw-r--r--   0 runner    (1001) docker     (127)      440 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/imputation/patchtst/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3051 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/imputation/patchtst/core.py
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/imputation/patchtst/data.py
--rw-r--r--   0 runner    (1001) docker     (127)    12391 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/imputation/patchtst/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:06:57.831941 pypots-0.4.1/pypots/imputation/saits/
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/imputation/saits/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4103 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/imputation/saits/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     6318 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/imputation/saits/data.py
--rw-r--r--   0 runner    (1001) docker     (127)    14631 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/imputation/saits/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:06:57.831941 pypots-0.4.1/pypots/imputation/timesnet/
--rw-r--r--   0 runner    (1001) docker     (127)      450 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/imputation/timesnet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2368 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/imputation/timesnet/core.py
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/imputation/timesnet/data.py
--rw-r--r--   0 runner    (1001) docker     (127)    11290 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/imputation/timesnet/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:06:57.831941 pypots-0.4.1/pypots/imputation/transformer/
--rw-r--r--   0 runner    (1001) docker     (127)      778 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/imputation/transformer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3083 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/imputation/transformer/core.py
--rw-r--r--   0 runner    (1001) docker     (127)      547 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/imputation/transformer/data.py
--rw-r--r--   0 runner    (1001) docker     (127)    11372 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/imputation/transformer/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:06:57.831941 pypots-0.4.1/pypots/imputation/usgan/
--rw-r--r--   0 runner    (1001) docker     (127)      489 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/imputation/usgan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2000 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/imputation/usgan/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     2107 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/imputation/usgan/data.py
--rw-r--r--   0 runner    (1001) docker     (127)    17737 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/imputation/usgan/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:06:57.831941 pypots-0.4.1/pypots/nn/
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/nn/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:06:57.835940 pypots-0.4.1/pypots/nn/functional/
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/nn/functional/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3251 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/nn/functional/normalization.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:06:57.835940 pypots-0.4.1/pypots/nn/modules/
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/nn/modules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:06:57.835940 pypots-0.4.1/pypots/nn/modules/autoformer/
--rw-r--r--   0 runner    (1001) docker     (127)      985 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/nn/modules/autoformer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1245 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/nn/modules/autoformer/auto_encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)    11263 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/nn/modules/autoformer/layers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:06:57.835940 pypots-0.4.1/pypots/nn/modules/brits/
--rw-r--r--   0 runner    (1001) docker     (127)      628 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/nn/modules/brits/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8525 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/nn/modules/brits/backbone.py
--rw-r--r--   0 runner    (1001) docker     (127)     2257 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/nn/modules/brits/layers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:06:57.835940 pypots-0.4.1/pypots/nn/modules/crli/
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/nn/modules/crli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/nn/modules/crli/backbone.py
--rw-r--r--   0 runner    (1001) docker     (127)     9275 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/nn/modules/crli/layers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:06:57.835940 pypots-0.4.1/pypots/nn/modules/crossformer/
--rw-r--r--   0 runner    (1001) docker     (127)      646 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/nn/modules/crossformer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/nn/modules/crossformer/auto_encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     6718 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/nn/modules/crossformer/layers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:06:57.835940 pypots-0.4.1/pypots/nn/modules/csdi/
--rw-r--r--   0 runner    (1001) docker     (127)      650 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/nn/modules/csdi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7477 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/nn/modules/csdi/backbone.py
--rw-r--r--   0 runner    (1001) docker     (127)     6521 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/nn/modules/csdi/layers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:06:57.835940 pypots-0.4.1/pypots/nn/modules/dlinear/
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/nn/modules/dlinear/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3127 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/nn/modules/dlinear/backbone.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:06:57.835940 pypots-0.4.1/pypots/nn/modules/etsformer/
--rw-r--r--   0 runner    (1001) docker     (127)      630 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/nn/modules/etsformer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/nn/modules/etsformer/auto_encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)    10413 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/nn/modules/etsformer/layers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:06:57.835940 pypots-0.4.1/pypots/nn/modules/fedformer/
--rw-r--r--   0 runner    (1001) docker     (127)      822 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/nn/modules/fedformer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4524 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/nn/modules/fedformer/autoencoder.py
--rw-r--r--   0 runner    (1001) docker     (127)    31276 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/nn/modules/fedformer/layers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:06:57.839940 pypots-0.4.1/pypots/nn/modules/gpvae/
--rw-r--r--   0 runner    (1001) docker     (127)      543 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/nn/modules/gpvae/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6158 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/nn/modules/gpvae/backbone.py
--rw-r--r--   0 runner    (1001) docker     (127)     8580 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/nn/modules/gpvae/layers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:06:57.839940 pypots-0.4.1/pypots/nn/modules/grud/
--rw-r--r--   0 runner    (1001) docker     (127)      433 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/nn/modules/grud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2188 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/nn/modules/grud/backbone.py
--rw-r--r--   0 runner    (1001) docker     (127)     2402 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/nn/modules/grud/layers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:06:57.839940 pypots-0.4.1/pypots/nn/modules/informer/
--rw-r--r--   0 runner    (1001) docker     (127)      802 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/nn/modules/informer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1742 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/nn/modules/informer/auto_encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     7489 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/nn/modules/informer/layers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:06:57.839940 pypots-0.4.1/pypots/nn/modules/mrnn/
--rw-r--r--   0 runner    (1001) docker     (127)      542 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/nn/modules/mrnn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2914 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/nn/modules/mrnn/backbone.py
--rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/nn/modules/mrnn/layers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:06:57.839940 pypots-0.4.1/pypots/nn/modules/patchtst/
--rw-r--r--   0 runner    (1001) docker     (127)      610 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/nn/modules/patchtst/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/nn/modules/patchtst/auto_encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     4684 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/nn/modules/patchtst/layers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:06:57.839940 pypots-0.4.1/pypots/nn/modules/raindrop/
--rw-r--r--   0 runner    (1001) docker     (127)      431 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/nn/modules/raindrop/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7879 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/nn/modules/raindrop/backbone.py
--rw-r--r--   0 runner    (1001) docker     (127)    11622 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/nn/modules/raindrop/layers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:06:57.839940 pypots-0.4.1/pypots/nn/modules/saits/
--rw-r--r--   0 runner    (1001) docker     (127)      443 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/nn/modules/saits/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4883 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/nn/modules/saits/backbone.py
--rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/nn/modules/saits/loss.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:06:57.839940 pypots-0.4.1/pypots/nn/modules/timesnet/
--rw-r--r--   0 runner    (1001) docker     (127)      530 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/nn/modules/timesnet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      890 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/nn/modules/timesnet/backbone.py
--rw-r--r--   0 runner    (1001) docker     (127)     3509 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/nn/modules/timesnet/layers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:06:57.843941 pypots-0.4.1/pypots/nn/modules/transformer/
--rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/nn/modules/transformer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6242 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/nn/modules/transformer/attention.py
--rw-r--r--   0 runner    (1001) docker     (127)     6065 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/nn/modules/transformer/auto_encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     5728 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/nn/modules/transformer/embedding.py
--rw-r--r--   0 runner    (1001) docker     (127)     6389 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/nn/modules/transformer/layers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:06:57.843941 pypots-0.4.1/pypots/nn/modules/usgan/
--rw-r--r--   0 runner    (1001) docker     (127)      513 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/nn/modules/usgan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2913 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/nn/modules/usgan/backbone.py
--rw-r--r--   0 runner    (1001) docker     (127)     1994 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/nn/modules/usgan/layers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:06:57.843941 pypots-0.4.1/pypots/nn/modules/vader/
--rw-r--r--   0 runner    (1001) docker     (127)      737 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/nn/modules/vader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4898 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/nn/modules/vader/backbone.py
--rw-r--r--   0 runner    (1001) docker     (127)     3810 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/nn/modules/vader/layers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:06:57.843941 pypots-0.4.1/pypots/optim/
--rw-r--r--   0 runner    (1001) docker     (127)      368 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/optim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1800 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/optim/adadelta.py
--rw-r--r--   0 runner    (1001) docker     (127)     2155 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/optim/adagrad.py
--rw-r--r--   0 runner    (1001) docker     (127)     2058 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/optim/adam.py
--rw-r--r--   0 runner    (1001) docker     (127)     2069 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/optim/adamw.py
--rw-r--r--   0 runner    (1001) docker     (127)     3963 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/optim/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:06:57.843941 pypots-0.4.1/pypots/optim/lr_scheduler/
--rw-r--r--   0 runner    (1001) docker     (127)      983 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/optim/lr_scheduler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6195 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/optim/lr_scheduler/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2899 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/optim/lr_scheduler/constant_lrs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/optim/lr_scheduler/exponential_lrs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2479 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/optim/lr_scheduler/lambda_lrs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3766 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/optim/lr_scheduler/linear_lrs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2576 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/optim/lr_scheduler/multiplicative_lrs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2494 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/optim/lr_scheduler/multistep_lrs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2254 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/optim/lr_scheduler/step_lrs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2127 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/optim/rmsprop.py
--rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/optim/sgd.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:06:57.847941 pypots-0.4.1/pypots/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/utils/file.py
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/utils/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:06:57.847941 pypots-0.4.1/pypots/utils/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/utils/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7426 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/utils/metrics/classification.py
--rw-r--r--   0 runner    (1001) docker     (127)     8597 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/utils/metrics/clustering.py
--rw-r--r--   0 runner    (1001) docker     (127)    13674 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/utils/metrics/error.py
--rw-r--r--   0 runner    (1001) docker     (127)      861 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/utils/random.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:06:57.847941 pypots-0.4.1/pypots/utils/visual/
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/utils/visual/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10008 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/utils/visual/clustering.py
--rw-r--r--   0 runner    (1001) docker     (127)     5827 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/utils/visual/data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:06:57.815940 pypots-0.4.1/pypots.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    27877 2024-04-17 16:06:57.000000 pypots-0.4.1/pypots.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7346 2024-04-17 16:06:57.000000 pypots-0.4.1/pypots.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 16:06:57.000000 pypots-0.4.1/pypots.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-17 16:06:57.000000 pypots-0.4.1/pypots.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      881 2024-04-17 16:06:57.000000 pypots-0.4.1/pypots.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-17 16:06:57.000000 pypots-0.4.1/pypots.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      577 2024-04-17 16:06:57.847941 pypots-0.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2644 2024-04-17 16:04:57.000000 pypots-0.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:24:30.542978 pypots-0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-05-06 14:22:32.000000 pypots-0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-06 14:22:32.000000 pypots-0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    28506 2024-05-06 14:24:30.542978 pypots-0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    26693 2024-05-06 14:22:32.000000 pypots-0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:24:30.506978 pypots-0.5/pypots/
+-rw-r--r--   0 runner    (1001) docker     (127)      782 2024-05-06 14:22:32.000000 pypots-0.5/pypots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22480 2024-05-06 14:22:32.000000 pypots-0.5/pypots/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:24:30.506978 pypots-0.5/pypots/classification/
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-06 14:22:32.000000 pypots-0.5/pypots/classification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17630 2024-05-06 14:22:32.000000 pypots-0.5/pypots/classification/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:24:30.506978 pypots-0.5/pypots/classification/brits/
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-05-06 14:22:32.000000 pypots-0.5/pypots/classification/brits/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2904 2024-05-06 14:22:32.000000 pypots-0.5/pypots/classification/brits/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2110 2024-05-06 14:22:32.000000 pypots-0.5/pypots/classification/brits/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9224 2024-05-06 14:22:32.000000 pypots-0.5/pypots/classification/brits/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:24:30.510978 pypots-0.5/pypots/classification/grud/
+-rw-r--r--   0 runner    (1001) docker     (127)      589 2024-05-06 14:22:32.000000 pypots-0.5/pypots/classification/grud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2096 2024-05-06 14:22:32.000000 pypots-0.5/pypots/classification/grud/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5326 2024-05-06 14:22:32.000000 pypots-0.5/pypots/classification/grud/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8436 2024-05-06 14:22:32.000000 pypots-0.5/pypots/classification/grud/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:24:30.510978 pypots-0.5/pypots/classification/raindrop/
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-05-06 14:22:32.000000 pypots-0.5/pypots/classification/raindrop/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3579 2024-05-06 14:22:32.000000 pypots-0.5/pypots/classification/raindrop/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1955 2024-05-06 14:22:32.000000 pypots-0.5/pypots/classification/raindrop/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9646 2024-05-06 14:22:32.000000 pypots-0.5/pypots/classification/raindrop/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:24:30.510978 pypots-0.5/pypots/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-06 14:22:32.000000 pypots-0.5/pypots/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2552 2024-05-06 14:22:32.000000 pypots-0.5/pypots/cli/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6268 2024-05-06 14:22:32.000000 pypots-0.5/pypots/cli/dev.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7915 2024-05-06 14:22:32.000000 pypots-0.5/pypots/cli/doc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4534 2024-05-06 14:22:32.000000 pypots-0.5/pypots/cli/env.py
+-rw-r--r--   0 runner    (1001) docker     (127)      969 2024-05-06 14:22:32.000000 pypots-0.5/pypots/cli/pypots_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9149 2024-05-06 14:22:32.000000 pypots-0.5/pypots/cli/tuning.py
+-rw-r--r--   0 runner    (1001) docker     (127)      658 2024-05-06 14:22:32.000000 pypots-0.5/pypots/cli/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:24:30.510978 pypots-0.5/pypots/clustering/
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-05-06 14:22:32.000000 pypots-0.5/pypots/clustering/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16739 2024-05-06 14:22:32.000000 pypots-0.5/pypots/clustering/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:24:30.510978 pypots-0.5/pypots/clustering/crli/
+-rw-r--r--   0 runner    (1001) docker     (127)      548 2024-05-06 14:22:32.000000 pypots-0.5/pypots/clustering/crli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3250 2024-05-06 14:22:32.000000 pypots-0.5/pypots/clustering/crli/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2308 2024-05-06 14:22:32.000000 pypots-0.5/pypots/clustering/crli/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18175 2024-05-06 14:22:32.000000 pypots-0.5/pypots/clustering/crli/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:24:30.510978 pypots-0.5/pypots/clustering/vader/
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-05-06 14:22:32.000000 pypots-0.5/pypots/clustering/vader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5055 2024-05-06 14:22:32.000000 pypots-0.5/pypots/clustering/vader/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2311 2024-05-06 14:22:32.000000 pypots-0.5/pypots/clustering/vader/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20197 2024-05-06 14:22:32.000000 pypots-0.5/pypots/clustering/vader/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:24:30.514978 pypots-0.5/pypots/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-05-06 14:22:32.000000 pypots-0.5/pypots/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      825 2024-05-06 14:22:32.000000 pypots-0.5/pypots/data/checking.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:24:30.514978 pypots-0.5/pypots/data/dataset/
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-05-06 14:22:32.000000 pypots-0.5/pypots/data/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19043 2024-05-06 14:22:32.000000 pypots-0.5/pypots/data/dataset/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-05-06 14:22:32.000000 pypots-0.5/pypots/data/dataset/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13991 2024-05-06 14:22:32.000000 pypots-0.5/pypots/data/generating.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1822 2024-05-06 14:22:32.000000 pypots-0.5/pypots/data/load_preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2107 2024-05-06 14:22:32.000000 pypots-0.5/pypots/data/load_specific_datasets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:24:30.514978 pypots-0.5/pypots/data/saving/
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-06 14:22:32.000000 pypots-0.5/pypots/data/saving/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4518 2024-05-06 14:22:32.000000 pypots-0.5/pypots/data/saving/h5.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1434 2024-05-06 14:22:32.000000 pypots-0.5/pypots/data/saving/pickle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7435 2024-05-06 14:22:32.000000 pypots-0.5/pypots/data/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:24:30.514978 pypots-0.5/pypots/forecasting/
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-06 14:22:32.000000 pypots-0.5/pypots/forecasting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17454 2024-05-06 14:22:32.000000 pypots-0.5/pypots/forecasting/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:24:30.514978 pypots-0.5/pypots/forecasting/bttf/
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-05-06 14:22:32.000000 pypots-0.5/pypots/forecasting/bttf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8941 2024-05-06 14:22:32.000000 pypots-0.5/pypots/forecasting/bttf/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4420 2024-05-06 14:22:32.000000 pypots-0.5/pypots/forecasting/bttf/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6228 2024-05-06 14:22:32.000000 pypots-0.5/pypots/forecasting/bttf/submodules.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:24:30.514978 pypots-0.5/pypots/forecasting/csdi/
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2024-05-06 14:22:32.000000 pypots-0.5/pypots/forecasting/csdi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5247 2024-05-06 14:22:32.000000 pypots-0.5/pypots/forecasting/csdi/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11470 2024-05-06 14:22:32.000000 pypots-0.5/pypots/forecasting/csdi/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17628 2024-05-06 14:22:32.000000 pypots-0.5/pypots/forecasting/csdi/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:24:30.514978 pypots-0.5/pypots/imputation/
+-rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-05-06 14:22:32.000000 pypots-0.5/pypots/imputation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:24:30.518978 pypots-0.5/pypots/imputation/autoformer/
+-rw-r--r--   0 runner    (1001) docker     (127)      705 2024-05-06 14:22:32.000000 pypots-0.5/pypots/imputation/autoformer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2936 2024-05-06 14:22:32.000000 pypots-0.5/pypots/imputation/autoformer/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-05-06 14:22:32.000000 pypots-0.5/pypots/imputation/autoformer/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10792 2024-05-06 14:22:32.000000 pypots-0.5/pypots/imputation/autoformer/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17417 2024-05-06 14:22:32.000000 pypots-0.5/pypots/imputation/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:24:30.518978 pypots-0.5/pypots/imputation/brits/
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-05-06 14:22:32.000000 pypots-0.5/pypots/imputation/brits/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2007 2024-05-06 14:22:32.000000 pypots-0.5/pypots/imputation/brits/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6751 2024-05-06 14:22:32.000000 pypots-0.5/pypots/imputation/brits/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9069 2024-05-06 14:22:32.000000 pypots-0.5/pypots/imputation/brits/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:24:30.518978 pypots-0.5/pypots/imputation/crossformer/
+-rw-r--r--   0 runner    (1001) docker     (127)      560 2024-05-06 14:22:32.000000 pypots-0.5/pypots/imputation/crossformer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4296 2024-05-06 14:22:32.000000 pypots-0.5/pypots/imputation/crossformer/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-06 14:22:32.000000 pypots-0.5/pypots/imputation/crossformer/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10902 2024-05-06 14:22:32.000000 pypots-0.5/pypots/imputation/crossformer/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:24:30.518978 pypots-0.5/pypots/imputation/csdi/
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2024-05-06 14:22:32.000000 pypots-0.5/pypots/imputation/csdi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4738 2024-05-06 14:22:32.000000 pypots-0.5/pypots/imputation/csdi/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10893 2024-05-06 14:22:32.000000 pypots-0.5/pypots/imputation/csdi/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16770 2024-05-06 14:22:32.000000 pypots-0.5/pypots/imputation/csdi/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:24:30.518978 pypots-0.5/pypots/imputation/dlinear/
+-rw-r--r--   0 runner    (1001) docker     (127)      562 2024-05-06 14:22:32.000000 pypots-0.5/pypots/imputation/dlinear/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3647 2024-05-06 14:22:32.000000 pypots-0.5/pypots/imputation/dlinear/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)      583 2024-05-06 14:22:32.000000 pypots-0.5/pypots/imputation/dlinear/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10367 2024-05-06 14:22:32.000000 pypots-0.5/pypots/imputation/dlinear/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:24:30.518978 pypots-0.5/pypots/imputation/etsformer/
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-05-06 14:22:32.000000 pypots-0.5/pypots/imputation/etsformer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3573 2024-05-06 14:22:32.000000 pypots-0.5/pypots/imputation/etsformer/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)      589 2024-05-06 14:22:32.000000 pypots-0.5/pypots/imputation/etsformer/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10651 2024-05-06 14:22:32.000000 pypots-0.5/pypots/imputation/etsformer/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:24:30.518978 pypots-0.5/pypots/imputation/fedformer/
+-rw-r--r--   0 runner    (1001) docker     (127)      671 2024-05-06 14:22:32.000000 pypots-0.5/pypots/imputation/fedformer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3005 2024-05-06 14:22:32.000000 pypots-0.5/pypots/imputation/fedformer/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)      589 2024-05-06 14:22:32.000000 pypots-0.5/pypots/imputation/fedformer/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11252 2024-05-06 14:22:32.000000 pypots-0.5/pypots/imputation/fedformer/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:24:30.522978 pypots-0.5/pypots/imputation/film/
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-05-06 14:22:32.000000 pypots-0.5/pypots/imputation/film/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2749 2024-05-06 14:22:32.000000 pypots-0.5/pypots/imputation/film/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-05-06 14:22:32.000000 pypots-0.5/pypots/imputation/film/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10705 2024-05-06 14:22:32.000000 pypots-0.5/pypots/imputation/film/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:24:30.522978 pypots-0.5/pypots/imputation/frets/
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-05-06 14:22:32.000000 pypots-0.5/pypots/imputation/frets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2911 2024-05-06 14:22:32.000000 pypots-0.5/pypots/imputation/frets/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)      577 2024-05-06 14:22:32.000000 pypots-0.5/pypots/imputation/frets/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10251 2024-05-06 14:22:32.000000 pypots-0.5/pypots/imputation/frets/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:24:30.522978 pypots-0.5/pypots/imputation/gpvae/
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-05-06 14:22:32.000000 pypots-0.5/pypots/imputation/gpvae/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-05-06 14:22:32.000000 pypots-0.5/pypots/imputation/gpvae/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5063 2024-05-06 14:22:32.000000 pypots-0.5/pypots/imputation/gpvae/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17420 2024-05-06 14:22:32.000000 pypots-0.5/pypots/imputation/gpvae/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:24:30.522978 pypots-0.5/pypots/imputation/informer/
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-05-06 14:22:32.000000 pypots-0.5/pypots/imputation/informer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3508 2024-05-06 14:22:32.000000 pypots-0.5/pypots/imputation/informer/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-05-06 14:22:32.000000 pypots-0.5/pypots/imputation/informer/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10565 2024-05-06 14:22:32.000000 pypots-0.5/pypots/imputation/informer/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:24:30.522978 pypots-0.5/pypots/imputation/itransformer/
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-05-06 14:22:32.000000 pypots-0.5/pypots/imputation/itransformer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3367 2024-05-06 14:22:32.000000 pypots-0.5/pypots/imputation/itransformer/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-05-06 14:22:32.000000 pypots-0.5/pypots/imputation/itransformer/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10972 2024-05-06 14:22:32.000000 pypots-0.5/pypots/imputation/itransformer/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:24:30.522978 pypots-0.5/pypots/imputation/locf/
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-05-06 14:22:32.000000 pypots-0.5/pypots/imputation/locf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6975 2024-05-06 14:22:32.000000 pypots-0.5/pypots/imputation/locf/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5960 2024-05-06 14:22:32.000000 pypots-0.5/pypots/imputation/locf/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:24:30.522978 pypots-0.5/pypots/imputation/mean/
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-06 14:22:32.000000 pypots-0.5/pypots/imputation/mean/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4552 2024-05-06 14:22:32.000000 pypots-0.5/pypots/imputation/mean/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:24:30.526978 pypots-0.5/pypots/imputation/median/
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-05-06 14:22:32.000000 pypots-0.5/pypots/imputation/median/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4582 2024-05-06 14:22:32.000000 pypots-0.5/pypots/imputation/median/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:24:30.526978 pypots-0.5/pypots/imputation/mrnn/
+-rw-r--r--   0 runner    (1001) docker     (127)      628 2024-05-06 14:22:32.000000 pypots-0.5/pypots/imputation/mrnn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-05-06 14:22:32.000000 pypots-0.5/pypots/imputation/mrnn/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6750 2024-05-06 14:22:32.000000 pypots-0.5/pypots/imputation/mrnn/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9036 2024-05-06 14:22:32.000000 pypots-0.5/pypots/imputation/mrnn/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:24:30.526978 pypots-0.5/pypots/imputation/patchtst/
+-rw-r--r--   0 runner    (1001) docker     (127)      543 2024-05-06 14:22:32.000000 pypots-0.5/pypots/imputation/patchtst/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3278 2024-05-06 14:22:32.000000 pypots-0.5/pypots/imputation/patchtst/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-05-06 14:22:32.000000 pypots-0.5/pypots/imputation/patchtst/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12042 2024-05-06 14:22:32.000000 pypots-0.5/pypots/imputation/patchtst/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:24:30.526978 pypots-0.5/pypots/imputation/saits/
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-05-06 14:22:32.000000 pypots-0.5/pypots/imputation/saits/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3903 2024-05-06 14:22:32.000000 pypots-0.5/pypots/imputation/saits/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6133 2024-05-06 14:22:32.000000 pypots-0.5/pypots/imputation/saits/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14172 2024-05-06 14:22:32.000000 pypots-0.5/pypots/imputation/saits/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:24:30.526978 pypots-0.5/pypots/imputation/timesnet/
+-rw-r--r--   0 runner    (1001) docker     (127)      560 2024-05-06 14:22:32.000000 pypots-0.5/pypots/imputation/timesnet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2368 2024-05-06 14:22:32.000000 pypots-0.5/pypots/imputation/timesnet/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-05-06 14:22:32.000000 pypots-0.5/pypots/imputation/timesnet/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10784 2024-05-06 14:22:32.000000 pypots-0.5/pypots/imputation/timesnet/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:24:30.526978 pypots-0.5/pypots/imputation/transformer/
+-rw-r--r--   0 runner    (1001) docker     (127)      859 2024-05-06 14:22:32.000000 pypots-0.5/pypots/imputation/transformer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2786 2024-05-06 14:22:32.000000 pypots-0.5/pypots/imputation/transformer/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2024-05-06 14:22:32.000000 pypots-0.5/pypots/imputation/transformer/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10951 2024-05-06 14:22:32.000000 pypots-0.5/pypots/imputation/transformer/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:24:30.526978 pypots-0.5/pypots/imputation/usgan/
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-05-06 14:22:32.000000 pypots-0.5/pypots/imputation/usgan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1863 2024-05-06 14:22:32.000000 pypots-0.5/pypots/imputation/usgan/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2143 2024-05-06 14:22:32.000000 pypots-0.5/pypots/imputation/usgan/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17287 2024-05-06 14:22:32.000000 pypots-0.5/pypots/imputation/usgan/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:24:30.526978 pypots-0.5/pypots/nn/
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-06 14:22:32.000000 pypots-0.5/pypots/nn/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:24:30.530978 pypots-0.5/pypots/nn/functional/
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-06 14:22:32.000000 pypots-0.5/pypots/nn/functional/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3251 2024-05-06 14:22:32.000000 pypots-0.5/pypots/nn/functional/normalization.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:24:30.530978 pypots-0.5/pypots/nn/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-06 14:22:32.000000 pypots-0.5/pypots/nn/modules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:24:30.530978 pypots-0.5/pypots/nn/modules/autoformer/
+-rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-05-06 14:22:32.000000 pypots-0.5/pypots/nn/modules/autoformer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-05-06 14:22:32.000000 pypots-0.5/pypots/nn/modules/autoformer/autoencoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11068 2024-05-06 14:22:32.000000 pypots-0.5/pypots/nn/modules/autoformer/layers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:24:30.530978 pypots-0.5/pypots/nn/modules/brits/
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-05-06 14:22:32.000000 pypots-0.5/pypots/nn/modules/brits/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8144 2024-05-06 14:22:32.000000 pypots-0.5/pypots/nn/modules/brits/backbone.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1915 2024-05-06 14:22:32.000000 pypots-0.5/pypots/nn/modules/brits/layers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:24:30.530978 pypots-0.5/pypots/nn/modules/crli/
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-06 14:22:32.000000 pypots-0.5/pypots/nn/modules/crli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-05-06 14:22:32.000000 pypots-0.5/pypots/nn/modules/crli/backbone.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9014 2024-05-06 14:22:32.000000 pypots-0.5/pypots/nn/modules/crli/layers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:24:30.530978 pypots-0.5/pypots/nn/modules/crossformer/
+-rw-r--r--   0 runner    (1001) docker     (127)      755 2024-05-06 14:22:32.000000 pypots-0.5/pypots/nn/modules/crossformer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-05-06 14:22:32.000000 pypots-0.5/pypots/nn/modules/crossformer/autoencoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6718 2024-05-06 14:22:32.000000 pypots-0.5/pypots/nn/modules/crossformer/layers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:24:30.530978 pypots-0.5/pypots/nn/modules/csdi/
+-rw-r--r--   0 runner    (1001) docker     (127)      779 2024-05-06 14:22:32.000000 pypots-0.5/pypots/nn/modules/csdi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5992 2024-05-06 14:22:32.000000 pypots-0.5/pypots/nn/modules/csdi/backbone.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6498 2024-05-06 14:22:32.000000 pypots-0.5/pypots/nn/modules/csdi/layers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:24:30.530978 pypots-0.5/pypots/nn/modules/dlinear/
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-05-06 14:22:32.000000 pypots-0.5/pypots/nn/modules/dlinear/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3127 2024-05-06 14:22:32.000000 pypots-0.5/pypots/nn/modules/dlinear/backbone.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:24:30.530978 pypots-0.5/pypots/nn/modules/etsformer/
+-rw-r--r--   0 runner    (1001) docker     (127)      734 2024-05-06 14:22:32.000000 pypots-0.5/pypots/nn/modules/etsformer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-05-06 14:22:32.000000 pypots-0.5/pypots/nn/modules/etsformer/autoencoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10373 2024-05-06 14:22:32.000000 pypots-0.5/pypots/nn/modules/etsformer/layers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:24:30.530978 pypots-0.5/pypots/nn/modules/fedformer/
+-rw-r--r--   0 runner    (1001) docker     (127)      925 2024-05-06 14:22:32.000000 pypots-0.5/pypots/nn/modules/fedformer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4341 2024-05-06 14:22:32.000000 pypots-0.5/pypots/nn/modules/fedformer/autoencoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32398 2024-05-06 14:22:32.000000 pypots-0.5/pypots/nn/modules/fedformer/layers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:24:30.534978 pypots-0.5/pypots/nn/modules/film/
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2024-05-06 14:22:32.000000 pypots-0.5/pypots/nn/modules/film/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2632 2024-05-06 14:22:32.000000 pypots-0.5/pypots/nn/modules/film/backbone.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4369 2024-05-06 14:22:32.000000 pypots-0.5/pypots/nn/modules/film/layers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:24:30.534978 pypots-0.5/pypots/nn/modules/frets/
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2024-05-06 14:22:32.000000 pypots-0.5/pypots/nn/modules/frets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4305 2024-05-06 14:22:32.000000 pypots-0.5/pypots/nn/modules/frets/backbone.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:24:30.534978 pypots-0.5/pypots/nn/modules/gpvae/
+-rw-r--r--   0 runner    (1001) docker     (127)      644 2024-05-06 14:22:32.000000 pypots-0.5/pypots/nn/modules/gpvae/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6158 2024-05-06 14:22:32.000000 pypots-0.5/pypots/nn/modules/gpvae/backbone.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8580 2024-05-06 14:22:32.000000 pypots-0.5/pypots/nn/modules/gpvae/layers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:24:30.534978 pypots-0.5/pypots/nn/modules/grud/
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-05-06 14:22:32.000000 pypots-0.5/pypots/nn/modules/grud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2188 2024-05-06 14:22:32.000000 pypots-0.5/pypots/nn/modules/grud/backbone.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2402 2024-05-06 14:22:32.000000 pypots-0.5/pypots/nn/modules/grud/layers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:24:30.534978 pypots-0.5/pypots/nn/modules/informer/
+-rw-r--r--   0 runner    (1001) docker     (127)      908 2024-05-06 14:22:32.000000 pypots-0.5/pypots/nn/modules/informer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1742 2024-05-06 14:22:32.000000 pypots-0.5/pypots/nn/modules/informer/autoencoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7612 2024-05-06 14:22:32.000000 pypots-0.5/pypots/nn/modules/informer/layers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:24:30.534978 pypots-0.5/pypots/nn/modules/mrnn/
+-rw-r--r--   0 runner    (1001) docker     (127)      680 2024-05-06 14:22:32.000000 pypots-0.5/pypots/nn/modules/mrnn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2706 2024-05-06 14:22:32.000000 pypots-0.5/pypots/nn/modules/mrnn/backbone.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-05-06 14:22:32.000000 pypots-0.5/pypots/nn/modules/mrnn/layers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:24:30.534978 pypots-0.5/pypots/nn/modules/patchtst/
+-rw-r--r--   0 runner    (1001) docker     (127)      712 2024-05-06 14:22:32.000000 pypots-0.5/pypots/nn/modules/patchtst/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-05-06 14:22:32.000000 pypots-0.5/pypots/nn/modules/patchtst/autoencoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4684 2024-05-06 14:22:32.000000 pypots-0.5/pypots/nn/modules/patchtst/layers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:24:30.534978 pypots-0.5/pypots/nn/modules/raindrop/
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-05-06 14:22:32.000000 pypots-0.5/pypots/nn/modules/raindrop/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7360 2024-05-06 14:22:32.000000 pypots-0.5/pypots/nn/modules/raindrop/backbone.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11269 2024-05-06 14:22:32.000000 pypots-0.5/pypots/nn/modules/raindrop/layers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:24:30.534978 pypots-0.5/pypots/nn/modules/saits/
+-rw-r--r--   0 runner    (1001) docker     (127)      602 2024-05-06 14:22:32.000000 pypots-0.5/pypots/nn/modules/saits/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4520 2024-05-06 14:22:32.000000 pypots-0.5/pypots/nn/modules/saits/backbone.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-05-06 14:22:32.000000 pypots-0.5/pypots/nn/modules/saits/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-05-06 14:22:32.000000 pypots-0.5/pypots/nn/modules/saits/loss.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:24:30.538978 pypots-0.5/pypots/nn/modules/timesnet/
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-06 14:22:32.000000 pypots-0.5/pypots/nn/modules/timesnet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      890 2024-05-06 14:22:32.000000 pypots-0.5/pypots/nn/modules/timesnet/backbone.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3509 2024-05-06 14:22:32.000000 pypots-0.5/pypots/nn/modules/timesnet/layers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:24:30.538978 pypots-0.5/pypots/nn/modules/transformer/
+-rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-05-06 14:22:32.000000 pypots-0.5/pypots/nn/modules/transformer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6234 2024-05-06 14:22:32.000000 pypots-0.5/pypots/nn/modules/transformer/attention.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6065 2024-05-06 14:22:32.000000 pypots-0.5/pypots/nn/modules/transformer/autoencoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5742 2024-05-06 14:22:32.000000 pypots-0.5/pypots/nn/modules/transformer/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6580 2024-05-06 14:22:32.000000 pypots-0.5/pypots/nn/modules/transformer/layers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:24:30.538978 pypots-0.5/pypots/nn/modules/usgan/
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-05-06 14:22:32.000000 pypots-0.5/pypots/nn/modules/usgan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2655 2024-05-06 14:22:32.000000 pypots-0.5/pypots/nn/modules/usgan/backbone.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1994 2024-05-06 14:22:32.000000 pypots-0.5/pypots/nn/modules/usgan/layers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:24:30.538978 pypots-0.5/pypots/nn/modules/vader/
+-rw-r--r--   0 runner    (1001) docker     (127)      840 2024-05-06 14:22:32.000000 pypots-0.5/pypots/nn/modules/vader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4547 2024-05-06 14:22:32.000000 pypots-0.5/pypots/nn/modules/vader/backbone.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3498 2024-05-06 14:22:32.000000 pypots-0.5/pypots/nn/modules/vader/layers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:24:30.538978 pypots-0.5/pypots/optim/
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2024-05-06 14:22:32.000000 pypots-0.5/pypots/optim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1800 2024-05-06 14:22:32.000000 pypots-0.5/pypots/optim/adadelta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2155 2024-05-06 14:22:32.000000 pypots-0.5/pypots/optim/adagrad.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2058 2024-05-06 14:22:32.000000 pypots-0.5/pypots/optim/adam.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2069 2024-05-06 14:22:32.000000 pypots-0.5/pypots/optim/adamw.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3963 2024-05-06 14:22:32.000000 pypots-0.5/pypots/optim/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:24:30.542978 pypots-0.5/pypots/optim/lr_scheduler/
+-rw-r--r--   0 runner    (1001) docker     (127)      983 2024-05-06 14:22:32.000000 pypots-0.5/pypots/optim/lr_scheduler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6195 2024-05-06 14:22:32.000000 pypots-0.5/pypots/optim/lr_scheduler/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2899 2024-05-06 14:22:32.000000 pypots-0.5/pypots/optim/lr_scheduler/constant_lrs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-05-06 14:22:32.000000 pypots-0.5/pypots/optim/lr_scheduler/exponential_lrs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2479 2024-05-06 14:22:32.000000 pypots-0.5/pypots/optim/lr_scheduler/lambda_lrs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3766 2024-05-06 14:22:32.000000 pypots-0.5/pypots/optim/lr_scheduler/linear_lrs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2576 2024-05-06 14:22:32.000000 pypots-0.5/pypots/optim/lr_scheduler/multiplicative_lrs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2494 2024-05-06 14:22:32.000000 pypots-0.5/pypots/optim/lr_scheduler/multistep_lrs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2254 2024-05-06 14:22:32.000000 pypots-0.5/pypots/optim/lr_scheduler/step_lrs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2127 2024-05-06 14:22:32.000000 pypots-0.5/pypots/optim/rmsprop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-05-06 14:22:32.000000 pypots-0.5/pypots/optim/sgd.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:24:30.542978 pypots-0.5/pypots/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-05-06 14:22:32.000000 pypots-0.5/pypots/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-05-06 14:22:32.000000 pypots-0.5/pypots/utils/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-05-06 14:22:32.000000 pypots-0.5/pypots/utils/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:24:30.542978 pypots-0.5/pypots/utils/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-05-06 14:22:32.000000 pypots-0.5/pypots/utils/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7426 2024-05-06 14:22:32.000000 pypots-0.5/pypots/utils/metrics/classification.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8597 2024-05-06 14:22:32.000000 pypots-0.5/pypots/utils/metrics/clustering.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13674 2024-05-06 14:22:32.000000 pypots-0.5/pypots/utils/metrics/error.py
+-rw-r--r--   0 runner    (1001) docker     (127)      861 2024-05-06 14:22:32.000000 pypots-0.5/pypots/utils/random.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:24:30.542978 pypots-0.5/pypots/utils/visual/
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-05-06 14:22:32.000000 pypots-0.5/pypots/utils/visual/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10008 2024-05-06 14:22:32.000000 pypots-0.5/pypots/utils/visual/clustering.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5774 2024-05-06 14:22:32.000000 pypots-0.5/pypots/utils/visual/data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:24:30.506978 pypots-0.5/pypots.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    28506 2024-05-06 14:24:30.000000 pypots-0.5/pypots.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8178 2024-05-06 14:24:30.000000 pypots-0.5/pypots.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 14:24:30.000000 pypots-0.5/pypots.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-06 14:24:30.000000 pypots-0.5/pypots.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      881 2024-05-06 14:24:30.000000 pypots-0.5/pypots.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-06 14:24:30.000000 pypots-0.5/pypots.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      577 2024-05-06 14:24:30.542978 pypots-0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2644 2024-05-06 14:22:32.000000 pypots-0.5/setup.py
```

### Comparing `pypots-0.4.1/LICENSE` & `pypots-0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pypots-0.4.1/PKG-INFO` & `pypots-0.5/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypots
-Version: 0.4.1
+Version: 0.5
 Summary: A Python Toolbox for Data Mining on Partially-Observed Time Series
 Home-page: https://pypots.com/
 Author: Wenjie Du
 Author-email: wenjay.du@gmail.com
 License: BSD-3-Clause
 Project-URL: Documentation, https://docs.pypots.com/
 Project-URL: Source, https://github.com/WenjieDu/PyPOTS/
@@ -86,14 +86,17 @@
     </a>
     <a href="https://pepy.tech/project/pypots">
         <img alt="PyPI downloads" src="https://img.shields.io/endpoint?url=https://pypots.com/figs/downloads_badges/pypi_pypots_downloads.json">
     </a>
     <a href="https://arxiv.org/abs/2305.18811">
         <img alt="arXiv DOI" src="https://img.shields.io/badge/DOI-10.48550/arXiv.2305.18811-F8F7F0">
     </a>
+    <a href="https://github.com/WenjieDu/PyPOTS/blob/main/README_zh.md">
+        <img alt="README in Chinese" src="https://img.shields.io/badge/README-🇨🇳中文版-FCEFE8">
+    </a>
 </p>
 
 ⦿ `Motivation`: Due to all kinds of reasons like failure of collection sensors, communication error,
 and unexpected malfunction, missing values are common to see in time series from the real-world environment.
 This makes partially-observed time series (POTS) a pervasive problem in open-world modeling and prevents advanced
 data analysis. Although this problem is important, the area of machine learning on POTS still lacks a dedicated toolkit.
 PyPOTS is created to fill in this blank.
@@ -105,36 +108,90 @@
 have unified APIs together with detailed documentation and interactive examples across algorithms as tutorials.
 
 🤗 **Please** star this repo to help others notice PyPOTS if you think it is a useful toolkit.
 **Please** properly [cite PyPOTS](https://github.com/WenjieDu/PyPOTS#-citing-pypots) in your publications
 if it helps with your research. This really means a lot to our open-source research. Thank you!
 
 The rest of this readme file is organized as follows:
+[**❖ Available Algorithms**](#-available-algorithms),
 [**❖ PyPOTS Ecosystem**](#-pypots-ecosystem),
 [**❖ Installation**](#-installation),
 [**❖ Usage**](#-usage),
-[**❖ Available Algorithms**](#-available-algorithms),
 [**❖ Citing PyPOTS**](#-citing-pypots),
 [**❖ Contribution**](#-contribution),
 [**❖ Community**](#-community).
 
 
+## ❖ Available Algorithms
+PyPOTS supports imputation, classification, clustering, forecasting, and anomaly detection tasks on multivariate partially-observed
+time series with missing values. The table below shows the availability of each algorithm (sorted by Year) in PyPOTS for different tasks.
+The symbol ✅ indicates the algorithm is available for the corresponding task (note that models will be continuously updated
+in the future to handle tasks that are not currently supported. Stay tuned❗️).
+
+🌟 Since **v0.2**, all neural-network models in PyPOTS has got hyperparameter-optimization support.
+This functionality is implemented with the [Microsoft NNI](https://github.com/microsoft/nni) framework. You may want to refer to our time-series
+imputation survey repo [Awesome_Imputation](https://github.com/WenjieDu/Awesome_Imputation) to see how to config and
+tune the hyperparameters.
+
+🔥 Note that Transformer, iTransformer, FreTS, Crossformer, PatchTST, DLinear, ETSformer, FiLM, FEDformer, Informer, Autoformer
+are not proposed as imputation methods in their original papers, and they cannot accept POTS as input.
+**To make them applicable on POTS data, we apply the embedding strategy and training approach (ORT+MIT)
+the same as we did in [SAITS paper](https://arxiv.org/pdf/2202.08516).**
+
+The task types are abbreviated as follows:
+**`IMPU`**: Imputation;
+**`FORE`**: Forecasting;
+**`CLAS`**: Classification;
+**`CLUS`**: Clustering;
+**`ANOD`**: Anomaly Detection.
+The paper references and links are all listed at the bottom of this file.
+
+| **Type**      | **Algo**                           | **IMPU** | **FORE** | **CLAS** | **CLUS** | **ANOD** | **Year - Venue** |
+|:--------------|:-----------------------------------|:--------:|:--------:|:--------:|:--------:|:--------:|:-----------------|
+| Neural Net    | iTransformer[^24]                  |    ✅     |          |          |          |          | 2024 - ICLR      |
+| Neural Net    | FreTS[^23]                         |    ✅     |          |          |          |          | 2024 - NeurIPS   |
+| Neural Net    | SAITS[^1]                          |    ✅     |          |          |          |          | 2023 - ESWA      |
+| Neural Net    | Crossformer[^16]                   |    ✅     |          |          |          |          | 2023 - ICLR      |
+| Neural Net    | TimesNet[^14]                      |    ✅     |          |          |          |          | 2023 - ICLR      |
+| Neural Net    | PatchTST[^18]                      |    ✅     |          |          |          |          | 2023 - ICLR      |
+| Neural Net    | ETSformer[^19]                     |    ✅     |          |          |          |          | 2023 - ICLR      |
+| Neural Net    | DLinear[^17]                       |    ✅     |          |          |          |          | 2023 - AAAI      |
+| Neural Net    | FiLM[^22]                          |    ✅     |          |          |          |          | 2022 - NeurIPS   |
+| Neural Net    | Raindrop[^5]                       |          |          |    ✅     |          |          | 2022 - ICLR      |
+| Neural Net    | FEDformer[^20]                     |    ✅     |          |          |          |          | 2022 - ICML      |
+| Neural Net    | Autoformer[^15]                    |    ✅     |          |          |          |          | 2021 - NeurIPS   |
+| Neural Net    | CSDI[^12]                          |    ✅     |    ✅     |          |          |          | 2021 - NeurIPS   |
+| Neural Net    | Informer[^21]                      |    ✅     |          |          |          |          | 2021 - AAAI      |
+| Neural Net    | US-GAN[^10]                        |    ✅     |          |          |          |          | 2021 - AAAI      |
+| Neural Net    | CRLI[^6]                           |          |          |          |    ✅     |          | 2021 - AAAI      |
+| Probabilistic | BTTF[^8]                           |          |    ✅     |          |          |          | 2021 - TPAMI     |
+| Neural Net    | GP-VAE[^11]                        |    ✅     |          |          |          |          | 2020 - AISTATS   |
+| Neural Net    | VaDER[^7]                          |          |          |          |    ✅     |          | 2019 - GigaSci.  |
+| Neural Net    | M-RNN[^9]                          |    ✅     |          |          |          |          | 2019 - TBME      |
+| Neural Net    | BRITS[^3]                          |    ✅     |          |    ✅     |          |          | 2018 - NeurIPS   |
+| Neural Net    | GRU-D[^4]                          |    ✅     |          |    ✅     |          |          | 2018 - Sci. Rep. |
+| Neural Net    | Transformer[^2]                    |    ✅     |          |          |          |          | 2017 - NeurIPS   |
+| Naive         | LOCF/NOCB                          |    ✅     |          |          |          |          |                  |
+| Naive         | Mean                               |    ✅     |          |          |          |          |                  |
+| Naive         | Median                             |    ✅     |          |          |          |          |                  |
+
+
 ## ❖ PyPOTS Ecosystem
 At PyPOTS, things are related to coffee, which we're familiar with. Yes, this is a coffee universe!
 As you can see, there is a coffee pot in the PyPOTS logo.
 And what else? Please read on ;-)
 
 <a href="https://github.com/WenjieDu/TSDB">
     <img src="https://pypots.com/figs/pypots_logos/TSDB/logo_FFBG.svg" align="left" width="140" alt="TSDB logo"/>
 </a>
 
 👈 Time series datasets are taken as coffee beans at PyPOTS, and POTS datasets are incomplete coffee beans with missing parts that have their own meanings.
 To make various public time-series datasets readily available to users,
 <i>Time Series Data Beans (TSDB)</i> is created to make loading time-series datasets super easy!
-Visit [TSDB](https://github.com/WenjieDu/TSDB) right now to know more about this handy tool 🛠, and it now supports a total of 168 open-source datasets!
+Visit [TSDB](https://github.com/WenjieDu/TSDB) right now to know more about this handy tool 🛠, and it now supports a total of 169 open-source datasets!
 
 <a href="https://github.com/WenjieDu/PyGrinder">
     <img src="https://pypots.com/figs/pypots_logos/PyGrinder/logo_FFBG.svg" align="right" width="140" alt="PyGrinder logo"/>
 </a>
 
 👉 To simulate the real-world data beans with missingness, the ecosystem library [PyGrinder](https://github.com/WenjieDu/PyGrinder),
 a toolkit helping grind your coffee beans into incomplete ones, is created. Missing patterns fall into three categories according to Robin's theory[^13]:
@@ -160,15 +217,15 @@
 </p>
 
 
 ## ❖ Installation
 You can refer to [the installation instruction](https://docs.pypots.com/en/latest/install.html) in PyPOTS documentation for a guideline with more details.
 
 PyPOTS is available on both [PyPI](https://pypi.python.org/pypi/pypots) and [Anaconda](https://anaconda.org/conda-forge/pypots).
-You can install PyPOTS as shown below:
+You can install PyPOTS like below as well as TSDB and PyGrinder:
 
 ``` bash
 # via pip
 pip install pypots            # the first time installation
 pip install pypots --upgrade  # update pypots to the latest version
 # install from the latest source code with the latest features but may be not officially released yet
 pip install https://github.com/WenjieDu/PyPOTS/archive/main.zip
@@ -188,91 +245,45 @@
 
 We present you a usage example of imputing missing values in time series with PyPOTS below, you can click it to view.
 
 <details open>
 <summary><b>Click here to see an example applying SAITS on PhysioNet2012 for imputation:</b></summary>
 
 ``` python
+# Data preprocessing. Tedious, but PyPOTS can help.
 import numpy as np
 from sklearn.preprocessing import StandardScaler
 from pygrinder import mcar
 from pypots.data import load_specific_dataset
-from pypots.imputation import SAITS
-from pypots.utils.metrics import calc_mae
-
-# Data preprocessing. Tedious, but PyPOTS can help.
 data = load_specific_dataset('physionet_2012')  # PyPOTS will automatically download and extract it.
 X = data['X']
 num_samples = len(X['RecordID'].unique())
 X = X.drop(['RecordID', 'Time'], axis = 1)
 X = StandardScaler().fit_transform(X.to_numpy())
 X = X.reshape(num_samples, 48, -1)
 X_ori = X  # keep X_ori for validation
 X = mcar(X, 0.1)  # randomly hold out 10% observed values as ground truth
 dataset = {"X": X}  # X for model input
 print(X.shape)  # (11988, 48, 37), 11988 samples and each sample has 48 time steps, 37 features
 
 # Model training. This is PyPOTS showtime.
-saits = SAITS(n_steps=48, n_features=37, n_layers=2, d_model=256, d_ffn=128, n_heads=4, d_k=64, d_v=64, dropout=0.1, epochs=10)
+from pypots.imputation import SAITS
+from pypots.utils.metrics import calc_mae
+saits = SAITS(n_steps=48, n_features=37, n_layers=2, d_model=256, n_heads=4, d_k=64, d_v=64, d_ffn=128, dropout=0.1, epochs=10)
 # Here I use the whole dataset as the training set because ground truth is not visible to the model, you can also split it into train/val/test sets
-saits.fit(dataset)
+saits.fit(dataset)  # train the model on the dataset
 imputation = saits.impute(dataset)  # impute the originally-missing values and artificially-missing values
 indicating_mask = np.isnan(X) ^ np.isnan(X_ori)  # indicating mask for imputation error calculation
 mae = calc_mae(imputation, np.nan_to_num(X_ori), indicating_mask)  # calculate mean absolute error on the ground truth (artificially-missing values)
+saits.save("save_it_here/saits_physionet2012.pypots")  # save the model for future use
+saits.load("save_it_here/saits_physionet2012.pypots")  # reload the serialized model file for following imputation or training
 ```
 </details>
 
 
-## ❖ Available Algorithms
-PyPOTS supports imputation, classification, clustering, and forecasting tasks on multivariate time series with missing values.
-The currently available algorithms of four tasks are cataloged in the following table with four partitions.
-The paper references are all listed at the bottom of this readme file.
-
-🌟 Since **v0.2**, all neural-network models in PyPOTS has got hyperparameter-optimization support.
-This functionality is implemented with the [Microsoft NNI](https://github.com/microsoft/nni) framework.
-
-🔥 Note that Transformer, Crossformer, PatchTST, DLinear, ETSformer, FEDformer, Informer, Autoformer are not proposed as imputation methods in their original papers,
-and they cannot accept POTS as input. **To make them applicable on POTS data, we apply the embedding strategy and training approach (ORT+MIT)
-the same as we did in [SAITS paper](https://arxiv.org/pdf/2202.08516).**
-
-|   ***`Imputation`***   |     🚥      |                                               🚥                                                |    🚥    |
-|:----------------------:|:-----------:|:-----------------------------------------------------------------------------------------------:|:--------:|
-|        **Type**        |  **Abbr.**  |                              **Full name of the algorithm/model**                               | **Year** |
-|       Neural Net       |    SAITS    |                      Self-Attention-based Imputation for Time Series [^1]                       |   2023   |
-|       Neural Net       | Transformer |                                 Attention is All you Need [^2]                                  |   2017   |
-|       Neural Net       | Crossformer | Transformer Utilizing Cross-Dimension Dependency for Multivariate Time Series Forecasting [^16] |   2023   |
-|       Neural Net       |  TimesNet   |              Temporal 2D-Variation Modeling for General Time Series Analysis [^14]              |   2023   |
-|       Neural Net       |  PatchTST   |         A Time Series is Worth 64 Words: Long-Term Forecasting with Transformers [^18]          |   2023   |
-|       Neural Net       |   DLinear   |                  Are Transformers Effective for Time Series Forecasting? [^17]                  |   2023   |
-|       Neural Net       |  ETSformer  |              Exponential Smoothing Transformers for Time-series Forecasting [^19]               |   2023   |
-|       Neural Net       |  FEDformer  |        Frequency Enhanced Decomposed Transformer for Long-term Series Forecasting [^20]         |   2022   |
-|       Neural Net       |  Informer   |          Beyond Efficient Transformer for Long Sequence Time-Series Forecasting [^21]           |   2021   |
-|       Neural Net       | Autoformer  |     Decomposition Transformers with Auto-Correlation for Long-Term Series Forecasting [^15]     |   2021   |
-|       Neural Net       |    CSDI     |     Conditional Score-based Diffusion Models for Probabilistic Time Series Imputation [^12]     |   2021   |
-|       Neural Net       |   US-GAN    |                 Unsupervised GAN for Multivariate Time Series Imputation [^10]                  |   2021   |
-|       Neural Net       |   GP-VAE    |                         Gaussian Process Variational Autoencoder [^11]                          |   2020   |
-|       Neural Net       |    BRITS    |                     Bidirectional Recurrent Imputation for Time Series [^3]                     |   2018   |
-|       Neural Net       |    M-RNN    |                         Multi-directional Recurrent Neural Network [^9]                         |   2019   |
-|         Naive          |  LOCF/NOCB  |              Last Observation Carried Forward / Next Observation Carried Backward               |    -     |
-|         Naive          |   Median    |                                     Median Value Imputation                                     |    -     |
-|         Naive          |    Mean     |                                      Mean Value Imputation                                      |    -     |
-| ***`Classification`*** |     🚥      |                                               🚥                                                |    🚥    |
-|        **Type**        |  **Abbr.**  |                           **Full name of the algorithm/model/paper**                            | **Year** |
-|       Neural Net       |    BRITS    |                     Bidirectional Recurrent Imputation for Time Series [^3]                     |   2018   |
-|       Neural Net       |    GRU-D    |         Recurrent Neural Networks for Multivariate Time Series with Missing Values [^4]         |   2018   |
-|       Neural Net       |  Raindrop   |           Graph-Guided Network for Irregularly Sampled Multivariate Time Series [^5]            |   2022   |
-|   ***`Clustering`***   |     🚥      |                                               🚥                                                |    🚥    |
-|        **Type**        |  **Abbr.**  |                           **Full name of the algorithm/model/paper**                            | **Year** |
-|       Neural Net       |    CRLI     |             Clustering Representation Learning on Incomplete time-series data [^6]              |   2021   |
-|       Neural Net       |    VaDER    |                         Variational Deep Embedding with Recurrence [^7]                         |   2019   |
-|  ***`Forecasting`***   |     🚥      |                                               🚥                                                |    🚥    |
-|        **Type**        |  **Abbr.**  |                           **Full name of the algorithm/model/paper**                            | **Year** |
-|     Probabilistic      |    BTTF     |                           Bayesian Temporal Tensor Factorization [^8]                           |   2021   |
-
-
 ## ❖ Citing PyPOTS
 > [!TIP]
 > **[Updates in Feb 2024]** 😎 Our survey paper [Deep Learning for Multivariate Time Series Imputation: A Survey](https://arxiv.org/abs/2402.04059) has been released on arXiv.
 The code is open source in the GitHub repo [Awesome_Imputation](https://github.com/WenjieDu/Awesome_Imputation).
 We comprehensively review the literature of the state-of-the-art deep-learning imputation methods for time series,
 provide a taxonomy for them, and discuss the challenges and future directions in this field.
 >
@@ -372,14 +383,17 @@
 [^15]: Wu, H., Xu, J., Wang, J., & Long, M. (2021). [Autoformer: Decomposition transformers with auto-correlation for long-term series forecasting](https://proceedings.neurips.cc/paper/2021/hash/bcc0d400288793e8bdcd7c19a8ac0c2b-Abstract.html). *NeurIPS 2021*.
 [^16]: Zhang, Y., & Yan, J. (2023). [Crossformer: Transformer utilizing cross-dimension dependency for multivariate time series forecasting](https://openreview.net/forum?id=vSVLM2j9eie). *ICLR 2023*.
 [^17]: Zeng, A., Chen, M., Zhang, L., & Xu, Q. (2023). [Are transformers effective for time series forecasting?](https://ojs.aaai.org/index.php/AAAI/article/view/26317). *AAAI 2023*
 [^18]: Nie, Y., Nguyen, N. H., Sinthong, P., & Kalagnanam, J. (2023). [A time series is worth 64 words: Long-term forecasting with transformers](https://openreview.net/forum?id=Jbdc0vTOcol). *ICLR 2023*
 [^19]: Woo, G., Liu, C., Sahoo, D., Kumar, A., & Hoi, S. (2023). [ETSformer: Exponential Smoothing Transformers for Time-series Forecasting](https://openreview.net/forum?id=5m_3whfo483).  *ICLR 2023*
 [^20]: Zhou, T., Ma, Z., Wen, Q., Wang, X., Sun, L., & Jin, R. (2022). [FEDformer: Frequency enhanced decomposed transformer for long-term series forecasting](https://proceedings.mlr.press/v162/zhou22g.html). *ICML 2022*.
 [^21]: Zhou, H., Zhang, S., Peng, J., Zhang, S., Li, J., Xiong, H., & Zhang, W. (2021). [Informer: Beyond efficient transformer for long sequence time-series forecasting](https://ojs.aaai.org/index.php/AAAI/article/view/17325). *AAAI 2021*.
+[^22]: Zhou, T., Ma, Z., Wen, Q., Sun, L., Yao, T., Yin, W., & Jin, R. (2022). [FiLM: Frequency improved Legendre Memory Model for Long-term Time Series Forecasting](https://proceedings.neurips.cc/paper_files/paper/2022/hash/524ef58c2bd075775861234266e5e020-Abstract-Conference.html). *NeurIPS 2022*.
+[^23]: Yi, K., Zhang, Q., Fan, W., Wang, S., Wang, P., He, H., An, N., Lian, D., Cao, L., & Niu, Z. (2024). [Frequency-domain MLPs are More Effective Learners in Time Series Forecasting](https://proceedings.neurips.cc/paper_files/paper/2023/hash/f1d16af76939f476b5f040fd1398c0a3-Abstract-Conference.html). *NeurIPS 2024*.
+[^24]: Liu, Y., Hu, T., Zhang, H., Wu, H., Wang, S., Ma, L., & Long, M. (2024). [iTransformer: Inverted Transformers Are Effective for Time Series Forecasting](https://openreview.net/forum?id=JePfAI8fah). *ICLR 2024*.
 
 
 
 <details>
 <summary>🏠 Visits</summary>
 <a href="https://github.com/WenjieDu/PyPOTS">
     <img alt="PyPOTS visits" align="left" src="https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fgithub.com%2FPyPOTS%2FPyPOTS&count_bg=%23009A0A&title_bg=%23555555&icon=&icon_color=%23E7E7E7&title=Visits%20since%20May%202022&edge_flat=false">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pypots Version: 0.4.1 Summary: A Python Toolbox for
+Metadata-Version: 2.1 Name: pypots Version: 0.5 Summary: A Python Toolbox for
 Data Mining on Partially-Observed Time Series Home-page: https://pypots.com/
 Author: Wenjie Du Author-email: wenjay.du@gmail.com License: BSD-3-Clause
 Project-URL: Documentation, https://docs.pypots.com/ Project-URL: Source,
 https://github.com/WenjieDu/PyPOTS/ Project-URL: Tracker, https://github.com/
 WenjieDu/PyPOTS/issues/ Project-URL: Download, https://github.com/WenjieDu/
 PyPOTS/archive/main.zip Keywords: data science,data mining,neural
 networks,machine learning,deep learning,artificial intelligence,time-series
@@ -25,15 +25,15 @@
 Provides-Extra: test Provides-Extra: doc Provides-Extra: dev License-File:
 LICENSE_[_h_t_t_p_s_:_/_/_p_y_p_o_t_s_._c_o_m_/_f_i_g_s_/_p_y_p_o_t_s___l_o_g_o_s_/_P_y_P_O_T_S_/_l_o_g_o___F_F_B_G_._s_v_g_]
                           ******** WWeellccoommee ttoo PPyyPPOOTTSS ********
     a Python toolbox for machine learning on Partially-Observed Time Series
 _[_P_y_t_h_o_n_ _v_e_r_s_i_o_n_]_[_p_o_w_e_r_e_d_ _b_y_ _P_y_t_o_r_c_h_]_[_t_h_e_ _l_a_t_e_s_t_ _r_e_l_e_a_s_e_ _v_e_r_s_i_o_n_]_[_B_S_D_-_3_ _l_i_c_e_n_s_e_]
   _[_C_o_m_m_u_n_i_t_y_]_[_G_i_t_H_u_b_ _c_o_n_t_r_i_b_u_t_o_r_s_]_[_G_i_t_H_u_b_ _R_e_p_o_ _s_t_a_r_s_]_[_G_i_t_H_u_b_ _R_e_p_o_ _f_o_r_k_s_]_[_C_o_d_e
   _C_l_i_m_a_t_e_ _m_a_i_n_t_a_i_n_a_b_i_l_i_t_y_]_[_C_o_v_e_r_a_l_l_s_ _c_o_v_e_r_a_g_e_]_[_G_i_t_H_u_b_ _T_e_s_t_i_n_g_]_[_D_o_c_s_ _b_u_i_l_d_i_n_g_]
-                 _[_C_o_n_d_a_ _d_o_w_n_l_o_a_d_s_]_[_P_y_P_I_ _d_o_w_n_l_o_a_d_s_]_[_a_r_X_i_v_ _D_O_I_]
+        _[_C_o_n_d_a_ _d_o_w_n_l_o_a_d_s_]_[_P_y_P_I_ _d_o_w_n_l_o_a_d_s_]_[_a_r_X_i_v_ _D_O_I_]_[_R_E_A_D_M_E_ _i_n_ _C_h_i_n_e_s_e_]
 â¦¿ `Motivation`: Due to all kinds of reasons like failure of collection
 sensors, communication error, and unexpected malfunction, missing values are
 common to see in time series from the real-world environment. This makes
 partially-observed time series (POTS) a pervasive problem in open-world
 modeling and prevents advanced data analysis. Although this problem is
 important, the area of machine learning on POTS still lacks a dedicated
 toolkit. PyPOTS is created to fill in this blank. â¦¿ `Mission`: PyPOTS
@@ -45,150 +45,144 @@
 partially-observed multivariate time series. For sure, besides various
 algorithms, PyPOTS is going to have unified APIs together with detailed
 documentation and interactive examples across algorithms as tutorials. ð¤
 **Please** star this repo to help others notice PyPOTS if you think it is a
 useful toolkit. **Please** properly [cite PyPOTS](https://github.com/WenjieDu/
 PyPOTS#-citing-pypots) in your publications if it helps with your research.
 This really means a lot to our open-source research. Thank you! The rest of
-this readme file is organized as follows: [**â PyPOTS Ecosystem**](#-pypots-
-ecosystem), [**â Installation**](#-installation), [**â Usage**](#-usage),
-[**â Available Algorithms**](#-available-algorithms), [**â Citing PyPOTS**]
-(#-citing-pypots), [**â Contribution**](#-contribution), [**â Community**]
-(#-community). ## â PyPOTS Ecosystem At PyPOTS, things are related to coffee,
-which we're familiar with. Yes, this is a coffee universe! As you can see,
-there is a coffee pot in the PyPOTS logo. And what else? Please read on ;-)
-_[_T_S_D_B_ _l_o_g_o_]ð Time series datasets are taken as coffee beans at PyPOTS, and
-POTS datasets are incomplete coffee beans with missing parts that have their
-own meanings. To make various public time-series datasets readily available to
-users, Time Series Data Beans (TSDB) is created to make loading time-series
-datasets super easy! Visit [TSDB](https://github.com/WenjieDu/TSDB) right now
-to know more about this handy tool ð , and it now supports a total of 168
-open-source datasets! _[_P_y_G_r_i_n_d_e_r_ _l_o_g_o_]ð To simulate the real-world data
-beans with missingness, the ecosystem library [PyGrinder](https://github.com/
-WenjieDu/PyGrinder), a toolkit helping grind your coffee beans into incomplete
-ones, is created. Missing patterns fall into three categories according to
-Robin's theory[^13]: MCAR (missing completely at random), MAR (missing at
-random), and MNAR (missing not at random). PyGrinder supports all of them and
-additional functionalities related to missingness. With PyGrinder, you can
-introduce synthetic missing values into your datasets with a single line of
-code. _[_B_r_e_w_P_O_T_S_ _l_o_g_o_]ð Now we have the beans, the grinder, and the pot, how
-to brew us a cup of coffee? Tutorials are necessary! Considering the future
-workload, PyPOTS tutorials are released in a single repo, and you can find them
-in [BrewPOTS](https://github.com/WenjieDu/BrewPOTS). Take a look at it now, and
-learn how to brew your POTS datasets!
+this readme file is organized as follows: [**â Available Algorithms**](#-
+available-algorithms), [**â PyPOTS Ecosystem**](#-pypots-ecosystem), [**â
+Installation**](#-installation), [**â Usage**](#-usage), [**â Citing
+PyPOTS**](#-citing-pypots), [**â Contribution**](#-contribution), [**â
+Community**](#-community). ## â Available Algorithms PyPOTS supports
+imputation, classification, clustering, forecasting, and anomaly detection
+tasks on multivariate partially-observed time series with missing values. The
+table below shows the availability of each algorithm (sorted by Year) in PyPOTS
+for different tasks. The symbol â indicates the algorithm is available for
+the corresponding task (note that models will be continuously updated in the
+future to handle tasks that are not currently supported. Stay tunedâï¸).
+ð Since **v0.2**, all neural-network models in PyPOTS has got
+hyperparameter-optimization support. This functionality is implemented with the
+[Microsoft NNI](https://github.com/microsoft/nni) framework. You may want to
+refer to our time-series imputation survey repo [Awesome_Imputation](https://
+github.com/WenjieDu/Awesome_Imputation) to see how to config and tune the
+hyperparameters. ð¥ Note that Transformer, iTransformer, FreTS, Crossformer,
+PatchTST, DLinear, ETSformer, FiLM, FEDformer, Informer, Autoformer are not
+proposed as imputation methods in their original papers, and they cannot accept
+POTS as input. **To make them applicable on POTS data, we apply the embedding
+strategy and training approach (ORT+MIT) the same as we did in [SAITS paper]
+(https://arxiv.org/pdf/2202.08516).** The task types are abbreviated as
+follows: **`IMPU`**: Imputation; **`FORE`**: Forecasting; **`CLAS`**:
+Classification; **`CLUS`**: Clustering; **`ANOD`**: Anomaly Detection. The
+paper references and links are all listed at the bottom of this file. |
+**Type** | **Algo** | **IMPU** | **FORE** | **CLAS** | **CLUS** | **ANOD** |
+**Year - Venue** | |:--------------|:-----------------------------------|:-----
+---:|:--------:|:--------:|:--------:|:--------:|:-----------------| | Neural
+Net | iTransformer[^24] | â | | | | | 2024 - ICLR | | Neural Net | FreTS[^23]
+| â | | | | | 2024 - NeurIPS | | Neural Net | SAITS[^1] | â | | | | | 2023
+- ESWA | | Neural Net | Crossformer[^16] | â | | | | | 2023 - ICLR | | Neural
+Net | TimesNet[^14] | â | | | | | 2023 - ICLR | | Neural Net | PatchTST[^18]
+| â | | | | | 2023 - ICLR | | Neural Net | ETSformer[^19] | â | | | | |
+2023 - ICLR | | Neural Net | DLinear[^17] | â | | | | | 2023 - AAAI | |
+Neural Net | FiLM[^22] | â | | | | | 2022 - NeurIPS | | Neural Net | Raindrop
+[^5] | | | â | | | 2022 - ICLR | | Neural Net | FEDformer[^20] | â | | | |
+| 2022 - ICML | | Neural Net | Autoformer[^15] | â | | | | | 2021 - NeurIPS |
+| Neural Net | CSDI[^12] | â | â | | | | 2021 - NeurIPS | | Neural Net |
+Informer[^21] | â | | | | | 2021 - AAAI | | Neural Net | US-GAN[^10] | â |
+| | | | 2021 - AAAI | | Neural Net | CRLI[^6] | | | | â | | 2021 - AAAI | |
+Probabilistic | BTTF[^8] | | â | | | | 2021 - TPAMI | | Neural Net | GP-VAE
+[^11] | â | | | | | 2020 - AISTATS | | Neural Net | VaDER[^7] | | | | â | |
+2019 - GigaSci. | | Neural Net | M-RNN[^9] | â | | | | | 2019 - TBME | |
+Neural Net | BRITS[^3] | â | | â | | | 2018 - NeurIPS | | Neural Net | GRU-
+D[^4] | â | | â | | | 2018 - Sci. Rep. | | Neural Net | Transformer[^2] |
+â | | | | | 2017 - NeurIPS | | Naive | LOCF/NOCB | â | | | | | | | Naive |
+Mean | â | | | | | | | Naive | Median | â | | | | | | ## â PyPOTS
+Ecosystem At PyPOTS, things are related to coffee, which we're familiar with.
+Yes, this is a coffee universe! As you can see, there is a coffee pot in the
+PyPOTS logo. And what else? Please read on ;-) _[_T_S_D_B_ _l_o_g_o_]ð Time series
+datasets are taken as coffee beans at PyPOTS, and POTS datasets are incomplete
+coffee beans with missing parts that have their own meanings. To make various
+public time-series datasets readily available to users, Time Series Data Beans
+(TSDB) is created to make loading time-series datasets super easy! Visit [TSDB]
+(https://github.com/WenjieDu/TSDB) right now to know more about this handy tool
+ð , and it now supports a total of 169 open-source datasets! _[_P_y_G_r_i_n_d_e_r
+_l_o_g_o_]ð To simulate the real-world data beans with missingness, the ecosystem
+library [PyGrinder](https://github.com/WenjieDu/PyGrinder), a toolkit helping
+grind your coffee beans into incomplete ones, is created. Missing patterns fall
+into three categories according to Robin's theory[^13]: MCAR (missing
+completely at random), MAR (missing at random), and MNAR (missing not at
+random). PyGrinder supports all of them and additional functionalities related
+to missingness. With PyGrinder, you can introduce synthetic missing values into
+your datasets with a single line of code. _[_B_r_e_w_P_O_T_S_ _l_o_g_o_]ð Now we have the
+beans, the grinder, and the pot, how to brew us a cup of coffee? Tutorials are
+necessary! Considering the future workload, PyPOTS tutorials are released in a
+single repo, and you can find them in [BrewPOTS](https://github.com/WenjieDu/
+BrewPOTS). Take a look at it now, and learn how to brew your POTS datasets!
 _[_h_t_t_p_s_:_/_/_p_y_p_o_t_s_._c_o_m_/_f_i_g_s_/_p_y_p_o_t_s___l_o_g_o_s_/_E_c_o_s_y_s_t_e_m_/_P_y_P_O_T_S___E_c_o_s_y_s_t_e_m___P_i_p_e_l_i_n_e_._p_n_g_]
        ?â???ï?¸? WWeellccoommee ttoo tthhee uunniivveerrssee ooff PPyyPPOOTTSS.. EEnnjjooyy iitt aanndd hhaavvee ffuunn!!
 ## â Installation You can refer to [the installation instruction](https://
 docs.pypots.com/en/latest/install.html) in PyPOTS documentation for a guideline
 with more details. PyPOTS is available on both [PyPI](https://pypi.python.org/
 pypi/pypots) and [Anaconda](https://anaconda.org/conda-forge/pypots). You can
-install PyPOTS as shown below: ``` bash # via pip pip install pypots # the
-first time installation pip install pypots --upgrade # update pypots to the
-latest version # install from the latest source code with the latest features
-but may be not officially released yet pip install https://github.com/WenjieDu/
-PyPOTS/archive/main.zip # via conda conda install -c conda-forge pypots # the
-first time installation conda update -c conda-forge pypots # update pypots to
-the latest version ``` ## â Usage Besides [BrewPOTS](https://github.com/
-WenjieDu/BrewPOTS), you can also find a simple and quick-start tutorial
-notebook on Google Colab _[_C_o_l_a_b_ _t_u_t_o_r_i_a_l_s_]. If you have further questions,
-please refer to PyPOTS documentation [docs.pypots.com](https://
+install PyPOTS like below as well as TSDB and PyGrinder: ``` bash # via pip pip
+install pypots # the first time installation pip install pypots --upgrade #
+update pypots to the latest version # install from the latest source code with
+the latest features but may be not officially released yet pip install https://
+github.com/WenjieDu/PyPOTS/archive/main.zip # via conda conda install -c conda-
+forge pypots # the first time installation conda update -c conda-forge pypots #
+update pypots to the latest version ``` ## â Usage Besides [BrewPOTS](https:/
+/github.com/WenjieDu/BrewPOTS), you can also find a simple and quick-start
+tutorial notebook on Google Colab _[_C_o_l_a_b_ _t_u_t_o_r_i_a_l_s_]. If you have further
+questions, please refer to PyPOTS documentation [docs.pypots.com](https://
 docs.pypots.com). You can also [raise an issue](https://github.com/WenjieDu/
 PyPOTS/issues) or [ask in our community](#-community). We present you a usage
 example of imputing missing values in time series with PyPOTS below, you can
 click it to view. CClliicckk hheerree ttoo sseeee aann eexxaammppllee aappppllyyiinngg SSAAIITTSS oonn PPhhyyssiiooNNeett22001122
-ffoorr iimmppuuttaattiioonn:: ``` python import numpy as np from sklearn.preprocessing import
-StandardScaler from pygrinder import mcar from pypots.data import
-load_specific_dataset from pypots.imputation import SAITS from
-pypots.utils.metrics import calc_mae # Data preprocessing. Tedious, but PyPOTS
-can help. data = load_specific_dataset('physionet_2012') # PyPOTS will
-automatically download and extract it. X = data['X'] num_samples = len(X
-['RecordID'].unique()) X = X.drop(['RecordID', 'Time'], axis = 1) X =
-StandardScaler().fit_transform(X.to_numpy()) X = X.reshape(num_samples, 48, -1)
-X_ori = X # keep X_ori for validation X = mcar(X, 0.1) # randomly hold out 10%
-observed values as ground truth dataset = {"X": X} # X for model input print
-(X.shape) # (11988, 48, 37), 11988 samples and each sample has 48 time steps,
-37 features # Model training. This is PyPOTS showtime. saits = SAITS
-(n_steps=48, n_features=37, n_layers=2, d_model=256, d_ffn=128, n_heads=4,
-d_k=64, d_v=64, dropout=0.1, epochs=10) # Here I use the whole dataset as the
-training set because ground truth is not visible to the model, you can also
-split it into train/val/test sets saits.fit(dataset) imputation = saits.impute
-(dataset) # impute the originally-missing values and artificially-missing
-values indicating_mask = np.isnan(X) ^ np.isnan(X_ori) # indicating mask for
-imputation error calculation mae = calc_mae(imputation, np.nan_to_num(X_ori),
-indicating_mask) # calculate mean absolute error on the ground truth
-(artificially-missing values) ``` ## â Available Algorithms PyPOTS supports
-imputation, classification, clustering, and forecasting tasks on multivariate
-time series with missing values. The currently available algorithms of four
-tasks are cataloged in the following table with four partitions. The paper
-references are all listed at the bottom of this readme file. ð Since
-**v0.2**, all neural-network models in PyPOTS has got hyperparameter-
-optimization support. This functionality is implemented with the [Microsoft
-NNI](https://github.com/microsoft/nni) framework. ð¥ Note that Transformer,
-Crossformer, PatchTST, DLinear, ETSformer, FEDformer, Informer, Autoformer are
-not proposed as imputation methods in their original papers, and they cannot
-accept POTS as input. **To make them applicable on POTS data, we apply the
-embedding strategy and training approach (ORT+MIT) the same as we did in [SAITS
-paper](https://arxiv.org/pdf/2202.08516).** | ***`Imputation`*** | ð¥ | ð¥
-| ð¥ | |:----------------------:|:-----------:|:-----------------------------
-------------------------------------------------------------------:|:--------:
-| | **Type** | **Abbr.** | **Full name of the algorithm/model** | **Year** | |
-Neural Net | SAITS | Self-Attention-based Imputation for Time Series [^1] |
-2023 | | Neural Net | Transformer | Attention is All you Need [^2] | 2017 | |
-Neural Net | Crossformer | Transformer Utilizing Cross-Dimension Dependency for
-Multivariate Time Series Forecasting [^16] | 2023 | | Neural Net | TimesNet |
-Temporal 2D-Variation Modeling for General Time Series Analysis [^14] | 2023 |
-| Neural Net | PatchTST | A Time Series is Worth 64 Words: Long-Term
-Forecasting with Transformers [^18] | 2023 | | Neural Net | DLinear | Are
-Transformers Effective for Time Series Forecasting? [^17] | 2023 | | Neural Net
-| ETSformer | Exponential Smoothing Transformers for Time-series Forecasting
-[^19] | 2023 | | Neural Net | FEDformer | Frequency Enhanced Decomposed
-Transformer for Long-term Series Forecasting [^20] | 2022 | | Neural Net |
-Informer | Beyond Efficient Transformer for Long Sequence Time-Series
-Forecasting [^21] | 2021 | | Neural Net | Autoformer | Decomposition
-Transformers with Auto-Correlation for Long-Term Series Forecasting [^15] |
-2021 | | Neural Net | CSDI | Conditional Score-based Diffusion Models for
-Probabilistic Time Series Imputation [^12] | 2021 | | Neural Net | US-GAN |
-Unsupervised GAN for Multivariate Time Series Imputation [^10] | 2021 | |
-Neural Net | GP-VAE | Gaussian Process Variational Autoencoder [^11] | 2020 | |
-Neural Net | BRITS | Bidirectional Recurrent Imputation for Time Series [^3] |
-2018 | | Neural Net | M-RNN | Multi-directional Recurrent Neural Network [^9] |
-2019 | | Naive | LOCF/NOCB | Last Observation Carried Forward / Next
-Observation Carried Backward | - | | Naive | Median | Median Value Imputation |
-- | | Naive | Mean | Mean Value Imputation | - | | ***`Classification`*** |
-ð¥ | ð¥ | ð¥ | | **Type** | **Abbr.** | **Full name of the algorithm/
-model/paper** | **Year** | | Neural Net | BRITS | Bidirectional Recurrent
-Imputation for Time Series [^3] | 2018 | | Neural Net | GRU-D | Recurrent
-Neural Networks for Multivariate Time Series with Missing Values [^4] | 2018 |
-| Neural Net | Raindrop | Graph-Guided Network for Irregularly Sampled
-Multivariate Time Series [^5] | 2022 | | ***`Clustering`*** | ð¥ | ð¥ |
-ð¥ | | **Type** | **Abbr.** | **Full name of the algorithm/model/paper** |
-**Year** | | Neural Net | CRLI | Clustering Representation Learning on
-Incomplete time-series data [^6] | 2021 | | Neural Net | VaDER | Variational
-Deep Embedding with Recurrence [^7] | 2019 | | ***`Forecasting`*** | ð¥ |
-ð¥ | ð¥ | | **Type** | **Abbr.** | **Full name of the algorithm/model/
-paper** | **Year** | | Probabilistic | BTTF | Bayesian Temporal Tensor
-Factorization [^8] | 2021 | ## â Citing PyPOTS > [!TIP] > **[Updates in Feb
-2024]** ð Our survey paper [Deep Learning for Multivariate Time Series
-Imputation: A Survey](https://arxiv.org/abs/2402.04059) has been released on
-arXiv. The code is open source in the GitHub repo [Awesome_Imputation](https://
-github.com/WenjieDu/Awesome_Imputation). We comprehensively review the
-literature of the state-of-the-art deep-learning imputation methods for time
-series, provide a taxonomy for them, and discuss the challenges and future
-directions in this field. > > **[Updates in Jun 2023]** ð A short version of
-the PyPOTS paper is accepted by the 9th SIGKDD international workshop on Mining
-and Learning from Time Series ([MiLeTS'23](https://kdd-milets.github.io/
-milets2023/))). **Additionally**, PyPOTS has been included as a [PyTorch
-Ecosystem](https://pytorch.org/ecosystem/) project. The paper introducing
-PyPOTS is available on arXiv at [this URL](https://arxiv.org/abs/2305.18811),
-and we are pursuing to publish it in prestigious academic venues, e.g. JMLR
-(track for [Machine Learning Open Source Software](https://www.jmlr.org/mloss/
-)). If you use PyPOTS in your work, please cite it as below and ðstar this
-repository to make others notice this library. ð¤ There are scientific
-research projects using PyPOTS and referencing in their papers. Here is [an
-incomplete list of them](https://scholar.google.com/
+ffoorr iimmppuuttaattiioonn:: ``` python # Data preprocessing. Tedious, but PyPOTS can help.
+import numpy as np from sklearn.preprocessing import StandardScaler from
+pygrinder import mcar from pypots.data import load_specific_dataset data =
+load_specific_dataset('physionet_2012') # PyPOTS will automatically download
+and extract it. X = data['X'] num_samples = len(X['RecordID'].unique()) X =
+X.drop(['RecordID', 'Time'], axis = 1) X = StandardScaler().fit_transform
+(X.to_numpy()) X = X.reshape(num_samples, 48, -1) X_ori = X # keep X_ori for
+validation X = mcar(X, 0.1) # randomly hold out 10% observed values as ground
+truth dataset = {"X": X} # X for model input print(X.shape) # (11988, 48, 37),
+11988 samples and each sample has 48 time steps, 37 features # Model training.
+This is PyPOTS showtime. from pypots.imputation import SAITS from
+pypots.utils.metrics import calc_mae saits = SAITS(n_steps=48, n_features=37,
+n_layers=2, d_model=256, n_heads=4, d_k=64, d_v=64, d_ffn=128, dropout=0.1,
+epochs=10) # Here I use the whole dataset as the training set because ground
+truth is not visible to the model, you can also split it into train/val/test
+sets saits.fit(dataset) # train the model on the dataset imputation =
+saits.impute(dataset) # impute the originally-missing values and artificially-
+missing values indicating_mask = np.isnan(X) ^ np.isnan(X_ori) # indicating
+mask for imputation error calculation mae = calc_mae(imputation, np.nan_to_num
+(X_ori), indicating_mask) # calculate mean absolute error on the ground truth
+(artificially-missing values) saits.save("save_it_here/
+saits_physionet2012.pypots") # save the model for future use saits.load
+("save_it_here/saits_physionet2012.pypots") # reload the serialized model file
+for following imputation or training ``` ## â Citing PyPOTS > [!TIP] > **
+[Updates in Feb 2024]** ð Our survey paper [Deep Learning for Multivariate
+Time Series Imputation: A Survey](https://arxiv.org/abs/2402.04059) has been
+released on arXiv. The code is open source in the GitHub repo
+[Awesome_Imputation](https://github.com/WenjieDu/Awesome_Imputation). We
+comprehensively review the literature of the state-of-the-art deep-learning
+imputation methods for time series, provide a taxonomy for them, and discuss
+the challenges and future directions in this field. > > **[Updates in Jun
+2023]** ð A short version of the PyPOTS paper is accepted by the 9th SIGKDD
+international workshop on Mining and Learning from Time Series ([MiLeTS'23]
+(https://kdd-milets.github.io/milets2023/))). **Additionally**, PyPOTS has been
+included as a [PyTorch Ecosystem](https://pytorch.org/ecosystem/) project. The
+paper introducing PyPOTS is available on arXiv at [this URL](https://arxiv.org/
+abs/2305.18811), and we are pursuing to publish it in prestigious academic
+venues, e.g. JMLR (track for [Machine Learning Open Source Software](https://
+www.jmlr.org/mloss/)). If you use PyPOTS in your work, please cite it as below
+and ðstar this repository to make others notice this library. ð¤ There are
+scientific research projects using PyPOTS and referencing in their papers. Here
+is [an incomplete list of them](https://scholar.google.com/
 scholar?as_ylo=2022&q=%E2%80%9CPyPOTS%E2%80%9D&hl=en>). ``` bibtex @article
 {du2023pypots, title={{PyPOTS: a Python toolbox for data mining on Partially-
 Observed Time Series}}, author={Wenjie Du}, year={2023}, eprint={2305.18811},
 archivePrefix={arXiv}, primaryClass={cs.LG}, url={https://arxiv.org/abs/
 2305.18811}, doi={10.48550/arXiv.2305.18811}, } ``` or > Wenjie Du. (2023). >
 PyPOTS: a Python toolbox for data mining on Partially-Observed Time Series. >
 arXiv, abs/2305.18811.https://arxiv.org/abs/2305.18811 ## â Contribution
@@ -276,9 +270,20 @@
 Exponential Smoothing Transformers for Time-series Forecasting](https://
 openreview.net/forum?id=5m_3whfo483). *ICLR 2023* [^20]: Zhou, T., Ma, Z., Wen,
 Q., Wang, X., Sun, L., & Jin, R. (2022). [FEDformer: Frequency enhanced
 decomposed transformer for long-term series forecasting](https://
 proceedings.mlr.press/v162/zhou22g.html). *ICML 2022*. [^21]: Zhou, H., Zhang,
 S., Peng, J., Zhang, S., Li, J., Xiong, H., & Zhang, W. (2021). [Informer:
 Beyond efficient transformer for long sequence time-series forecasting](https:/
-/ojs.aaai.org/index.php/AAAI/article/view/17325). *AAAI 2021*. ð  Visits
-_[_P_y_P_O_T_S_ _v_i_s_i_t_s_]
+/ojs.aaai.org/index.php/AAAI/article/view/17325). *AAAI 2021*. [^22]: Zhou, T.,
+Ma, Z., Wen, Q., Sun, L., Yao, T., Yin, W., & Jin, R. (2022). [FiLM: Frequency
+improved Legendre Memory Model for Long-term Time Series Forecasting](https://
+proceedings.neurips.cc/paper_files/paper/2022/hash/
+524ef58c2bd075775861234266e5e020-Abstract-Conference.html). *NeurIPS 2022*.
+[^23]: Yi, K., Zhang, Q., Fan, W., Wang, S., Wang, P., He, H., An, N., Lian,
+D., Cao, L., & Niu, Z. (2024). [Frequency-domain MLPs are More Effective
+Learners in Time Series Forecasting](https://proceedings.neurips.cc/
+paper_files/paper/2023/hash/f1d16af76939f476b5f040fd1398c0a3-Abstract-
+Conference.html). *NeurIPS 2024*. [^24]: Liu, Y., Hu, T., Zhang, H., Wu, H.,
+Wang, S., Ma, L., & Long, M. (2024). [iTransformer: Inverted Transformers Are
+Effective for Time Series Forecasting](https://openreview.net/
+forum?id=JePfAI8fah). *ICLR 2024*. ð  Visits_[_P_y_P_O_T_S_ _v_i_s_i_t_s_]
```

### Comparing `pypots-0.4.1/README.md` & `pypots-0.5/pypots.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,45 @@
+Metadata-Version: 2.1
+Name: pypots
+Version: 0.5
+Summary: A Python Toolbox for Data Mining on Partially-Observed Time Series
+Home-page: https://pypots.com/
+Author: Wenjie Du
+Author-email: wenjay.du@gmail.com
+License: BSD-3-Clause
+Project-URL: Documentation, https://docs.pypots.com/
+Project-URL: Source, https://github.com/WenjieDu/PyPOTS/
+Project-URL: Tracker, https://github.com/WenjieDu/PyPOTS/issues/
+Project-URL: Download, https://github.com/WenjieDu/PyPOTS/archive/main.zip
+Keywords: data science,data mining,neural networks,machine learning,deep learning,artificial intelligence,time-series analysis,time series,imputation,interpolation,classification,clustering,forecasting,partially observed,irregular sampled,partially-observed time series,incomplete time series,missing data,missing values
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Education
+Classifier: Intended Audience :: Science/Research
+Classifier: Intended Audience :: Healthcare Industry
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
+Requires-Python: >=3.7.0
+Description-Content-Type: text/markdown
+Provides-Extra: basic
+Provides-Extra: optional
+Provides-Extra: full
+Provides-Extra: test
+Provides-Extra: doc
+Provides-Extra: dev
+License-File: LICENSE
+
 <a href="https://github.com/WenjieDu/PyPOTS">
     <img src="https://pypots.com/figs/pypots_logos/PyPOTS/logo_FFBG.svg" width="200" align="right">
 </a>
 
 <h3 align="center">Welcome to PyPOTS</h3>
 
 <p align="center"><i>a Python toolbox for machine learning on Partially-Observed Time Series</i></p>
@@ -48,14 +86,17 @@
     </a>
     <a href="https://pepy.tech/project/pypots">
         <img alt="PyPI downloads" src="https://img.shields.io/endpoint?url=https://pypots.com/figs/downloads_badges/pypi_pypots_downloads.json">
     </a>
     <a href="https://arxiv.org/abs/2305.18811">
         <img alt="arXiv DOI" src="https://img.shields.io/badge/DOI-10.48550/arXiv.2305.18811-F8F7F0">
     </a>
+    <a href="https://github.com/WenjieDu/PyPOTS/blob/main/README_zh.md">
+        <img alt="README in Chinese" src="https://img.shields.io/badge/README-🇨🇳中文版-FCEFE8">
+    </a>
 </p>
 
 ⦿ `Motivation`: Due to all kinds of reasons like failure of collection sensors, communication error,
 and unexpected malfunction, missing values are common to see in time series from the real-world environment.
 This makes partially-observed time series (POTS) a pervasive problem in open-world modeling and prevents advanced
 data analysis. Although this problem is important, the area of machine learning on POTS still lacks a dedicated toolkit.
 PyPOTS is created to fill in this blank.
@@ -67,36 +108,90 @@
 have unified APIs together with detailed documentation and interactive examples across algorithms as tutorials.
 
 🤗 **Please** star this repo to help others notice PyPOTS if you think it is a useful toolkit.
 **Please** properly [cite PyPOTS](https://github.com/WenjieDu/PyPOTS#-citing-pypots) in your publications
 if it helps with your research. This really means a lot to our open-source research. Thank you!
 
 The rest of this readme file is organized as follows:
+[**❖ Available Algorithms**](#-available-algorithms),
 [**❖ PyPOTS Ecosystem**](#-pypots-ecosystem),
 [**❖ Installation**](#-installation),
 [**❖ Usage**](#-usage),
-[**❖ Available Algorithms**](#-available-algorithms),
 [**❖ Citing PyPOTS**](#-citing-pypots),
 [**❖ Contribution**](#-contribution),
 [**❖ Community**](#-community).
 
 
+## ❖ Available Algorithms
+PyPOTS supports imputation, classification, clustering, forecasting, and anomaly detection tasks on multivariate partially-observed
+time series with missing values. The table below shows the availability of each algorithm (sorted by Year) in PyPOTS for different tasks.
+The symbol ✅ indicates the algorithm is available for the corresponding task (note that models will be continuously updated
+in the future to handle tasks that are not currently supported. Stay tuned❗️).
+
+🌟 Since **v0.2**, all neural-network models in PyPOTS has got hyperparameter-optimization support.
+This functionality is implemented with the [Microsoft NNI](https://github.com/microsoft/nni) framework. You may want to refer to our time-series
+imputation survey repo [Awesome_Imputation](https://github.com/WenjieDu/Awesome_Imputation) to see how to config and
+tune the hyperparameters.
+
+🔥 Note that Transformer, iTransformer, FreTS, Crossformer, PatchTST, DLinear, ETSformer, FiLM, FEDformer, Informer, Autoformer
+are not proposed as imputation methods in their original papers, and they cannot accept POTS as input.
+**To make them applicable on POTS data, we apply the embedding strategy and training approach (ORT+MIT)
+the same as we did in [SAITS paper](https://arxiv.org/pdf/2202.08516).**
+
+The task types are abbreviated as follows:
+**`IMPU`**: Imputation;
+**`FORE`**: Forecasting;
+**`CLAS`**: Classification;
+**`CLUS`**: Clustering;
+**`ANOD`**: Anomaly Detection.
+The paper references and links are all listed at the bottom of this file.
+
+| **Type**      | **Algo**                           | **IMPU** | **FORE** | **CLAS** | **CLUS** | **ANOD** | **Year - Venue** |
+|:--------------|:-----------------------------------|:--------:|:--------:|:--------:|:--------:|:--------:|:-----------------|
+| Neural Net    | iTransformer[^24]                  |    ✅     |          |          |          |          | 2024 - ICLR      |
+| Neural Net    | FreTS[^23]                         |    ✅     |          |          |          |          | 2024 - NeurIPS   |
+| Neural Net    | SAITS[^1]                          |    ✅     |          |          |          |          | 2023 - ESWA      |
+| Neural Net    | Crossformer[^16]                   |    ✅     |          |          |          |          | 2023 - ICLR      |
+| Neural Net    | TimesNet[^14]                      |    ✅     |          |          |          |          | 2023 - ICLR      |
+| Neural Net    | PatchTST[^18]                      |    ✅     |          |          |          |          | 2023 - ICLR      |
+| Neural Net    | ETSformer[^19]                     |    ✅     |          |          |          |          | 2023 - ICLR      |
+| Neural Net    | DLinear[^17]                       |    ✅     |          |          |          |          | 2023 - AAAI      |
+| Neural Net    | FiLM[^22]                          |    ✅     |          |          |          |          | 2022 - NeurIPS   |
+| Neural Net    | Raindrop[^5]                       |          |          |    ✅     |          |          | 2022 - ICLR      |
+| Neural Net    | FEDformer[^20]                     |    ✅     |          |          |          |          | 2022 - ICML      |
+| Neural Net    | Autoformer[^15]                    |    ✅     |          |          |          |          | 2021 - NeurIPS   |
+| Neural Net    | CSDI[^12]                          |    ✅     |    ✅     |          |          |          | 2021 - NeurIPS   |
+| Neural Net    | Informer[^21]                      |    ✅     |          |          |          |          | 2021 - AAAI      |
+| Neural Net    | US-GAN[^10]                        |    ✅     |          |          |          |          | 2021 - AAAI      |
+| Neural Net    | CRLI[^6]                           |          |          |          |    ✅     |          | 2021 - AAAI      |
+| Probabilistic | BTTF[^8]                           |          |    ✅     |          |          |          | 2021 - TPAMI     |
+| Neural Net    | GP-VAE[^11]                        |    ✅     |          |          |          |          | 2020 - AISTATS   |
+| Neural Net    | VaDER[^7]                          |          |          |          |    ✅     |          | 2019 - GigaSci.  |
+| Neural Net    | M-RNN[^9]                          |    ✅     |          |          |          |          | 2019 - TBME      |
+| Neural Net    | BRITS[^3]                          |    ✅     |          |    ✅     |          |          | 2018 - NeurIPS   |
+| Neural Net    | GRU-D[^4]                          |    ✅     |          |    ✅     |          |          | 2018 - Sci. Rep. |
+| Neural Net    | Transformer[^2]                    |    ✅     |          |          |          |          | 2017 - NeurIPS   |
+| Naive         | LOCF/NOCB                          |    ✅     |          |          |          |          |                  |
+| Naive         | Mean                               |    ✅     |          |          |          |          |                  |
+| Naive         | Median                             |    ✅     |          |          |          |          |                  |
+
+
 ## ❖ PyPOTS Ecosystem
 At PyPOTS, things are related to coffee, which we're familiar with. Yes, this is a coffee universe!
 As you can see, there is a coffee pot in the PyPOTS logo.
 And what else? Please read on ;-)
 
 <a href="https://github.com/WenjieDu/TSDB">
     <img src="https://pypots.com/figs/pypots_logos/TSDB/logo_FFBG.svg" align="left" width="140" alt="TSDB logo"/>
 </a>
 
 👈 Time series datasets are taken as coffee beans at PyPOTS, and POTS datasets are incomplete coffee beans with missing parts that have their own meanings.
 To make various public time-series datasets readily available to users,
 <i>Time Series Data Beans (TSDB)</i> is created to make loading time-series datasets super easy!
-Visit [TSDB](https://github.com/WenjieDu/TSDB) right now to know more about this handy tool 🛠, and it now supports a total of 168 open-source datasets!
+Visit [TSDB](https://github.com/WenjieDu/TSDB) right now to know more about this handy tool 🛠, and it now supports a total of 169 open-source datasets!
 
 <a href="https://github.com/WenjieDu/PyGrinder">
     <img src="https://pypots.com/figs/pypots_logos/PyGrinder/logo_FFBG.svg" align="right" width="140" alt="PyGrinder logo"/>
 </a>
 
 👉 To simulate the real-world data beans with missingness, the ecosystem library [PyGrinder](https://github.com/WenjieDu/PyGrinder),
 a toolkit helping grind your coffee beans into incomplete ones, is created. Missing patterns fall into three categories according to Robin's theory[^13]:
@@ -122,15 +217,15 @@
 </p>
 
 
 ## ❖ Installation
 You can refer to [the installation instruction](https://docs.pypots.com/en/latest/install.html) in PyPOTS documentation for a guideline with more details.
 
 PyPOTS is available on both [PyPI](https://pypi.python.org/pypi/pypots) and [Anaconda](https://anaconda.org/conda-forge/pypots).
-You can install PyPOTS as shown below:
+You can install PyPOTS like below as well as TSDB and PyGrinder:
 
 ``` bash
 # via pip
 pip install pypots            # the first time installation
 pip install pypots --upgrade  # update pypots to the latest version
 # install from the latest source code with the latest features but may be not officially released yet
 pip install https://github.com/WenjieDu/PyPOTS/archive/main.zip
@@ -150,91 +245,45 @@
 
 We present you a usage example of imputing missing values in time series with PyPOTS below, you can click it to view.
 
 <details open>
 <summary><b>Click here to see an example applying SAITS on PhysioNet2012 for imputation:</b></summary>
 
 ``` python
+# Data preprocessing. Tedious, but PyPOTS can help.
 import numpy as np
 from sklearn.preprocessing import StandardScaler
 from pygrinder import mcar
 from pypots.data import load_specific_dataset
-from pypots.imputation import SAITS
-from pypots.utils.metrics import calc_mae
-
-# Data preprocessing. Tedious, but PyPOTS can help.
 data = load_specific_dataset('physionet_2012')  # PyPOTS will automatically download and extract it.
 X = data['X']
 num_samples = len(X['RecordID'].unique())
 X = X.drop(['RecordID', 'Time'], axis = 1)
 X = StandardScaler().fit_transform(X.to_numpy())
 X = X.reshape(num_samples, 48, -1)
 X_ori = X  # keep X_ori for validation
 X = mcar(X, 0.1)  # randomly hold out 10% observed values as ground truth
 dataset = {"X": X}  # X for model input
 print(X.shape)  # (11988, 48, 37), 11988 samples and each sample has 48 time steps, 37 features
 
 # Model training. This is PyPOTS showtime.
-saits = SAITS(n_steps=48, n_features=37, n_layers=2, d_model=256, d_ffn=128, n_heads=4, d_k=64, d_v=64, dropout=0.1, epochs=10)
+from pypots.imputation import SAITS
+from pypots.utils.metrics import calc_mae
+saits = SAITS(n_steps=48, n_features=37, n_layers=2, d_model=256, n_heads=4, d_k=64, d_v=64, d_ffn=128, dropout=0.1, epochs=10)
 # Here I use the whole dataset as the training set because ground truth is not visible to the model, you can also split it into train/val/test sets
-saits.fit(dataset)
+saits.fit(dataset)  # train the model on the dataset
 imputation = saits.impute(dataset)  # impute the originally-missing values and artificially-missing values
 indicating_mask = np.isnan(X) ^ np.isnan(X_ori)  # indicating mask for imputation error calculation
 mae = calc_mae(imputation, np.nan_to_num(X_ori), indicating_mask)  # calculate mean absolute error on the ground truth (artificially-missing values)
+saits.save("save_it_here/saits_physionet2012.pypots")  # save the model for future use
+saits.load("save_it_here/saits_physionet2012.pypots")  # reload the serialized model file for following imputation or training
 ```
 </details>
 
 
-## ❖ Available Algorithms
-PyPOTS supports imputation, classification, clustering, and forecasting tasks on multivariate time series with missing values.
-The currently available algorithms of four tasks are cataloged in the following table with four partitions.
-The paper references are all listed at the bottom of this readme file.
-
-🌟 Since **v0.2**, all neural-network models in PyPOTS has got hyperparameter-optimization support.
-This functionality is implemented with the [Microsoft NNI](https://github.com/microsoft/nni) framework.
-
-🔥 Note that Transformer, Crossformer, PatchTST, DLinear, ETSformer, FEDformer, Informer, Autoformer are not proposed as imputation methods in their original papers,
-and they cannot accept POTS as input. **To make them applicable on POTS data, we apply the embedding strategy and training approach (ORT+MIT)
-the same as we did in [SAITS paper](https://arxiv.org/pdf/2202.08516).**
-
-|   ***`Imputation`***   |     🚥      |                                               🚥                                                |    🚥    |
-|:----------------------:|:-----------:|:-----------------------------------------------------------------------------------------------:|:--------:|
-|        **Type**        |  **Abbr.**  |                              **Full name of the algorithm/model**                               | **Year** |
-|       Neural Net       |    SAITS    |                      Self-Attention-based Imputation for Time Series [^1]                       |   2023   |
-|       Neural Net       | Transformer |                                 Attention is All you Need [^2]                                  |   2017   |
-|       Neural Net       | Crossformer | Transformer Utilizing Cross-Dimension Dependency for Multivariate Time Series Forecasting [^16] |   2023   |
-|       Neural Net       |  TimesNet   |              Temporal 2D-Variation Modeling for General Time Series Analysis [^14]              |   2023   |
-|       Neural Net       |  PatchTST   |         A Time Series is Worth 64 Words: Long-Term Forecasting with Transformers [^18]          |   2023   |
-|       Neural Net       |   DLinear   |                  Are Transformers Effective for Time Series Forecasting? [^17]                  |   2023   |
-|       Neural Net       |  ETSformer  |              Exponential Smoothing Transformers for Time-series Forecasting [^19]               |   2023   |
-|       Neural Net       |  FEDformer  |        Frequency Enhanced Decomposed Transformer for Long-term Series Forecasting [^20]         |   2022   |
-|       Neural Net       |  Informer   |          Beyond Efficient Transformer for Long Sequence Time-Series Forecasting [^21]           |   2021   |
-|       Neural Net       | Autoformer  |     Decomposition Transformers with Auto-Correlation for Long-Term Series Forecasting [^15]     |   2021   |
-|       Neural Net       |    CSDI     |     Conditional Score-based Diffusion Models for Probabilistic Time Series Imputation [^12]     |   2021   |
-|       Neural Net       |   US-GAN    |                 Unsupervised GAN for Multivariate Time Series Imputation [^10]                  |   2021   |
-|       Neural Net       |   GP-VAE    |                         Gaussian Process Variational Autoencoder [^11]                          |   2020   |
-|       Neural Net       |    BRITS    |                     Bidirectional Recurrent Imputation for Time Series [^3]                     |   2018   |
-|       Neural Net       |    M-RNN    |                         Multi-directional Recurrent Neural Network [^9]                         |   2019   |
-|         Naive          |  LOCF/NOCB  |              Last Observation Carried Forward / Next Observation Carried Backward               |    -     |
-|         Naive          |   Median    |                                     Median Value Imputation                                     |    -     |
-|         Naive          |    Mean     |                                      Mean Value Imputation                                      |    -     |
-| ***`Classification`*** |     🚥      |                                               🚥                                                |    🚥    |
-|        **Type**        |  **Abbr.**  |                           **Full name of the algorithm/model/paper**                            | **Year** |
-|       Neural Net       |    BRITS    |                     Bidirectional Recurrent Imputation for Time Series [^3]                     |   2018   |
-|       Neural Net       |    GRU-D    |         Recurrent Neural Networks for Multivariate Time Series with Missing Values [^4]         |   2018   |
-|       Neural Net       |  Raindrop   |           Graph-Guided Network for Irregularly Sampled Multivariate Time Series [^5]            |   2022   |
-|   ***`Clustering`***   |     🚥      |                                               🚥                                                |    🚥    |
-|        **Type**        |  **Abbr.**  |                           **Full name of the algorithm/model/paper**                            | **Year** |
-|       Neural Net       |    CRLI     |             Clustering Representation Learning on Incomplete time-series data [^6]              |   2021   |
-|       Neural Net       |    VaDER    |                         Variational Deep Embedding with Recurrence [^7]                         |   2019   |
-|  ***`Forecasting`***   |     🚥      |                                               🚥                                                |    🚥    |
-|        **Type**        |  **Abbr.**  |                           **Full name of the algorithm/model/paper**                            | **Year** |
-|     Probabilistic      |    BTTF     |                           Bayesian Temporal Tensor Factorization [^8]                           |   2021   |
-
-
 ## ❖ Citing PyPOTS
 > [!TIP]
 > **[Updates in Feb 2024]** 😎 Our survey paper [Deep Learning for Multivariate Time Series Imputation: A Survey](https://arxiv.org/abs/2402.04059) has been released on arXiv.
 The code is open source in the GitHub repo [Awesome_Imputation](https://github.com/WenjieDu/Awesome_Imputation).
 We comprehensively review the literature of the state-of-the-art deep-learning imputation methods for time series,
 provide a taxonomy for them, and discuss the challenges and future directions in this field.
 >
@@ -334,14 +383,17 @@
 [^15]: Wu, H., Xu, J., Wang, J., & Long, M. (2021). [Autoformer: Decomposition transformers with auto-correlation for long-term series forecasting](https://proceedings.neurips.cc/paper/2021/hash/bcc0d400288793e8bdcd7c19a8ac0c2b-Abstract.html). *NeurIPS 2021*.
 [^16]: Zhang, Y., & Yan, J. (2023). [Crossformer: Transformer utilizing cross-dimension dependency for multivariate time series forecasting](https://openreview.net/forum?id=vSVLM2j9eie). *ICLR 2023*.
 [^17]: Zeng, A., Chen, M., Zhang, L., & Xu, Q. (2023). [Are transformers effective for time series forecasting?](https://ojs.aaai.org/index.php/AAAI/article/view/26317). *AAAI 2023*
 [^18]: Nie, Y., Nguyen, N. H., Sinthong, P., & Kalagnanam, J. (2023). [A time series is worth 64 words: Long-term forecasting with transformers](https://openreview.net/forum?id=Jbdc0vTOcol). *ICLR 2023*
 [^19]: Woo, G., Liu, C., Sahoo, D., Kumar, A., & Hoi, S. (2023). [ETSformer: Exponential Smoothing Transformers for Time-series Forecasting](https://openreview.net/forum?id=5m_3whfo483).  *ICLR 2023*
 [^20]: Zhou, T., Ma, Z., Wen, Q., Wang, X., Sun, L., & Jin, R. (2022). [FEDformer: Frequency enhanced decomposed transformer for long-term series forecasting](https://proceedings.mlr.press/v162/zhou22g.html). *ICML 2022*.
 [^21]: Zhou, H., Zhang, S., Peng, J., Zhang, S., Li, J., Xiong, H., & Zhang, W. (2021). [Informer: Beyond efficient transformer for long sequence time-series forecasting](https://ojs.aaai.org/index.php/AAAI/article/view/17325). *AAAI 2021*.
+[^22]: Zhou, T., Ma, Z., Wen, Q., Sun, L., Yao, T., Yin, W., & Jin, R. (2022). [FiLM: Frequency improved Legendre Memory Model for Long-term Time Series Forecasting](https://proceedings.neurips.cc/paper_files/paper/2022/hash/524ef58c2bd075775861234266e5e020-Abstract-Conference.html). *NeurIPS 2022*.
+[^23]: Yi, K., Zhang, Q., Fan, W., Wang, S., Wang, P., He, H., An, N., Lian, D., Cao, L., & Niu, Z. (2024). [Frequency-domain MLPs are More Effective Learners in Time Series Forecasting](https://proceedings.neurips.cc/paper_files/paper/2023/hash/f1d16af76939f476b5f040fd1398c0a3-Abstract-Conference.html). *NeurIPS 2024*.
+[^24]: Liu, Y., Hu, T., Zhang, H., Wu, H., Wang, S., Ma, L., & Long, M. (2024). [iTransformer: Inverted Transformers Are Effective for Time Series Forecasting](https://openreview.net/forum?id=JePfAI8fah). *ICLR 2024*.
 
 
 
 <details>
 <summary>🏠 Visits</summary>
 <a href="https://github.com/WenjieDu/PyPOTS">
     <img alt="PyPOTS visits" align="left" src="https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fgithub.com%2FPyPOTS%2FPyPOTS&count_bg=%23009A0A&title_bg=%23555555&icon=&icon_color=%23E7E7E7&title=Visits%20since%20May%202022&edge_flat=false">
```

#### html2text {}

```diff
@@ -1,14 +1,39 @@
-_[_h_t_t_p_s_:_/_/_p_y_p_o_t_s_._c_o_m_/_f_i_g_s_/_p_y_p_o_t_s___l_o_g_o_s_/_P_y_P_O_T_S_/_l_o_g_o___F_F_B_G_._s_v_g_]
+Metadata-Version: 2.1 Name: pypots Version: 0.5 Summary: A Python Toolbox for
+Data Mining on Partially-Observed Time Series Home-page: https://pypots.com/
+Author: Wenjie Du Author-email: wenjay.du@gmail.com License: BSD-3-Clause
+Project-URL: Documentation, https://docs.pypots.com/ Project-URL: Source,
+https://github.com/WenjieDu/PyPOTS/ Project-URL: Tracker, https://github.com/
+WenjieDu/PyPOTS/issues/ Project-URL: Download, https://github.com/WenjieDu/
+PyPOTS/archive/main.zip Keywords: data science,data mining,neural
+networks,machine learning,deep learning,artificial intelligence,time-series
+analysis,time
+series,imputation,interpolation,classification,clustering,forecasting,partially
+observed,irregular sampled,partially-observed time series,incomplete time
+series,missing data,missing values Classifier: Development Status :: 5 -
+Production/Stable Classifier: Intended Audience :: Developers Classifier:
+Intended Audience :: Education Classifier: Intended Audience :: Science/
+Research Classifier: Intended Audience :: Healthcare Industry Classifier:
+License :: OSI Approved :: BSD License Classifier: Operating System :: OS
+Independent Classifier: Programming Language :: Python :: 3 Classifier:
+Programming Language :: Python :: 3.7 Classifier: Programming Language ::
+Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
+Programming Language :: Python :: 3.10 Classifier: Programming Language ::
+Python :: 3.11 Classifier: Topic :: Scientific/Engineering :: Artificial
+Intelligence Classifier: Topic :: Software Development :: Libraries ::
+Application Frameworks Requires-Python: >=3.7.0 Description-Content-Type: text/
+markdown Provides-Extra: basic Provides-Extra: optional Provides-Extra: full
+Provides-Extra: test Provides-Extra: doc Provides-Extra: dev License-File:
+LICENSE_[_h_t_t_p_s_:_/_/_p_y_p_o_t_s_._c_o_m_/_f_i_g_s_/_p_y_p_o_t_s___l_o_g_o_s_/_P_y_P_O_T_S_/_l_o_g_o___F_F_B_G_._s_v_g_]
                           ******** WWeellccoommee ttoo PPyyPPOOTTSS ********
     a Python toolbox for machine learning on Partially-Observed Time Series
 _[_P_y_t_h_o_n_ _v_e_r_s_i_o_n_]_[_p_o_w_e_r_e_d_ _b_y_ _P_y_t_o_r_c_h_]_[_t_h_e_ _l_a_t_e_s_t_ _r_e_l_e_a_s_e_ _v_e_r_s_i_o_n_]_[_B_S_D_-_3_ _l_i_c_e_n_s_e_]
   _[_C_o_m_m_u_n_i_t_y_]_[_G_i_t_H_u_b_ _c_o_n_t_r_i_b_u_t_o_r_s_]_[_G_i_t_H_u_b_ _R_e_p_o_ _s_t_a_r_s_]_[_G_i_t_H_u_b_ _R_e_p_o_ _f_o_r_k_s_]_[_C_o_d_e
   _C_l_i_m_a_t_e_ _m_a_i_n_t_a_i_n_a_b_i_l_i_t_y_]_[_C_o_v_e_r_a_l_l_s_ _c_o_v_e_r_a_g_e_]_[_G_i_t_H_u_b_ _T_e_s_t_i_n_g_]_[_D_o_c_s_ _b_u_i_l_d_i_n_g_]
-                 _[_C_o_n_d_a_ _d_o_w_n_l_o_a_d_s_]_[_P_y_P_I_ _d_o_w_n_l_o_a_d_s_]_[_a_r_X_i_v_ _D_O_I_]
+        _[_C_o_n_d_a_ _d_o_w_n_l_o_a_d_s_]_[_P_y_P_I_ _d_o_w_n_l_o_a_d_s_]_[_a_r_X_i_v_ _D_O_I_]_[_R_E_A_D_M_E_ _i_n_ _C_h_i_n_e_s_e_]
 â¦¿ `Motivation`: Due to all kinds of reasons like failure of collection
 sensors, communication error, and unexpected malfunction, missing values are
 common to see in time series from the real-world environment. This makes
 partially-observed time series (POTS) a pervasive problem in open-world
 modeling and prevents advanced data analysis. Although this problem is
 important, the area of machine learning on POTS still lacks a dedicated
 toolkit. PyPOTS is created to fill in this blank. â¦¿ `Mission`: PyPOTS
@@ -20,150 +45,144 @@
 partially-observed multivariate time series. For sure, besides various
 algorithms, PyPOTS is going to have unified APIs together with detailed
 documentation and interactive examples across algorithms as tutorials. ð¤
 **Please** star this repo to help others notice PyPOTS if you think it is a
 useful toolkit. **Please** properly [cite PyPOTS](https://github.com/WenjieDu/
 PyPOTS#-citing-pypots) in your publications if it helps with your research.
 This really means a lot to our open-source research. Thank you! The rest of
-this readme file is organized as follows: [**â PyPOTS Ecosystem**](#-pypots-
-ecosystem), [**â Installation**](#-installation), [**â Usage**](#-usage),
-[**â Available Algorithms**](#-available-algorithms), [**â Citing PyPOTS**]
-(#-citing-pypots), [**â Contribution**](#-contribution), [**â Community**]
-(#-community). ## â PyPOTS Ecosystem At PyPOTS, things are related to coffee,
-which we're familiar with. Yes, this is a coffee universe! As you can see,
-there is a coffee pot in the PyPOTS logo. And what else? Please read on ;-)
-_[_T_S_D_B_ _l_o_g_o_]ð Time series datasets are taken as coffee beans at PyPOTS, and
-POTS datasets are incomplete coffee beans with missing parts that have their
-own meanings. To make various public time-series datasets readily available to
-users, Time Series Data Beans (TSDB) is created to make loading time-series
-datasets super easy! Visit [TSDB](https://github.com/WenjieDu/TSDB) right now
-to know more about this handy tool ð , and it now supports a total of 168
-open-source datasets! _[_P_y_G_r_i_n_d_e_r_ _l_o_g_o_]ð To simulate the real-world data
-beans with missingness, the ecosystem library [PyGrinder](https://github.com/
-WenjieDu/PyGrinder), a toolkit helping grind your coffee beans into incomplete
-ones, is created. Missing patterns fall into three categories according to
-Robin's theory[^13]: MCAR (missing completely at random), MAR (missing at
-random), and MNAR (missing not at random). PyGrinder supports all of them and
-additional functionalities related to missingness. With PyGrinder, you can
-introduce synthetic missing values into your datasets with a single line of
-code. _[_B_r_e_w_P_O_T_S_ _l_o_g_o_]ð Now we have the beans, the grinder, and the pot, how
-to brew us a cup of coffee? Tutorials are necessary! Considering the future
-workload, PyPOTS tutorials are released in a single repo, and you can find them
-in [BrewPOTS](https://github.com/WenjieDu/BrewPOTS). Take a look at it now, and
-learn how to brew your POTS datasets!
+this readme file is organized as follows: [**â Available Algorithms**](#-
+available-algorithms), [**â PyPOTS Ecosystem**](#-pypots-ecosystem), [**â
+Installation**](#-installation), [**â Usage**](#-usage), [**â Citing
+PyPOTS**](#-citing-pypots), [**â Contribution**](#-contribution), [**â
+Community**](#-community). ## â Available Algorithms PyPOTS supports
+imputation, classification, clustering, forecasting, and anomaly detection
+tasks on multivariate partially-observed time series with missing values. The
+table below shows the availability of each algorithm (sorted by Year) in PyPOTS
+for different tasks. The symbol â indicates the algorithm is available for
+the corresponding task (note that models will be continuously updated in the
+future to handle tasks that are not currently supported. Stay tunedâï¸).
+ð Since **v0.2**, all neural-network models in PyPOTS has got
+hyperparameter-optimization support. This functionality is implemented with the
+[Microsoft NNI](https://github.com/microsoft/nni) framework. You may want to
+refer to our time-series imputation survey repo [Awesome_Imputation](https://
+github.com/WenjieDu/Awesome_Imputation) to see how to config and tune the
+hyperparameters. ð¥ Note that Transformer, iTransformer, FreTS, Crossformer,
+PatchTST, DLinear, ETSformer, FiLM, FEDformer, Informer, Autoformer are not
+proposed as imputation methods in their original papers, and they cannot accept
+POTS as input. **To make them applicable on POTS data, we apply the embedding
+strategy and training approach (ORT+MIT) the same as we did in [SAITS paper]
+(https://arxiv.org/pdf/2202.08516).** The task types are abbreviated as
+follows: **`IMPU`**: Imputation; **`FORE`**: Forecasting; **`CLAS`**:
+Classification; **`CLUS`**: Clustering; **`ANOD`**: Anomaly Detection. The
+paper references and links are all listed at the bottom of this file. |
+**Type** | **Algo** | **IMPU** | **FORE** | **CLAS** | **CLUS** | **ANOD** |
+**Year - Venue** | |:--------------|:-----------------------------------|:-----
+---:|:--------:|:--------:|:--------:|:--------:|:-----------------| | Neural
+Net | iTransformer[^24] | â | | | | | 2024 - ICLR | | Neural Net | FreTS[^23]
+| â | | | | | 2024 - NeurIPS | | Neural Net | SAITS[^1] | â | | | | | 2023
+- ESWA | | Neural Net | Crossformer[^16] | â | | | | | 2023 - ICLR | | Neural
+Net | TimesNet[^14] | â | | | | | 2023 - ICLR | | Neural Net | PatchTST[^18]
+| â | | | | | 2023 - ICLR | | Neural Net | ETSformer[^19] | â | | | | |
+2023 - ICLR | | Neural Net | DLinear[^17] | â | | | | | 2023 - AAAI | |
+Neural Net | FiLM[^22] | â | | | | | 2022 - NeurIPS | | Neural Net | Raindrop
+[^5] | | | â | | | 2022 - ICLR | | Neural Net | FEDformer[^20] | â | | | |
+| 2022 - ICML | | Neural Net | Autoformer[^15] | â | | | | | 2021 - NeurIPS |
+| Neural Net | CSDI[^12] | â | â | | | | 2021 - NeurIPS | | Neural Net |
+Informer[^21] | â | | | | | 2021 - AAAI | | Neural Net | US-GAN[^10] | â |
+| | | | 2021 - AAAI | | Neural Net | CRLI[^6] | | | | â | | 2021 - AAAI | |
+Probabilistic | BTTF[^8] | | â | | | | 2021 - TPAMI | | Neural Net | GP-VAE
+[^11] | â | | | | | 2020 - AISTATS | | Neural Net | VaDER[^7] | | | | â | |
+2019 - GigaSci. | | Neural Net | M-RNN[^9] | â | | | | | 2019 - TBME | |
+Neural Net | BRITS[^3] | â | | â | | | 2018 - NeurIPS | | Neural Net | GRU-
+D[^4] | â | | â | | | 2018 - Sci. Rep. | | Neural Net | Transformer[^2] |
+â | | | | | 2017 - NeurIPS | | Naive | LOCF/NOCB | â | | | | | | | Naive |
+Mean | â | | | | | | | Naive | Median | â | | | | | | ## â PyPOTS
+Ecosystem At PyPOTS, things are related to coffee, which we're familiar with.
+Yes, this is a coffee universe! As you can see, there is a coffee pot in the
+PyPOTS logo. And what else? Please read on ;-) _[_T_S_D_B_ _l_o_g_o_]ð Time series
+datasets are taken as coffee beans at PyPOTS, and POTS datasets are incomplete
+coffee beans with missing parts that have their own meanings. To make various
+public time-series datasets readily available to users, Time Series Data Beans
+(TSDB) is created to make loading time-series datasets super easy! Visit [TSDB]
+(https://github.com/WenjieDu/TSDB) right now to know more about this handy tool
+ð , and it now supports a total of 169 open-source datasets! _[_P_y_G_r_i_n_d_e_r
+_l_o_g_o_]ð To simulate the real-world data beans with missingness, the ecosystem
+library [PyGrinder](https://github.com/WenjieDu/PyGrinder), a toolkit helping
+grind your coffee beans into incomplete ones, is created. Missing patterns fall
+into three categories according to Robin's theory[^13]: MCAR (missing
+completely at random), MAR (missing at random), and MNAR (missing not at
+random). PyGrinder supports all of them and additional functionalities related
+to missingness. With PyGrinder, you can introduce synthetic missing values into
+your datasets with a single line of code. _[_B_r_e_w_P_O_T_S_ _l_o_g_o_]ð Now we have the
+beans, the grinder, and the pot, how to brew us a cup of coffee? Tutorials are
+necessary! Considering the future workload, PyPOTS tutorials are released in a
+single repo, and you can find them in [BrewPOTS](https://github.com/WenjieDu/
+BrewPOTS). Take a look at it now, and learn how to brew your POTS datasets!
 _[_h_t_t_p_s_:_/_/_p_y_p_o_t_s_._c_o_m_/_f_i_g_s_/_p_y_p_o_t_s___l_o_g_o_s_/_E_c_o_s_y_s_t_e_m_/_P_y_P_O_T_S___E_c_o_s_y_s_t_e_m___P_i_p_e_l_i_n_e_._p_n_g_]
        ?â???ï?¸? WWeellccoommee ttoo tthhee uunniivveerrssee ooff PPyyPPOOTTSS.. EEnnjjooyy iitt aanndd hhaavvee ffuunn!!
 ## â Installation You can refer to [the installation instruction](https://
 docs.pypots.com/en/latest/install.html) in PyPOTS documentation for a guideline
 with more details. PyPOTS is available on both [PyPI](https://pypi.python.org/
 pypi/pypots) and [Anaconda](https://anaconda.org/conda-forge/pypots). You can
-install PyPOTS as shown below: ``` bash # via pip pip install pypots # the
-first time installation pip install pypots --upgrade # update pypots to the
-latest version # install from the latest source code with the latest features
-but may be not officially released yet pip install https://github.com/WenjieDu/
-PyPOTS/archive/main.zip # via conda conda install -c conda-forge pypots # the
-first time installation conda update -c conda-forge pypots # update pypots to
-the latest version ``` ## â Usage Besides [BrewPOTS](https://github.com/
-WenjieDu/BrewPOTS), you can also find a simple and quick-start tutorial
-notebook on Google Colab _[_C_o_l_a_b_ _t_u_t_o_r_i_a_l_s_]. If you have further questions,
-please refer to PyPOTS documentation [docs.pypots.com](https://
+install PyPOTS like below as well as TSDB and PyGrinder: ``` bash # via pip pip
+install pypots # the first time installation pip install pypots --upgrade #
+update pypots to the latest version # install from the latest source code with
+the latest features but may be not officially released yet pip install https://
+github.com/WenjieDu/PyPOTS/archive/main.zip # via conda conda install -c conda-
+forge pypots # the first time installation conda update -c conda-forge pypots #
+update pypots to the latest version ``` ## â Usage Besides [BrewPOTS](https:/
+/github.com/WenjieDu/BrewPOTS), you can also find a simple and quick-start
+tutorial notebook on Google Colab _[_C_o_l_a_b_ _t_u_t_o_r_i_a_l_s_]. If you have further
+questions, please refer to PyPOTS documentation [docs.pypots.com](https://
 docs.pypots.com). You can also [raise an issue](https://github.com/WenjieDu/
 PyPOTS/issues) or [ask in our community](#-community). We present you a usage
 example of imputing missing values in time series with PyPOTS below, you can
 click it to view. CClliicckk hheerree ttoo sseeee aann eexxaammppllee aappppllyyiinngg SSAAIITTSS oonn PPhhyyssiiooNNeett22001122
-ffoorr iimmppuuttaattiioonn:: ``` python import numpy as np from sklearn.preprocessing import
-StandardScaler from pygrinder import mcar from pypots.data import
-load_specific_dataset from pypots.imputation import SAITS from
-pypots.utils.metrics import calc_mae # Data preprocessing. Tedious, but PyPOTS
-can help. data = load_specific_dataset('physionet_2012') # PyPOTS will
-automatically download and extract it. X = data['X'] num_samples = len(X
-['RecordID'].unique()) X = X.drop(['RecordID', 'Time'], axis = 1) X =
-StandardScaler().fit_transform(X.to_numpy()) X = X.reshape(num_samples, 48, -1)
-X_ori = X # keep X_ori for validation X = mcar(X, 0.1) # randomly hold out 10%
-observed values as ground truth dataset = {"X": X} # X for model input print
-(X.shape) # (11988, 48, 37), 11988 samples and each sample has 48 time steps,
-37 features # Model training. This is PyPOTS showtime. saits = SAITS
-(n_steps=48, n_features=37, n_layers=2, d_model=256, d_ffn=128, n_heads=4,
-d_k=64, d_v=64, dropout=0.1, epochs=10) # Here I use the whole dataset as the
-training set because ground truth is not visible to the model, you can also
-split it into train/val/test sets saits.fit(dataset) imputation = saits.impute
-(dataset) # impute the originally-missing values and artificially-missing
-values indicating_mask = np.isnan(X) ^ np.isnan(X_ori) # indicating mask for
-imputation error calculation mae = calc_mae(imputation, np.nan_to_num(X_ori),
-indicating_mask) # calculate mean absolute error on the ground truth
-(artificially-missing values) ``` ## â Available Algorithms PyPOTS supports
-imputation, classification, clustering, and forecasting tasks on multivariate
-time series with missing values. The currently available algorithms of four
-tasks are cataloged in the following table with four partitions. The paper
-references are all listed at the bottom of this readme file. ð Since
-**v0.2**, all neural-network models in PyPOTS has got hyperparameter-
-optimization support. This functionality is implemented with the [Microsoft
-NNI](https://github.com/microsoft/nni) framework. ð¥ Note that Transformer,
-Crossformer, PatchTST, DLinear, ETSformer, FEDformer, Informer, Autoformer are
-not proposed as imputation methods in their original papers, and they cannot
-accept POTS as input. **To make them applicable on POTS data, we apply the
-embedding strategy and training approach (ORT+MIT) the same as we did in [SAITS
-paper](https://arxiv.org/pdf/2202.08516).** | ***`Imputation`*** | ð¥ | ð¥
-| ð¥ | |:----------------------:|:-----------:|:-----------------------------
-------------------------------------------------------------------:|:--------:
-| | **Type** | **Abbr.** | **Full name of the algorithm/model** | **Year** | |
-Neural Net | SAITS | Self-Attention-based Imputation for Time Series [^1] |
-2023 | | Neural Net | Transformer | Attention is All you Need [^2] | 2017 | |
-Neural Net | Crossformer | Transformer Utilizing Cross-Dimension Dependency for
-Multivariate Time Series Forecasting [^16] | 2023 | | Neural Net | TimesNet |
-Temporal 2D-Variation Modeling for General Time Series Analysis [^14] | 2023 |
-| Neural Net | PatchTST | A Time Series is Worth 64 Words: Long-Term
-Forecasting with Transformers [^18] | 2023 | | Neural Net | DLinear | Are
-Transformers Effective for Time Series Forecasting? [^17] | 2023 | | Neural Net
-| ETSformer | Exponential Smoothing Transformers for Time-series Forecasting
-[^19] | 2023 | | Neural Net | FEDformer | Frequency Enhanced Decomposed
-Transformer for Long-term Series Forecasting [^20] | 2022 | | Neural Net |
-Informer | Beyond Efficient Transformer for Long Sequence Time-Series
-Forecasting [^21] | 2021 | | Neural Net | Autoformer | Decomposition
-Transformers with Auto-Correlation for Long-Term Series Forecasting [^15] |
-2021 | | Neural Net | CSDI | Conditional Score-based Diffusion Models for
-Probabilistic Time Series Imputation [^12] | 2021 | | Neural Net | US-GAN |
-Unsupervised GAN for Multivariate Time Series Imputation [^10] | 2021 | |
-Neural Net | GP-VAE | Gaussian Process Variational Autoencoder [^11] | 2020 | |
-Neural Net | BRITS | Bidirectional Recurrent Imputation for Time Series [^3] |
-2018 | | Neural Net | M-RNN | Multi-directional Recurrent Neural Network [^9] |
-2019 | | Naive | LOCF/NOCB | Last Observation Carried Forward / Next
-Observation Carried Backward | - | | Naive | Median | Median Value Imputation |
-- | | Naive | Mean | Mean Value Imputation | - | | ***`Classification`*** |
-ð¥ | ð¥ | ð¥ | | **Type** | **Abbr.** | **Full name of the algorithm/
-model/paper** | **Year** | | Neural Net | BRITS | Bidirectional Recurrent
-Imputation for Time Series [^3] | 2018 | | Neural Net | GRU-D | Recurrent
-Neural Networks for Multivariate Time Series with Missing Values [^4] | 2018 |
-| Neural Net | Raindrop | Graph-Guided Network for Irregularly Sampled
-Multivariate Time Series [^5] | 2022 | | ***`Clustering`*** | ð¥ | ð¥ |
-ð¥ | | **Type** | **Abbr.** | **Full name of the algorithm/model/paper** |
-**Year** | | Neural Net | CRLI | Clustering Representation Learning on
-Incomplete time-series data [^6] | 2021 | | Neural Net | VaDER | Variational
-Deep Embedding with Recurrence [^7] | 2019 | | ***`Forecasting`*** | ð¥ |
-ð¥ | ð¥ | | **Type** | **Abbr.** | **Full name of the algorithm/model/
-paper** | **Year** | | Probabilistic | BTTF | Bayesian Temporal Tensor
-Factorization [^8] | 2021 | ## â Citing PyPOTS > [!TIP] > **[Updates in Feb
-2024]** ð Our survey paper [Deep Learning for Multivariate Time Series
-Imputation: A Survey](https://arxiv.org/abs/2402.04059) has been released on
-arXiv. The code is open source in the GitHub repo [Awesome_Imputation](https://
-github.com/WenjieDu/Awesome_Imputation). We comprehensively review the
-literature of the state-of-the-art deep-learning imputation methods for time
-series, provide a taxonomy for them, and discuss the challenges and future
-directions in this field. > > **[Updates in Jun 2023]** ð A short version of
-the PyPOTS paper is accepted by the 9th SIGKDD international workshop on Mining
-and Learning from Time Series ([MiLeTS'23](https://kdd-milets.github.io/
-milets2023/))). **Additionally**, PyPOTS has been included as a [PyTorch
-Ecosystem](https://pytorch.org/ecosystem/) project. The paper introducing
-PyPOTS is available on arXiv at [this URL](https://arxiv.org/abs/2305.18811),
-and we are pursuing to publish it in prestigious academic venues, e.g. JMLR
-(track for [Machine Learning Open Source Software](https://www.jmlr.org/mloss/
-)). If you use PyPOTS in your work, please cite it as below and ðstar this
-repository to make others notice this library. ð¤ There are scientific
-research projects using PyPOTS and referencing in their papers. Here is [an
-incomplete list of them](https://scholar.google.com/
+ffoorr iimmppuuttaattiioonn:: ``` python # Data preprocessing. Tedious, but PyPOTS can help.
+import numpy as np from sklearn.preprocessing import StandardScaler from
+pygrinder import mcar from pypots.data import load_specific_dataset data =
+load_specific_dataset('physionet_2012') # PyPOTS will automatically download
+and extract it. X = data['X'] num_samples = len(X['RecordID'].unique()) X =
+X.drop(['RecordID', 'Time'], axis = 1) X = StandardScaler().fit_transform
+(X.to_numpy()) X = X.reshape(num_samples, 48, -1) X_ori = X # keep X_ori for
+validation X = mcar(X, 0.1) # randomly hold out 10% observed values as ground
+truth dataset = {"X": X} # X for model input print(X.shape) # (11988, 48, 37),
+11988 samples and each sample has 48 time steps, 37 features # Model training.
+This is PyPOTS showtime. from pypots.imputation import SAITS from
+pypots.utils.metrics import calc_mae saits = SAITS(n_steps=48, n_features=37,
+n_layers=2, d_model=256, n_heads=4, d_k=64, d_v=64, d_ffn=128, dropout=0.1,
+epochs=10) # Here I use the whole dataset as the training set because ground
+truth is not visible to the model, you can also split it into train/val/test
+sets saits.fit(dataset) # train the model on the dataset imputation =
+saits.impute(dataset) # impute the originally-missing values and artificially-
+missing values indicating_mask = np.isnan(X) ^ np.isnan(X_ori) # indicating
+mask for imputation error calculation mae = calc_mae(imputation, np.nan_to_num
+(X_ori), indicating_mask) # calculate mean absolute error on the ground truth
+(artificially-missing values) saits.save("save_it_here/
+saits_physionet2012.pypots") # save the model for future use saits.load
+("save_it_here/saits_physionet2012.pypots") # reload the serialized model file
+for following imputation or training ``` ## â Citing PyPOTS > [!TIP] > **
+[Updates in Feb 2024]** ð Our survey paper [Deep Learning for Multivariate
+Time Series Imputation: A Survey](https://arxiv.org/abs/2402.04059) has been
+released on arXiv. The code is open source in the GitHub repo
+[Awesome_Imputation](https://github.com/WenjieDu/Awesome_Imputation). We
+comprehensively review the literature of the state-of-the-art deep-learning
+imputation methods for time series, provide a taxonomy for them, and discuss
+the challenges and future directions in this field. > > **[Updates in Jun
+2023]** ð A short version of the PyPOTS paper is accepted by the 9th SIGKDD
+international workshop on Mining and Learning from Time Series ([MiLeTS'23]
+(https://kdd-milets.github.io/milets2023/))). **Additionally**, PyPOTS has been
+included as a [PyTorch Ecosystem](https://pytorch.org/ecosystem/) project. The
+paper introducing PyPOTS is available on arXiv at [this URL](https://arxiv.org/
+abs/2305.18811), and we are pursuing to publish it in prestigious academic
+venues, e.g. JMLR (track for [Machine Learning Open Source Software](https://
+www.jmlr.org/mloss/)). If you use PyPOTS in your work, please cite it as below
+and ðstar this repository to make others notice this library. ð¤ There are
+scientific research projects using PyPOTS and referencing in their papers. Here
+is [an incomplete list of them](https://scholar.google.com/
 scholar?as_ylo=2022&q=%E2%80%9CPyPOTS%E2%80%9D&hl=en>). ``` bibtex @article
 {du2023pypots, title={{PyPOTS: a Python toolbox for data mining on Partially-
 Observed Time Series}}, author={Wenjie Du}, year={2023}, eprint={2305.18811},
 archivePrefix={arXiv}, primaryClass={cs.LG}, url={https://arxiv.org/abs/
 2305.18811}, doi={10.48550/arXiv.2305.18811}, } ``` or > Wenjie Du. (2023). >
 PyPOTS: a Python toolbox for data mining on Partially-Observed Time Series. >
 arXiv, abs/2305.18811.https://arxiv.org/abs/2305.18811 ## â Contribution
@@ -251,9 +270,20 @@
 Exponential Smoothing Transformers for Time-series Forecasting](https://
 openreview.net/forum?id=5m_3whfo483). *ICLR 2023* [^20]: Zhou, T., Ma, Z., Wen,
 Q., Wang, X., Sun, L., & Jin, R. (2022). [FEDformer: Frequency enhanced
 decomposed transformer for long-term series forecasting](https://
 proceedings.mlr.press/v162/zhou22g.html). *ICML 2022*. [^21]: Zhou, H., Zhang,
 S., Peng, J., Zhang, S., Li, J., Xiong, H., & Zhang, W. (2021). [Informer:
 Beyond efficient transformer for long sequence time-series forecasting](https:/
-/ojs.aaai.org/index.php/AAAI/article/view/17325). *AAAI 2021*. ð  Visits
-_[_P_y_P_O_T_S_ _v_i_s_i_t_s_]
+/ojs.aaai.org/index.php/AAAI/article/view/17325). *AAAI 2021*. [^22]: Zhou, T.,
+Ma, Z., Wen, Q., Sun, L., Yao, T., Yin, W., & Jin, R. (2022). [FiLM: Frequency
+improved Legendre Memory Model for Long-term Time Series Forecasting](https://
+proceedings.neurips.cc/paper_files/paper/2022/hash/
+524ef58c2bd075775861234266e5e020-Abstract-Conference.html). *NeurIPS 2022*.
+[^23]: Yi, K., Zhang, Q., Fan, W., Wang, S., Wang, P., He, H., An, N., Lian,
+D., Cao, L., & Niu, Z. (2024). [Frequency-domain MLPs are More Effective
+Learners in Time Series Forecasting](https://proceedings.neurips.cc/
+paper_files/paper/2023/hash/f1d16af76939f476b5f040fd1398c0a3-Abstract-
+Conference.html). *NeurIPS 2024*. [^24]: Liu, Y., Hu, T., Zhang, H., Wu, H.,
+Wang, S., Ma, L., & Long, M. (2024). [iTransformer: Inverted Transformers Are
+Effective for Time Series Forecasting](https://openreview.net/
+forum?id=JePfAI8fah). *ICLR 2024*. ð  Visits_[_P_y_P_O_T_S_ _v_i_s_i_t_s_]
```

### Comparing `pypots-0.4.1/pypots/__init__.py` & `pypots-0.5/pypots/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 # X.YaN # Alpha release
 # X.YbN # Beta release
 # X.YrcN # Release Candidate
 # X.Y # Final release
 #
 # Dev branch marker is: 'X.Y.dev' or 'X.Y.devN' where N is an integer.
 # 'X.Y.dev0' is the canonical version of 'X.Y.dev'
-__version__ = "0.4.1"
+__version__ = "0.5"
 
 
 from . import imputation, classification, clustering, forecasting, optim, data, utils
 
 __all__ = [
     "imputation",
     "classification",
```

### Comparing `pypots-0.4.1/pypots/base.py` & `pypots-0.5/pypots/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -281,15 +281,18 @@
 
         if os.path.exists(saving_path):
             if overwrite:
                 logger.warning(
                     f"‼️ File {saving_path} exists. Argument `overwrite` is True. Overwriting now..."
                 )
             else:
-                logger.error(f"❌ File {saving_path} exists. Saving operation aborted.")
+                logger.error(
+                    f"❌ File {saving_path} exists. Saving operation aborted. "
+                    f"Use the arg `overwrite=True` to force overwrite."
+                )
 
         try:
             create_dir_if_not_exist(saving_dir)
             if isinstance(self.device, list):
                 # to save a DataParallel model generically, save the model.module.state_dict()
                 torch.save(self.model.module, saving_path)
             else:
@@ -333,69 +336,69 @@
         logger.info(f"Model loaded successfully from {path}")
 
     @abstractmethod
     def fit(
         self,
         train_set: Union[dict, str],
         val_set: Optional[Union[dict, str]] = None,
-        file_type: str = "h5py",
+        file_type: str = "hdf5",
     ) -> None:
         """Train the classifier on the given data.
 
         Parameters
         ----------
-        train_set : dict or str
+        train_set :
             The dataset for model training, should be a dictionary including keys as 'X',
             or a path string locating a data file supported by PyPOTS (e.g. h5 file).
-            If it is a dict, X should be array-like of shape [n_samples, sequence length (time steps), n_features],
+            If it is a dict, X should be array-like of shape [n_samples, sequence length (n_steps), n_features],
             which is time-series data for training, can contain missing values, and y should be array-like of shape
             [n_samples], which is classification labels of X.
             If it is a path string, the path should point to a data file, e.g. a h5 file, which contains
             key-value pairs like a dict, and it has to include keys as 'X' and 'y'.
 
-        val_set : dict or str
+        val_set :
             The dataset for model validating, should be a dictionary including keys as 'X',
             or a path string locating a data file supported by PyPOTS (e.g. h5 file).
-            If it is a dict, X should be array-like of shape [n_samples, sequence length (time steps), n_features],
+            If it is a dict, X should be array-like of shape [n_samples, sequence length (n_steps), n_features],
             which is time-series data for validating, can contain missing values, and y should be array-like of shape
             [n_samples], which is classification labels of X.
             If it is a path string, the path should point to a data file, e.g. a h5 file, which contains
             key-value pairs like a dict, and it has to include keys as 'X' and 'y'.
 
-        file_type : str
+        file_type :
             The type of the given file if train_set and val_set are path strings.
 
         """
         raise NotImplementedError
 
     @abstractmethod
     def predict(
         self,
         test_set: Union[dict, str],
-        file_type: str = "h5py",
+        file_type: str = "hdf5",
     ) -> dict:
         """Make predictions for the input data with the trained model.
 
         Parameters
         ----------
-        test_set : dict or str
+        test_set :
             The dataset for model validating, should be a dictionary including keys as 'X',
             or a path string locating a data file supported by PyPOTS (e.g. h5 file).
-            If it is a dict, X should be array-like of shape [n_samples, sequence length (time steps), n_features],
+            If it is a dict, X should be array-like of shape [n_samples, sequence length (n_steps), n_features],
             which is time-series data for validating, can contain missing values, and y should be array-like of shape
             [n_samples], which is classification labels of X.
             If it is a path string, the path should point to a data file, e.g. a h5 file, which contains
             key-value pairs like a dict, and it has to include keys as 'X' and 'y'.
 
-        file_type : str
+        file_type :
             The type of the given file if test_set is a path string.
 
         Returns
         -------
-        result_dict: dict
+        result_dict :
             Prediction results in a Python Dictionary for the given samples.
             It should be a dictionary including keys as 'imputation', 'classification', 'clustering', and 'forecasting'.
             For sure, only the keys that relevant tasks are supported by the model will be returned.
         """
         raise NotImplementedError
 
 
@@ -508,18 +511,18 @@
         )
 
     @abstractmethod
     def fit(
         self,
         train_set: Union[dict, str],
         val_set: Optional[Union[dict, str]] = None,
-        file_type: str = "h5py",
+        file_type: str = "hdf5",
     ) -> None:
         raise NotImplementedError
 
     @abstractmethod
     def predict(
         self,
         test_set: Union[dict, str],
-        file_type: str = "h5py",
+        file_type: str = "hdf5",
     ) -> dict:
         raise NotImplementedError
```

### Comparing `pypots-0.4.1/pypots/classification/base.py` & `pypots-0.5/pypots/classification/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,33 +68,33 @@
         self.n_classes = n_classes
 
     @abstractmethod
     def fit(
         self,
         train_set: Union[dict, str],
         val_set: Optional[Union[dict, str]] = None,
-        file_type: str = "h5py",
+        file_type: str = "hdf5",
     ) -> None:
         """Train the classifier on the given data.
 
         Parameters
         ----------
         train_set :
             The dataset for model training, should be a dictionary including keys as 'X' and 'y',
             or a path string locating a data file.
-            If it is a dict, X should be array-like of shape [n_samples, sequence length (time steps), n_features],
+            If it is a dict, X should be array-like of shape [n_samples, sequence length (n_steps), n_features],
             which is time-series data for training, can contain missing values, and y should be array-like of shape
             [n_samples], which is classification labels of X.
             If it is a path string, the path should point to a data file, e.g. a h5 file, which contains
             key-value pairs like a dict, and it has to include keys as 'X' and 'y'.
 
         val_set :
             The dataset for model validating, should be a dictionary including keys as 'X' and 'y',
             or a path string locating a data file.
-            If it is a dict, X should be array-like of shape [n_samples, sequence length (time steps), n_features],
+            If it is a dict, X should be array-like of shape [n_samples, sequence length (n_steps), n_features],
             which is time-series data for validating, can contain missing values, and y should be array-like of shape
             [n_samples], which is classification labels of X.
             If it is a path string, the path should point to a data file, e.g. a h5 file, which contains
             key-value pairs like a dict, and it has to include keys as 'X' and 'y'.
 
         file_type :
             The type of the given file if train_set and val_set are path strings.
@@ -102,42 +102,41 @@
         """
         raise NotImplementedError
 
     @abstractmethod
     def predict(
         self,
         test_set: Union[dict, str],
-        file_type: str = "h5py",
+        file_type: str = "hdf5",
     ) -> dict:
         raise NotImplementedError
 
     @abstractmethod
     def classify(
         self,
-        X: Union[dict, str],
-        file_type: str = "h5py",
+        test_set: Union[dict, str],
+        file_type: str = "hdf5",
     ) -> np.ndarray:
         """Classify the input data with the trained model.
 
         Parameters
         ----------
-        X :
-            The data samples for testing, should be array-like of shape [n_samples, sequence length (time steps),
+        test_set :
+            The data samples for testing, should be array-like of shape [n_samples, sequence length (n_steps),
             n_features], or a path string locating a data file, e.g. h5 file.
 
         file_type :
             The type of the given file if X is a path string.
 
         Returns
         -------
         array-like, shape [n_samples],
             Classification results of the given samples.
         """
-        # this is for old API compatibility, will be removed in the future.
-        # Please implement predict() instead.
+
         raise NotImplementedError
 
 
 class BaseNNClassifier(BaseNNModel):
     """The abstract class for all neural-network classification models in PyPOTS.
 
     Parameters
@@ -210,60 +209,60 @@
             device,
             saving_path,
             model_saving_strategy,
         )
         self.n_classes = n_classes
 
     @abstractmethod
-    def _assemble_input_for_training(self, data) -> dict:
+    def _assemble_input_for_training(self, data: list) -> dict:
         """Assemble the given data into a dictionary for training input.
 
         Parameters
         ----------
-        data : list,
+        data :
             Input data from dataloader, should be list.
 
         Returns
         -------
         dict,
             A python dictionary contains the input data for model training.
         """
         raise NotImplementedError
 
     @abstractmethod
-    def _assemble_input_for_validating(self, data) -> dict:
+    def _assemble_input_for_validating(self, data: list) -> dict:
         """Assemble the given data into a dictionary for validating input.
 
         Parameters
         ----------
-        data : list,
+        data :
             Data output from dataloader, should be list.
 
         Returns
         -------
         dict,
             A python dictionary contains the input data for model validating.
         """
         raise NotImplementedError
 
     @abstractmethod
-    def _assemble_input_for_testing(self, data) -> dict:
+    def _assemble_input_for_testing(self, data: list) -> dict:
         """Assemble the given data into a dictionary for testing input.
 
         Notes
         -----
         The processing functions of train/val/test stages are separated for the situation that the input of
         the three stages are different, and this situation usually happens when the Dataset/Dataloader classes
         used in the train/val/test stages are not the same, e.g. the training data and validating data in a
         classification task contains labels, but the testing data (from the production environment) generally
         doesn't have labels.
 
         Parameters
         ----------
-        data : list,
+        data :
             Data output from dataloader, should be list.
 
         Returns
         -------
         dict,
             A python dictionary contains the input data for model testing.
         """
@@ -382,33 +381,33 @@
         )
 
     @abstractmethod
     def fit(
         self,
         train_set: Union[dict, str],
         val_set: Optional[Union[dict, str]] = None,
-        file_type: str = "h5py",
+        file_type: str = "hdf5",
     ) -> None:
         """Train the classifier on the given data.
 
         Parameters
         ----------
         train_set :
             The dataset for model training, should be a dictionary including keys as 'X' and 'y',
             or a path string locating a data file.
-            If it is a dict, X should be array-like of shape [n_samples, sequence length (time steps), n_features],
+            If it is a dict, X should be array-like of shape [n_samples, sequence length (n_steps), n_features],
             which is time-series data for training, can contain missing values, and y should be array-like of shape
             [n_samples], which is classification labels of X.
             If it is a path string, the path should point to a data file, e.g. a h5 file, which contains
             key-value pairs like a dict, and it has to include keys as 'X' and 'y'.
 
         val_set :
             The dataset for model validating, should be a dictionary including keys as 'X' and 'y',
             or a path string locating a data file.
-            If it is a dict, X should be array-like of shape [n_samples, sequence length (time steps), n_features],
+            If it is a dict, X should be array-like of shape [n_samples, sequence length (n_steps), n_features],
             which is time-series data for validating, can contain missing values, and y should be array-like of shape
             [n_samples], which is classification labels of X.
             If it is a path string, the path should point to a data file, e.g. a h5 file, which contains
             key-value pairs like a dict, and it has to include keys as 'X' and 'y'.
 
         file_type :
             The type of the given file if train_set and val_set are path strings.
@@ -416,40 +415,37 @@
         """
         raise NotImplementedError
 
     @abstractmethod
     def predict(
         self,
         test_set: Union[dict, str],
-        file_type: str = "h5py",
+        file_type: str = "hdf5",
     ) -> dict:
         raise NotImplementedError
 
     @abstractmethod
     def classify(
         self,
-        X: Union[dict, str],
-        file_type: str = "h5py",
+        test_set: Union[dict, str],
+        file_type: str = "hdf5",
     ) -> np.ndarray:
         """Classify the input data with the trained model.
 
-        Warnings
-        --------
-        The method classify is deprecated. Please use `predict()` instead.
+
 
         Parameters
         ----------
-        X :
-            The data samples for testing, should be array-like of shape [n_samples, sequence length (time steps),
+        test_set :
+            The data samples for testing, should be array-like of shape [n_samples, sequence length (n_steps),
             n_features], or a path string locating a data file, e.g. h5 file.
 
         file_type :
             The type of the given file if X is a path string.
 
         Returns
         -------
         array-like, shape [n_samples],
             Classification results of the given samples.
         """
-        # this is for old API compatibility, will be removed in the future.
-        # Please implement predict() instead.
+
         raise NotImplementedError
```

### Comparing `pypots-0.4.1/pypots/classification/brits/__init__.py` & `pypots-0.5/pypots/imputation/crossformer/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,19 +1,24 @@
 """
-The package of the partially-observed time-series classification model BRITS.
+The package of the partially-observed time-series imputation model Transformer.
 
 Refer to the paper
-`Wei Cao, Dong Wang, Jian Li, Hao Zhou, Lei Li, and Yitan Li.
-BRITS: Bidirectional recurrent imputation for time series.
-In Advances in Neural Information Processing Systems, volume 31. Curran Associates, Inc., 2018.
-<https://papers.nips.cc/paper_files/paper/2018/file/734e6bfcd358e25ac1db0a4241b95651-Paper.pdf>`_
+`Yunhao Zhang and Junchi Yan.
+Crossformer: Transformer utilizing cross-dimension dependency for multivariate time series forecasting.
+In The 11th ICLR, 2023.
+<https://openreview.net/pdf?id=vSVLM2j9eie>`_
+
+Notes
+-----
+This implementation is inspired by the official one https://github.com/Thinklab-SJTU/Crossformer
 
 """
 
 # Created by Wenjie Du <wenjay.du@gmail.com>
 # License: BSD-3-Clause
 
-from .model import BRITS
+
+from .model import Crossformer
 
 __all__ = [
-    "BRITS",
+    "Crossformer",
 ]
```

### Comparing `pypots-0.4.1/pypots/classification/brits/core.py` & `pypots-0.5/pypots/imputation/brits/core.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,89 +1,71 @@
 """
-The implementation of BRITS for the partially-observed time-series classification task.
-
-Refer to the paper "Cao, W., Wang, D., Li, J., Zhou, H., Li, L., & Li, Y. (2018).
-BRITS: Bidirectional Recurrent Imputation for Time Series. NeurIPS 2018."
-
-Notes
------
-Partial implementation uses code from https://github.com/caow13/BRITS. The bugs in the original implementation
-are fixed here.
-
+The core wrapper assembles the submodules of BRITS imputation model
+and takes over the forward progress of the algorithm.
 """
 
 # Created by Wenjie Du <wenjay.du@gmail.com>
 # License: BSD-3-Clause
 
-import torch
 import torch.nn as nn
-import torch.nn.functional as F
 
 from ...nn.modules.brits import BackboneBRITS
 
 
 class _BRITS(nn.Module):
+    """model BRITS: Bidirectional RITS
+    BRITS consists of two RITS, which take time-series data from two directions (forward/backward) respectively.
+
+    Parameters
+    ----------
+    n_steps :
+        sequence length (number of time steps)
+
+    n_features :
+        number of features (input dimensions)
+
+    rnn_hidden_size :
+        the hidden size of the RNN cell
+
+    """
+
     def __init__(
         self,
         n_steps: int,
         n_features: int,
         rnn_hidden_size: int,
-        n_classes: int,
-        classification_weight: float,
-        reconstruction_weight: float,
     ):
         super().__init__()
         self.n_steps = n_steps
         self.n_features = n_features
         self.rnn_hidden_size = rnn_hidden_size
-        self.n_classes = n_classes
-        self.classification_weight = classification_weight
-        self.reconstruction_weight = reconstruction_weight
 
-        # create models
         self.model = BackboneBRITS(n_steps, n_features, rnn_hidden_size)
-        self.f_classifier = nn.Linear(self.rnn_hidden_size, n_classes)
-        self.b_classifier = nn.Linear(self.rnn_hidden_size, n_classes)
 
     def forward(self, inputs: dict, training: bool = True) -> dict:
         (
             imputed_data,
             f_reconstruction,
             b_reconstruction,
             f_hidden_states,
             b_hidden_states,
             consistency_loss,
             reconstruction_loss,
         ) = self.model(inputs)
 
-        f_logits = self.f_classifier(f_hidden_states)
-        b_logits = self.b_classifier(b_hidden_states)
-        f_prediction = torch.softmax(f_logits, dim=1)
-        b_prediction = torch.softmax(b_logits, dim=1)
-        classification_pred = (f_prediction + b_prediction) / 2
-
         results = {
             "imputed_data": imputed_data,
-            "classification_pred": classification_pred,
         }
 
         # if in training mode, return results with losses
         if training:
             results["consistency_loss"] = consistency_loss
             results["reconstruction_loss"] = reconstruction_loss
-            f_classification_loss = F.nll_loss(torch.log(f_prediction), inputs["label"])
-            b_classification_loss = F.nll_loss(torch.log(b_prediction), inputs["label"])
-            classification_loss = (f_classification_loss + b_classification_loss) / 2
-            loss = (
-                consistency_loss
-                + reconstruction_loss * self.reconstruction_weight
-                + classification_loss * self.classification_weight
-            )
+            loss = consistency_loss + reconstruction_loss
 
             # `loss` is always the item for backward propagating to update the model
             results["loss"] = loss
             results["reconstruction"] = (f_reconstruction + b_reconstruction) / 2
-            results["classification_loss"] = classification_loss
             results["f_reconstruction"] = f_reconstruction
             results["b_reconstruction"] = b_reconstruction
 
         return results
```

### Comparing `pypots-0.4.1/pypots/classification/brits/data.py` & `pypots-0.5/pypots/classification/raindrop/data.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,48 +1,47 @@
 """
-Dataset class for model BRITS.
+Dataset class for the classification model Raindrop.
 """
 
 # Created by Wenjie Du <wenjay.du@gmail.com>
 # License: BSD-3-Clause
 
+
 from typing import Union
 
-from ...imputation.brits.data import (
-    DatasetForBRITS as DatasetForBRITS_Imputation,
-)
+from ..grud.data import DatasetForGRUD
 
 
-class DatasetForBRITS(DatasetForBRITS_Imputation):
-    """Dataset class for BRITS.
+class DatasetForRaindrop(DatasetForGRUD):
+    """Dataset class for model GRU-D.
 
     Parameters
     ----------
-    data : dict or str,
+    data :
         The dataset for model input, should be a dictionary including keys as 'X' and 'y',
         or a path string locating a data file.
-        If it is a dict, X should be array-like of shape [n_samples, sequence length (time steps), n_features],
+        If it is a dict, X should be array-like of shape [n_samples, sequence length (n_steps), n_features],
         which is time-series data for input, can contain missing values, and y should be array-like of shape
         [n_samples], which is classification labels of X.
         If it is a path string, the path should point to a data file, e.g. a h5 file, which contains
         key-value pairs like a dict, and it has to include keys as 'X' and 'y'.
 
-    return_labels : bool, default = True,
+    return_y :
         Whether to return labels in function __getitem__() if they exist in the given data. If `True`, for example,
         during training of classification models, the Dataset class will return labels in __getitem__() for model input.
         Otherwise, labels won't be included in the data returned by __getitem__(). This parameter exists because we
         need the defined Dataset class for all training/validating/testing stages. For those big datasets stored in h5
         files, they already have both X and y saved. But we don't read labels from the file for validating and testing
         with function _fetch_data_from_file(), which works for all three stages. Therefore, we need this parameter for
         distinction.
 
-    file_type : str, default = "h5py"
+    file_type :
         The type of the given file if train_set and val_set are path strings.
     """
 
     def __init__(
         self,
         data: Union[dict, str],
-        return_labels: bool = True,
-        file_type: str = "h5py",
+        return_y: bool = True,
+        file_type: str = "hdf5",
     ):
-        super().__init__(data, False, return_labels, file_type)
+        super().__init__(data, return_y, file_type)
```

### Comparing `pypots-0.4.1/pypots/classification/brits/model.py` & `pypots-0.5/pypots/classification/brits/model.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,10 @@
 """
 The implementation of BRITS for the partially-observed time-series classification task.
 
-Refer to the paper "Wei Cao, Dong Wang, Jian Li, Hao Zhou, Lei Li, and Yitan Li.
-BRITS: Bidirectional recurrent imputation for time series.
-In Advances in Neural Information Processing Systems, volume 31. Curran Associates, Inc., 2018."
-
-Notes
------
-Partial implementation uses code from https://github.com/caow13/BRITS.
-The bugs in the original implementation are fixed here.
-
 """
 
 # Created by Wenjie Du <wenjay.du@gmail.com>
 # License: BSD-3-Clause
 
 from typing import Optional, Union
 
@@ -22,15 +13,14 @@
 from torch.utils.data import DataLoader
 
 from .core import _BRITS
 from .data import DatasetForBRITS
 from ..base import BaseNNClassifier
 from ...optim.adam import Adam
 from ...optim.base import Optimizer
-from ...utils.logging import logger
 
 
 class BRITS(BaseNNClassifier):
     """The PyTorch implementation of the BRITS model :cite:`cao2018BRITS`.
 
     Parameters
     ----------
@@ -204,15 +194,15 @@
         }
         return inputs
 
     def fit(
         self,
         train_set: Union[dict, str],
         val_set: Optional[Union[dict, str]] = None,
-        file_type: str = "h5py",
+        file_type: str = "hdf5",
     ) -> None:
         # Step 1: wrap the input data with classes Dataset and DataLoader
         training_set = DatasetForBRITS(train_set, file_type=file_type)
         training_loader = DataLoader(
             training_set,
             batch_size=self.batch_size,
             shuffle=True,
@@ -235,18 +225,18 @@
 
         # Step 3: save the model if necessary
         self._auto_save_model_if_necessary(confirm_saving=True)
 
     def predict(
         self,
         test_set: Union[dict, str],
-        file_type: str = "h5py",
+        file_type: str = "hdf5",
     ) -> dict:
         self.model.eval()  # set the model as eval status to freeze it.
-        test_set = DatasetForBRITS(test_set, return_labels=False, file_type=file_type)
+        test_set = DatasetForBRITS(test_set, return_y=False, file_type=file_type)
         test_loader = DataLoader(
             test_set,
             batch_size=self.batch_size,
             shuffle=False,
             num_workers=self.num_workers,
         )
         classification_collector = []
@@ -262,35 +252,29 @@
         result_dict = {
             "classification": classification,
         }
         return result_dict
 
     def classify(
         self,
-        X: Union[dict, str],
-        file_type: str = "h5py",
+        test_set: Union[dict, str],
+        file_type: str = "hdf5",
     ) -> np.ndarray:
         """Classify the input data with the trained model.
 
-        Warnings
-        --------
-        The method classify is deprecated. Please use `predict()` instead.
-
         Parameters
         ----------
-        X :
-            The data samples for testing, should be array-like of shape [n_samples, sequence length (time steps),
+        test_set :
+            The data samples for testing, should be array-like of shape [n_samples, sequence length (n_steps),
             n_features], or a path string locating a data file, e.g. h5 file.
 
         file_type :
             The type of the given file if X is a path string.
 
         Returns
         -------
         array-like, shape [n_samples],
             Classification results of the given samples.
         """
-        logger.warning(
-            "🚨DeprecationWarning: The method classify is deprecated. Please use `predict` instead."
-        )
-        result_dict = self.predict(X, file_type=file_type)
+
+        result_dict = self.predict(test_set, file_type=file_type)
         return result_dict["classification"]
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pypots-0.4.1/pypots/classification/grud/core.py` & `pypots-0.5/pypots/imputation/autoformer/core.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,83 +1,87 @@
 """
-The implementation of GRU-D for the partially-observed time-series imputation task.
-
-Refer to the paper "Che, Z., Purushotham, S., Cho, K., Sontag, D.A., & Liu, Y. (2018).
-Recurrent Neural Networks for Multivariate Time Series with Missing Values. Scientific Reports."
-
+The core wrapper assembles the submodules of Autoformer imputation model
+and takes over the forward progress of the algorithm.
 """
 
 # Created by Wenjie Du <wenjay.du@gmail.com>
 # License: BSD-3-Clause
 
-
-from typing import Union
-
-import torch
 import torch.nn as nn
-import torch.nn.functional as F
 
-from ...nn.modules.grud import BackboneGRUD
+from ...nn.modules.autoformer import AutoformerEncoder
+from ...nn.modules.saits import SaitsLoss, SaitsEmbedding
 
 
-class _GRUD(nn.Module):
+class _Autoformer(nn.Module):
     def __init__(
         self,
-        n_steps: int,
-        n_features: int,
-        rnn_hidden_size: int,
-        n_classes: int,
-        device: Union[str, torch.device],
+        n_steps,
+        n_features,
+        n_layers,
+        d_model,
+        n_heads,
+        d_ffn,
+        factor,
+        moving_avg_window_size,
+        dropout,
+        ORT_weight: float = 1,
+        MIT_weight: float = 1,
+        activation="relu",
     ):
         super().__init__()
+
         self.n_steps = n_steps
-        self.n_features = n_features
-        self.rnn_hidden_size = rnn_hidden_size
-        self.n_classes = n_classes
-        self.device = device
-
-        # create models
-        self.model = BackboneGRUD(
-            n_steps,
-            n_features,
-            rnn_hidden_size,
-        )
-        self.classifier = nn.Linear(self.rnn_hidden_size, self.n_classes)
 
-    def forward(self, inputs: dict, training: bool = True) -> dict:
-        """Forward processing of GRU-D.
+        self.saits_embedding = SaitsEmbedding(
+            n_features * 2,
+            d_model,
+            with_pos=False,
+            dropout=dropout,
+        )
+        self.encoder = AutoformerEncoder(
+            n_layers,
+            d_model,
+            n_heads,
+            d_ffn,
+            factor,
+            moving_avg_window_size,
+            dropout,
+            activation,
+        )
 
-        Parameters
-        ----------
-        inputs :
-            The input data.
-
-        training :
-            Whether in training mode.
-
-        Returns
-        -------
-        dict,
-            A dictionary includes all results.
-        """
-        X = inputs["X"]
-        missing_mask = inputs["missing_mask"]
-        deltas = inputs["deltas"]
-        empirical_mean = inputs["empirical_mean"]
-        X_filledLOCF = inputs["X_filledLOCF"]
+        # for the imputation task, the output dim is the same as input dim
+        self.output_projection = nn.Linear(d_model, n_features)
+        self.saits_loss_func = SaitsLoss(ORT_weight, MIT_weight)
 
-        _, hidden_state = self.model(
-            X, missing_mask, deltas, empirical_mean, X_filledLOCF
-        )
+    def forward(self, inputs: dict, training: bool = True) -> dict:
+        X, missing_mask = inputs["X"], inputs["missing_mask"]
 
-        logits = self.classifier(hidden_state)
-        classification_pred = torch.softmax(logits, dim=1)
-        results = {"classification_pred": classification_pred}
+        # WDU: the original Autoformer paper isn't proposed for imputation task. Hence the model doesn't take
+        # the missing mask into account, which means, in the process, the model doesn't know which part of
+        # the input data is missing, and this may hurt the model's imputation performance. Therefore, I apply the
+        # SAITS embedding method to project the concatenation of features and masks into a hidden space, as well as
+        # the output layers to project back from the hidden space to the original space.
+        enc_out = self.saits_embedding(X, missing_mask)
+
+        # Autoformer encoder processing
+        enc_out, attns = self.encoder(enc_out)
+        # project back the original data space
+        reconstruction = self.output_projection(enc_out)
+
+        imputed_data = missing_mask * X + (1 - missing_mask) * reconstruction
+        results = {
+            "imputed_data": imputed_data,
+        }
 
         # if in training mode, return results with losses
         if training:
-            classification_loss = F.nll_loss(
-                torch.log(classification_pred), inputs["label"]
+            X_ori, indicating_mask = inputs["X_ori"], inputs["indicating_mask"]
+            loss, ORT_loss, MIT_loss = self.saits_loss_func(
+                reconstruction, X_ori, missing_mask, indicating_mask
             )
-            results["loss"] = classification_loss
+            results["ORT_loss"] = ORT_loss
+            results["MIT_loss"] = MIT_loss
+            # `loss` is always the item for backward propagating to update the model
+            results["loss"] = loss
 
         return results
```

### Comparing `pypots-0.4.1/pypots/classification/grud/data.py` & `pypots-0.5/pypots/classification/grud/data.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,78 +1,84 @@
 """
-Dataset class for model GRU-D.
+Dataset class for the classification model GRU-D.
 """
 
 # Created by Wenjie Du <wenjay.du@gmail.com>
 # License: BSD-3-Clause
 
 
 from typing import Union, Iterable
 
 import torch
 
-from ...data.base import BaseDataset
+from ...data.dataset import BaseDataset
 from ...data.utils import _parse_delta_torch
 from ...imputation.locf import locf_torch
 
 
 class DatasetForGRUD(BaseDataset):
     """Dataset class for model GRU-D.
 
     Parameters
     ----------
-    data : dict or str,
+    data :
         The dataset for model input, should be a dictionary including keys as 'X' and 'y',
         or a path string locating a data file.
-        If it is a dict, X should be array-like of shape [n_samples, sequence length (time steps), n_features],
+        If it is a dict, X should be array-like of shape [n_samples, sequence length (n_steps), n_features],
         which is time-series data for input, can contain missing values, and y should be array-like of shape
         [n_samples], which is classification labels of X.
         If it is a path string, the path should point to a data file, e.g. a h5 file, which contains
         key-value pairs like a dict, and it has to include keys as 'X' and 'y'.
 
-    return_labels : bool, default = True,
+    return_y :
         Whether to return labels in function __getitem__() if they exist in the given data. If `True`, for example,
         during training of classification models, the Dataset class will return labels in __getitem__() for model input.
         Otherwise, labels won't be included in the data returned by __getitem__(). This parameter exists because we
         need the defined Dataset class for all training/validating/testing stages. For those big datasets stored in h5
         files, they already have both X and y saved. But we don't read labels from the file for validating and testing
         with function _fetch_data_from_file(), which works for all three stages. Therefore, we need this parameter for
         distinction.
 
-    file_type : str, default = "h5py"
+    file_type :
         The type of the given file if train_set and val_set are path strings.
     """
 
     def __init__(
         self,
         data: Union[dict, str],
-        return_labels: bool = True,
-        file_type: str = "h5py",
+        return_y: bool = True,
+        file_type: str = "hdf5",
     ):
-        super().__init__(data, False, return_labels, file_type)
+        super().__init__(
+            data=data,
+            return_X_ori=False,
+            return_X_pred=False,
+            return_y=return_y,
+            file_type=file_type,
+        )
         if not isinstance(self.data, str):  # data from array
             self.missing_mask = (~torch.isnan(self.X)).to(torch.float32)
             self.X_filledLOCF = locf_torch(self.X)
             self.X = torch.nan_to_num(self.X)
             self.deltas = _parse_delta_torch(self.missing_mask)
             self.empirical_mean = torch.sum(
                 self.missing_mask * self.X, dim=[0, 1]
             ) / torch.sum(self.missing_mask, dim=[0, 1])
 
     def _fetch_data_from_array(self, idx: int) -> Iterable:
         """Fetch data according to index.
 
         Parameters
         ----------
-        idx : int,
+        idx :
             The index to fetch the specified sample.
 
         Returns
         -------
-        sample : list,
+        sample :
             A list contains
 
             index : int tensor,
                 The index of the sample.
 
             X : tensor,
                 The feature vector for model input.
@@ -94,31 +100,31 @@
             self.X[idx].to(torch.float32),
             self.X_filledLOCF[idx].to(torch.float32),
             self.missing_mask[idx].to(torch.float32),
             self.deltas[idx].to(torch.float32),
             self.empirical_mean.to(torch.float32),
         ]
 
-        if self.y is not None and self.return_labels:
+        if self.return_y:
             sample.append(self.y[idx].to(torch.long))
 
         return sample
 
     def _fetch_data_from_file(self, idx: int) -> Iterable:
         """Fetch data with the lazy-loading strategy, i.e. only loading data from the file while requesting for samples.
         Here the opened file handle doesn't load the entire dataset into RAM but only load the currently accessed slice.
 
         Parameters
         ----------
-        idx : int,
+        idx :
             The index of the sample to be return.
 
         Returns
         -------
-        sample : list,
+        sample :
             The collated data sample, a list including all necessary sample info.
         """
 
         if self.file_handle is None:
             self.file_handle = self._open_file_handle()
 
         X = torch.from_numpy(self.file_handle["X"][idx]).to(torch.float32)
@@ -136,11 +142,11 @@
             X_filledLOCF,
             missing_mask,
             deltas,
             empirical_mean,
         ]
 
         # if the dataset has labels and is for training, then fetch it from the file
-        if "y" in self.file_handle.keys() and self.return_labels:
+        if self.return_y:
             sample.append(torch.tensor(self.file_handle["y"][idx], dtype=torch.long))
 
         return sample
```

### Comparing `pypots-0.4.1/pypots/classification/grud/model.py` & `pypots-0.5/pypots/classification/grud/model.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,10 @@
 """
 The implementation of GRU-D for the partially-observed time-series classification task.
 
-Refer to the paper "Zhengping Che, Sanjay Purushotham, Kyunghyun Cho, David Sontag, and Yan Liu.
-Recurrent Neural Networks for Multivariate Time Series with Missing Values.
-Scientific Reports, 8(1):6085, April 2018."
-
 """
 
 # Created by Wenjie Du <wenjay.du@gmail.com>
 # License: BSD-3-Clause
 
 
 from typing import Union, Optional
@@ -18,15 +14,14 @@
 from torch.utils.data import DataLoader
 
 from .core import _GRUD
 from .data import DatasetForGRUD
 from ..base import BaseNNClassifier
 from ...optim.adam import Adam
 from ...optim.base import Optimizer
-from ...utils.logging import logger
 
 
 class GRUD(BaseNNClassifier):
     """The PyTorch implementation of the GRU-D model :cite:`che2018GRUD`.
 
     Parameters
     ----------
@@ -176,15 +171,15 @@
 
         return inputs
 
     def fit(
         self,
         train_set: Union[dict, str],
         val_set: Optional[Union[dict, str]] = None,
-        file_type: str = "h5py",
+        file_type: str = "hdf5",
     ) -> None:
         # Step 1: wrap the input data with classes Dataset and DataLoader
         training_set = DatasetForGRUD(train_set, file_type=file_type)
         training_loader = DataLoader(
             training_set,
             batch_size=self.batch_size,
             shuffle=True,
@@ -207,18 +202,18 @@
 
         # Step 3: save the model if necessary
         self._auto_save_model_if_necessary(confirm_saving=True)
 
     def predict(
         self,
         test_set: Union[dict, str],
-        file_type: str = "h5py",
+        file_type: str = "hdf5",
     ) -> dict:
         self.model.eval()  # set the model as eval status to freeze it.
-        test_set = DatasetForGRUD(test_set, return_labels=False, file_type=file_type)
+        test_set = DatasetForGRUD(test_set, return_y=False, file_type=file_type)
         test_loader = DataLoader(
             test_set,
             batch_size=self.batch_size,
             shuffle=False,
             num_workers=self.num_workers,
         )
         classification_collector = []
@@ -234,35 +229,29 @@
         result_dict = {
             "classification": classification,
         }
         return result_dict
 
     def classify(
         self,
-        X: Union[dict, str],
-        file_type: str = "h5py",
+        test_set: Union[dict, str],
+        file_type: str = "hdf5",
     ) -> np.ndarray:
         """Classify the input data with the trained model.
 
-        Warnings
-        --------
-        The method classify is deprecated. Please use `predict()` instead.
-
         Parameters
         ----------
-        X :
-            The data samples for testing, should be array-like of shape [n_samples, sequence length (time steps),
+        test_set :
+            The data samples for testing, should be array-like of shape [n_samples, sequence length (n_steps),
             n_features], or a path string locating a data file, e.g. h5 file.
 
         file_type :
             The type of the given file if X is a path string.
 
         Returns
         -------
         array-like, shape [n_samples],
             Classification results of the given samples.
         """
-        logger.warning(
-            "🚨DeprecationWarning: The method classify is deprecated. Please use `predict` instead."
-        )
-        result_dict = self.predict(X, file_type=file_type)
+
+        result_dict = self.predict(test_set, file_type=file_type)
         return result_dict["classification"]
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pypots-0.4.1/pypots/classification/raindrop/core.py` & `pypots-0.5/pypots/classification/raindrop/core.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,10 @@
 """
-The implementation of Raindrop for the partially-observed time-series classification task.
-
-Refer to the paper "Zhang, X., Zeman, M., Tsiligkaridis, T., & Zitnik, M. (2022).
-Graph-Guided Network for Irregularly Sampled Multivariate Time Series. ICLR 2022."
-
+The core wrapper assembles the submodules of Raindrop classification model
+and takes over the forward progress of the algorithm.
 """
 
 
 # Created by Wenjie Du <wenjay.du@gmail.com>
 # License: BSD-3-Clause
 
 
@@ -20,16 +17,16 @@
 
 class _Raindrop(nn.Module):
     def __init__(
         self,
         n_features,
         n_layers,
         d_model,
-        d_ffn,
         n_heads,
+        d_ffn,
         n_classes,
         dropout=0.3,
         max_len=215,
         d_static=9,
         aggregation="mean",
         sensor_wise_mask=False,
         static=False,
@@ -40,16 +37,16 @@
         self.aggregation = aggregation
         self.sensor_wise_mask = sensor_wise_mask
 
         self.backbone = BackboneRaindrop(
             n_features,
             n_layers,
             d_model,
-            d_ffn,
             n_heads,
+            d_ffn,
             n_classes,
             dropout,
             max_len,
             d_static,
             d_pe,
             aggregation,
             sensor_wise_mask,
```

### Comparing `pypots-0.4.1/pypots/classification/raindrop/data.py` & `pypots-0.5/pypots/imputation/usgan/data.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,47 +1,52 @@
 """
-Dataset class for model Raindrop.
+Dataset class for the imputation model USGAN.
 """
 
-# Created by Wenjie Du <wenjay.du@gmail.com>
+# Created by Jun Wang <jwangfx@connect.ust.hk> and Wenjie Du <wenjay.du@gmail.com>
 # License: BSD-3-Clause
 
-
 from typing import Union
 
-from ..grud.data import DatasetForGRUD
+from ..brits.data import DatasetForBRITS
 
 
-class DatasetForRaindrop(DatasetForGRUD):
-    """Dataset class for model GRU-D.
+class DatasetForUSGAN(DatasetForBRITS):
+    """Dataset class for USGAN, the same with the one for BRITS.
 
     Parameters
     ----------
-    data : dict or str,
+    data :
         The dataset for model input, should be a dictionary including keys as 'X' and 'y',
         or a path string locating a data file.
-        If it is a dict, X should be array-like of shape [n_samples, sequence length (time steps), n_features],
+        If it is a dict, X should be array-like of shape [n_samples, sequence length (n_steps), n_features],
         which is time-series data for input, can contain missing values, and y should be array-like of shape
         [n_samples], which is classification labels of X.
         If it is a path string, the path should point to a data file, e.g. a h5 file, which contains
         key-value pairs like a dict, and it has to include keys as 'X' and 'y'.
 
-    return_labels : bool, default = True,
+    return_y :
         Whether to return labels in function __getitem__() if they exist in the given data. If `True`, for example,
         during training of classification models, the Dataset class will return labels in __getitem__() for model input.
         Otherwise, labels won't be included in the data returned by __getitem__(). This parameter exists because we
         need the defined Dataset class for all training/validating/testing stages. For those big datasets stored in h5
         files, they already have both X and y saved. But we don't read labels from the file for validating and testing
         with function _fetch_data_from_file(), which works for all three stages. Therefore, we need this parameter for
         distinction.
 
-    file_type : str, default = "h5py"
+    file_type :
         The type of the given file if train_set and val_set are path strings.
     """
 
     def __init__(
         self,
         data: Union[dict, str],
-        return_labels: bool = True,
-        file_type: str = "h5py",
+        return_X_ori: bool,
+        return_y: bool,
+        file_type: str = "hdf5",
     ):
-        super().__init__(data, return_labels, file_type)
+        super().__init__(
+            data=data,
+            return_X_ori=return_X_ori,
+            return_y=return_y,
+            file_type=file_type,
+        )
```

### Comparing `pypots-0.4.1/pypots/classification/raindrop/model.py` & `pypots-0.5/pypots/classification/raindrop/model.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,33 +1,28 @@
 """
 The implementation of Raindrop for the partially-observed time-series classification task.
 
-Refer to the paper "Xiang Zhang, Marko Zeman, Theodoros Tsiligkaridis, and Marinka Zitnik.
-Graph-guided network for irregularly sampled multivariate time series.
-In ICLR, 2022."
-
 """
 
 
 # Created by Wenjie Du <wenjay.du@gmail.com>
 # License: BSD-3-Clause
 
 
 from typing import Union, Optional
 
 import numpy as np
 import torch
 from torch.utils.data import DataLoader
 
 from .core import _Raindrop
+from .data import DatasetForRaindrop
 from ...classification.base import BaseNNClassifier
-from ...classification.grud.data import DatasetForGRUD
 from ...optim.adam import Adam
 from ...optim.base import Optimizer
-from ...utils.logging import logger
 
 
 class Raindrop(BaseNNClassifier):
     """The PyTorch implementation of the Raindrop model :cite:`zhang2022Raindrop`.
 
     Parameters
     ----------
@@ -43,20 +38,20 @@
     n_layers :
         The number of layers in the Transformer encoder in the Raindrop model.
 
     d_model :
         The dimension of the Transformer encoder backbone.
         It is the input dimension of the multi-head self-attention layers.
 
-    d_ffn :
-        The dimension of the layer in the Feed-Forward Networks (FFN).
-
     n_heads :
         The number of heads in the multi-head self-attention mechanism.
 
+    d_ffn :
+        The dimension of the layer in the Feed-Forward Networks (FFN).
+
     dropout :
         The dropout rate for all fully-connected layers in the model.
 
     d_static :
         The dimension of the static features.
 
     aggregation :
@@ -112,16 +107,16 @@
     def __init__(
         self,
         n_steps,
         n_features,
         n_classes,
         n_layers,
         d_model,
-        d_ffn,
         n_heads,
+        d_ffn,
         dropout,
         d_static=0,
         aggregation="mean",
         sensor_wise_mask=False,
         static=False,
         batch_size=32,
         epochs=100,
@@ -147,16 +142,16 @@
         self.n_steps = n_steps
 
         # set up the model
         self.model = _Raindrop(
             n_features,
             n_layers,
             d_model,
-            d_ffn,
             n_heads,
+            d_ffn,
             n_classes,
             dropout,
             n_steps,
             d_static,
             aggregation,
             sensor_wise_mask,
             static,
@@ -220,27 +215,27 @@
 
         return inputs
 
     def fit(
         self,
         train_set: Union[dict, str],
         val_set: Optional[Union[dict, str]] = None,
-        file_type="h5py",
+        file_type: str = "hdf5",
     ) -> None:
         # Step 1: wrap the input data with classes Dataset and DataLoader
-        training_set = DatasetForGRUD(train_set, file_type=file_type)
+        training_set = DatasetForRaindrop(train_set, file_type=file_type)
         training_loader = DataLoader(
             training_set,
             batch_size=self.batch_size,
             shuffle=True,
             num_workers=self.num_workers,
         )
         val_loader = None
         if val_set is not None:
-            val_set = DatasetForGRUD(val_set, file_type=file_type)
+            val_set = DatasetForRaindrop(val_set, file_type=file_type)
             val_loader = DataLoader(
                 val_set,
                 batch_size=self.batch_size,
                 shuffle=False,
                 num_workers=self.num_workers,
             )
 
@@ -251,18 +246,18 @@
 
         # Step 3: save the model if necessary
         self._auto_save_model_if_necessary(confirm_saving=True)
 
     def predict(
         self,
         test_set: Union[dict, str],
-        file_type: str = "h5py",
+        file_type: str = "hdf5",
     ) -> dict:
         self.model.eval()  # set the model as eval status to freeze it.
-        test_set = DatasetForGRUD(test_set, return_labels=False, file_type=file_type)
+        test_set = DatasetForRaindrop(test_set, return_y=False, file_type=file_type)
         test_loader = DataLoader(
             test_set,
             batch_size=self.batch_size,
             shuffle=False,
             num_workers=self.num_workers,
         )
 
@@ -279,35 +274,29 @@
         result_dict = {
             "classification": classification,
         }
         return result_dict
 
     def classify(
         self,
-        X: Union[dict, str],
-        file_type: str = "h5py",
+        test_set: Union[dict, str],
+        file_type: str = "hdf5",
     ) -> np.ndarray:
         """Classify the input data with the trained model.
 
-        Warnings
-        --------
-        The method classify is deprecated. Please use `predict()` instead.
-
         Parameters
         ----------
-        X :
-            The data samples for testing, should be array-like of shape [n_samples, sequence length (time steps),
+        test_set :
+            The data samples for testing, should be array-like of shape [n_samples, sequence length (n_steps),
             n_features], or a path string locating a data file, e.g. h5 file.
 
         file_type :
             The type of the given file if X is a path string.
 
         Returns
         -------
         array-like, shape [n_samples],
             Classification results of the given samples.
         """
-        logger.warning(
-            "🚨DeprecationWarning: The method classify is deprecated. Please use `predict` instead."
-        )
-        result_dict = self.predict(X, file_type=file_type)
+
+        result_dict = self.predict(test_set, file_type=file_type)
         return result_dict["classification"]
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pypots-0.4.1/pypots/cli/base.py` & `pypots-0.5/pypots/cli/base.py`

 * *Files identical despite different names*

### Comparing `pypots-0.4.1/pypots/cli/dev.py` & `pypots-0.5/pypots/cli/dev.py`

 * *Files identical despite different names*

### Comparing `pypots-0.4.1/pypots/cli/doc.py` & `pypots-0.5/pypots/cli/doc.py`

 * *Files identical despite different names*

### Comparing `pypots-0.4.1/pypots/cli/env.py` & `pypots-0.5/pypots/cli/env.py`

 * *Files identical despite different names*

### Comparing `pypots-0.4.1/pypots/cli/pypots_cli.py` & `pypots-0.5/pypots/cli/pypots_cli.py`

 * *Files identical despite different names*

### Comparing `pypots-0.4.1/pypots/cli/tuning.py` & `pypots-0.5/pypots/cli/tuning.py`

 * *Files identical despite different names*

### Comparing `pypots-0.4.1/pypots/cli/utils.py` & `pypots-0.5/pypots/cli/utils.py`

 * *Files identical despite different names*

### Comparing `pypots-0.4.1/pypots/clustering/base.py` & `pypots-0.5/pypots/clustering/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -68,32 +68,32 @@
         self.n_clusters = n_clusters
 
     @abstractmethod
     def fit(
         self,
         train_set: Union[dict, str],
         val_set: Union[dict, str] = None,
-        file_type: str = "h5py",
+        file_type: str = "hdf5",
     ) -> None:
         """Train the cluster.
 
         Parameters
         ----------
         train_set :
             The dataset for model training, should be a dictionary including the key 'X',
             or a path string locating a data file.
-            If it is a dict, X should be array-like of shape [n_samples, sequence length (time steps), n_features],
+            If it is a dict, X should be array-like of shape [n_samples, sequence length (n_steps), n_features],
             which is time-series data for training, can contain missing values.
             If it is a path string, the path should point to a data file, e.g. a h5 file, which contains
             key-value pairs like a dict, and it has to include the key 'X'.
 
         val_set :
             The dataset for model validating, should be a dictionary including keys as 'X' and 'y',
             or a path string locating a data file.
-            If it is a dict, X should be array-like of shape [n_samples, sequence length (time steps), n_features],
+            If it is a dict, X should be array-like of shape [n_samples, sequence length (n_steps), n_features],
             which is time-series data for validating, can contain missing values, and y should be array-like of shape
             [n_samples], which is classification labels of X.
             If it is a path string, the path should point to a data file, e.g. a h5 file, which contains
             key-value pairs like a dict, and it has to include keys as 'X' and 'y'.
 
         file_type :
             The type of the given file if train_set and val_set are path strings.
@@ -101,42 +101,41 @@
         """
         raise NotImplementedError
 
     @abstractmethod
     def predict(
         self,
         test_set: Union[dict, str],
-        file_type: str = "h5py",
+        file_type: str = "hdf5",
     ) -> dict:
         raise NotImplementedError
 
     @abstractmethod
     def cluster(
         self,
-        X: Union[dict, str],
-        file_type="h5py",
+        test_set: Union[dict, str],
+        file_type: str = "hdf5",
     ) -> np.ndarray:
         """Cluster the input with the trained model.
 
         Parameters
         ----------
-        X :
-            The data samples for testing, should be array-like of shape [n_samples, sequence length (time steps),
+        test_set :
+            The data samples for testing, should be array-like of shape [n_samples, sequence length (n_steps),
             n_features], or a path string locating a data file, e.g. h5 file.
 
         file_type :
             The type of the given file if X is a path string.
 
         Returns
         -------
         array-like,
             Clustering results.
         """
-        # this is for old API compatibility, will be removed in the future.
-        # Please implement predict() instead.
+
         raise NotImplementedError
 
 
 class BaseNNClusterer(BaseNNModel):
     """The abstract class for all neural-network clustering models in PyPOTS.
 
     Parameters
@@ -375,32 +374,32 @@
         )
 
     @abstractmethod
     def fit(
         self,
         train_set: Union[dict, str],
         val_set: Union[dict, str] = None,
-        file_type: str = "h5py",
+        file_type: str = "hdf5",
     ) -> None:
         """Train the cluster.
 
         Parameters
         ----------
         train_set :
             The dataset for model training, should be a dictionary including the key 'X',
             or a path string locating a data file.
-            If it is a dict, X should be array-like of shape [n_samples, sequence length (time steps), n_features],
+            If it is a dict, X should be array-like of shape [n_samples, sequence length (n_steps), n_features],
             which is time-series data for training, can contain missing values.
             If it is a path string, the path should point to a data file, e.g. a h5 file, which contains
             key-value pairs like a dict, and it has to include the key 'X'.
 
         val_set :
             The dataset for model validating, should be a dictionary including keys as 'X' and 'y',
             or a path string locating a data file.
-            If it is a dict, X should be array-like of shape [n_samples, sequence length (time steps), n_features],
+            If it is a dict, X should be array-like of shape [n_samples, sequence length (n_steps), n_features],
             which is time-series data for validating, can contain missing values, and y should be array-like of shape
             [n_samples], which is classification labels of X.
             If it is a path string, the path should point to a data file, e.g. a h5 file, which contains
             key-value pairs like a dict, and it has to include keys as 'X' and 'y'.
 
         file_type :
             The type of the given file if train_set and val_set are path strings.
@@ -408,40 +407,37 @@
         """
         raise NotImplementedError
 
     @abstractmethod
     def predict(
         self,
         test_set: Union[dict, str],
-        file_type: str = "h5py",
+        file_type: str = "hdf5",
     ) -> dict:
         raise NotImplementedError
 
     @abstractmethod
     def cluster(
         self,
-        X: Union[dict, str],
-        file_type="h5py",
+        test_set: Union[dict, str],
+        file_type: str = "hdf5",
     ) -> np.ndarray:
         """Cluster the input with the trained model.
 
-        Warnings
-        --------
-        The method cluster is deprecated. Please use `predict()` instead.
+
 
         Parameters
         ----------
-        X :
-            The data samples for testing, should be array-like of shape [n_samples, sequence length (time steps),
+        test_set :
+            The data samples for testing, should be array-like of shape [n_samples, sequence length (n_steps),
             n_features], or a path string locating a data file, e.g. h5 file.
 
         file_type :
             The type of the given file if X is a path string.
 
         Returns
         -------
         array-like,
             Clustering results.
         """
-        # this is for old API compatibility, will be removed in the future.
-        # Please implement predict() instead.
+
         raise NotImplementedError
```

### Comparing `pypots-0.4.1/pypots/clustering/crli/core.py` & `pypots-0.5/pypots/clustering/crli/core.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,10 @@
 """
-The implementation of CRLI (Clustering Representation Learning on Incomplete time-series data) for
-the partially-observed time-series clustering task.
-
-Refer to the paper "Ma, Q., Chen, C., Li, S., & Cottrell, G. W. (2021).
-Learning Representations for Incomplete Time Series Clustering. AAAI 2021."
-
+The core wrapper assembles the submodules of CRLI clustering model
+and takes over the forward progress of the algorithm.
 """
 
 # Created by Wenjie Du <wenjay.du@gmail.com>
 # License: BSD-3-Clause
 
 from typing import Optional
```

### Comparing `pypots-0.4.1/pypots/clustering/crli/data.py` & `pypots-0.5/pypots/clustering/crli/data.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,53 +1,59 @@
 """
-Dataset class for model GRU-D.
+Dataset class for the clustering model CRLI.
 """
 
 # Created by Wenjie Du <wenjay.du@gmail.com>
 # License: BSD-3-Clause
 
 
 from typing import Union, Iterable
 
-from ...data.base import BaseDataset
+from ...data.dataset import BaseDataset
 
 
 class DatasetForCRLI(BaseDataset):
     """Dataset class for model CRLI.
 
     Parameters
     ----------
-    data : dict or str,
+    data :
         The dataset for model input, should be a dictionary including keys as 'X' and 'y',
         or a path string locating a data file.
-        If it is a dict, X should be array-like of shape [n_samples, sequence length (time steps), n_features],
+        If it is a dict, X should be array-like of shape [n_samples, sequence length (n_steps), n_features],
         which is time-series data for input, can contain missing values, and y should be array-like of shape
         [n_samples], which is classification labels of X.
         If it is a path string, the path should point to a data file, e.g. a h5 file, which contains
         key-value pairs like a dict, and it has to include keys as 'X' and 'y'.
 
-    return_labels : bool, default = True,
+    return_y :
         Whether to return labels in function __getitem__() if they exist in the given data. If `True`, for example,
         during training of classification models, the Dataset class will return labels in __getitem__() for model input.
         Otherwise, labels won't be included in the data returned by __getitem__(). This parameter exists because we
         need the defined Dataset class for all training/validating/testing stages. For those big datasets stored in h5
         files, they already have both X and y saved. But we don't read labels from the file for validating and testing
         with function _fetch_data_from_file(), which works for all three stages. Therefore, we need this parameter for
         distinction.
 
-    file_type : str, default = "h5py"
+    file_type :
         The type of the given file if train_set and val_set are path strings.
     """
 
     def __init__(
         self,
         data: Union[dict, str],
-        return_labels: bool = True,
-        file_type: str = "h5py",
+        return_y: bool = True,
+        file_type: str = "hdf5",
     ):
-        super().__init__(data, False, return_labels, file_type)
+        super().__init__(
+            data=data,
+            return_X_ori=False,
+            return_X_pred=False,
+            return_y=return_y,
+            file_type=file_type,
+        )
 
     def _fetch_data_from_array(self, idx: int) -> Iterable:
         return super()._fetch_data_from_array(idx)
 
     def _fetch_data_from_file(self, idx: int) -> Iterable:
         return super()._fetch_data_from_file(idx)
```

### Comparing `pypots-0.4.1/pypots/clustering/crli/model.py` & `pypots-0.5/pypots/clustering/crli/model.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,11 @@
 """
 The implementation of CRLI (Clustering Representation Learning on Incomplete time-series data) for
 the partially-observed time-series clustering task.
 
-Refer to the paper "Qianli Ma, Chuxin Chen, Sen Li, and Garrison W. Cottrell.
-Learning Representations for Incomplete Time Series Clustering.
-In AAAI, 35(10):8837–8846, May 2021."
-
 """
 
 # Created by Wenjie Du <wenjay.du@gmail.com>
 # License: BSD-3-Clause
 
 import os
 from typing import Union, Optional
@@ -339,30 +335,28 @@
             f"Finished training. The best model is from epoch#{self.best_epoch}."
         )
 
     def fit(
         self,
         train_set: Union[dict, str],
         val_set: Optional[Union[dict, str]] = None,
-        file_type: str = "h5py",
+        file_type: str = "hdf5",
     ) -> None:
         # Step 1: wrap the input data with classes Dataset and DataLoader
-        training_set = DatasetForCRLI(
-            train_set, return_labels=False, file_type=file_type
-        )
+        training_set = DatasetForCRLI(train_set, return_y=False, file_type=file_type)
         training_loader = DataLoader(
             training_set,
             batch_size=self.batch_size,
             shuffle=True,
             num_workers=self.num_workers,
         )
         val_loader = None
 
         if val_set is not None:
-            val_set = DatasetForCRLI(val_set, return_labels=False, file_type=file_type)
+            val_set = DatasetForCRLI(val_set, return_y=False, file_type=file_type)
             val_loader = DataLoader(
                 val_set,
                 batch_size=self.batch_size,
                 shuffle=False,
                 num_workers=self.num_workers,
             )
 
@@ -373,46 +367,46 @@
 
         # Step 3: save the model if necessary
         self._auto_save_model_if_necessary(confirm_saving=True)
 
     def predict(
         self,
         test_set: Union[dict, str],
-        file_type: str = "h5py",
+        file_type: str = "hdf5",
         return_latent_vars: bool = False,
     ) -> dict:
         """Make predictions for the input data with the trained model.
 
         Parameters
         ----------
         test_set : dict or str
             The dataset for model validating, should be a dictionary including keys as 'X',
             or a path string locating a data file supported by PyPOTS (e.g. h5 file).
-            If it is a dict, X should be array-like of shape [n_samples, sequence length (time steps), n_features],
+            If it is a dict, X should be array-like of shape [n_samples, sequence length (n_steps), n_features],
             which is time-series data for validating, can contain missing values, and y should be array-like of shape
             [n_samples], which is classification labels of X.
             If it is a path string, the path should point to a data file, e.g. a h5 file, which contains
             key-value pairs like a dict, and it has to include keys as 'X' and 'y'.
 
-        file_type : str
+        file_type :
             The type of the given file if test_set is a path string.
 
         return_latent_vars : bool
             Whether to return the latent variables in CRLI, e.g. latent representation from the fully connected network
             in CRLI, etc.
 
         Returns
         -------
-        result_dict : dict,
+        file_type :
             The dictionary containing the clustering results and latent variables if necessary.
 
         """
 
         self.model.eval()  # set the model as eval status to freeze it.
-        test_set = DatasetForCRLI(test_set, return_labels=False, file_type=file_type)
+        test_set = DatasetForCRLI(test_set, return_y=False, file_type=file_type)
         test_loader = DataLoader(
             test_set,
             batch_size=self.batch_size,
             shuffle=False,
             num_workers=self.num_workers,
         )
         clustering_latent_collector = []
@@ -443,37 +437,30 @@
             }
             result_dict["latent_vars"] = latent_var_collector
 
         return result_dict
 
     def cluster(
         self,
-        X: Union[dict, str],
-        file_type: str = "h5py",
+        test_set: Union[dict, str],
+        file_type: str = "hdf5",
     ) -> np.ndarray:
         """Cluster the input with the trained model.
 
-        Warnings
-        --------
-        The method cluster is deprecated. Please use `predict()` instead.
-
         Parameters
         ----------
-        X :
-            The data samples for testing, should be array-like of shape [n_samples, sequence length (time steps),
+        test_set :
+            The data samples for testing, should be array-like of shape [n_samples, sequence length (n_steps),
             n_features], or a path string locating a data file, e.g. h5 file.
 
         file_type :
             The type of the given file if X is a path string.
 
         Returns
         -------
         array-like,
             Clustering results.
 
         """
-        logger.warning(
-            "🚨DeprecationWarning: The method cluster is deprecated. Please use `predict` instead."
-        )
 
-        result_dict = self.predict(X, file_type)
+        result_dict = self.predict(test_set, file_type=file_type)
         return result_dict["clustering"]
```

### Comparing `pypots-0.4.1/pypots/clustering/vader/__init__.py` & `pypots-0.5/pypots/clustering/vader/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,14 +4,18 @@
 Refer to the paper
 `Johann de Jong, Mohammad Asif Emon, Ping Wu, Reagon Karki, Meemansa Sood, Patrice Godard, Ashar Ahmad, Henri Vrooman,
 Martin Hofmann-Apitius, and Holger Fröhlich.
 Deep learning for clustering of multivariate clinical patient trajectories with missing values.
 GigaScience, 8(11):giz134, November 2019.
 <https://academic.oup.com/gigascience/article-pdf/8/11/giz134/30797160/giz134.pdf>`_
 
+Notes
+-----
+This implementation is inspired by the official one https://github.com/johanndejong/VaDER
+
 """
 
 # Created by Wenjie Du <wenjay.du@gmail.com>
 # License: BSD-3-Clause
 
 from .model import VaDER
```

### Comparing `pypots-0.4.1/pypots/clustering/vader/core.py` & `pypots-0.5/pypots/clustering/vader/core.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,22 @@
 """
-The implementation of VaDER for the partially-observed time-series clustering task.
-
-Refer to the paper "Jong, J.D., Emon, M.A., Wu, P., Karki, R., Sood, M., Godard, P., Ahmad, A., Vrooman, H.A.,
-Hofmann-Apitius, M., & Fröhlich, H. (2019).
-Deep learning for clustering of multivariate clinical patient trajectories with missing values. GigaScience."
-
+The core wrapper assembles the submodules of VaDER clustering model
+and takes over the forward progress of the algorithm.
 """
 
 # Created by Wenjie Du <wenjay.du@gmail.com>
 # License: BSD-3-Clause
 
 
 import numpy as np
 import torch
 import torch.nn as nn
 
-from pypots.utils.metrics import calc_mse
 from ...nn.modules.vader import BackboneVaDER
+from ...utils.metrics import calc_mse
 
 
 def inverse_softplus(x: np.ndarray) -> np.ndarray:
     b = x < 1e2
     x[b] = np.log(np.exp(x[b]) - 1.0 + 1e-9)
     return x
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pypots-0.4.1/pypots/clustering/vader/data.py` & `pypots-0.5/pypots/clustering/vader/data.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,53 +1,59 @@
 """
-Dataset class for model GRU-D.
+Dataset class for the clustering model VaDER.
 """
 
 # Created by Wenjie Du <wenjay.du@gmail.com>
 # License: BSD-3-Clause
 
 
 from typing import Union, Iterable
 
-from ...data.base import BaseDataset
+from ...data.dataset import BaseDataset
 
 
 class DatasetForVaDER(BaseDataset):
     """Dataset class for model VaDER.
 
     Parameters
     ----------
-    data : dict or str,
+    data :
         The dataset for model input, should be a dictionary including keys as 'X' and 'y',
         or a path string locating a data file.
-        If it is a dict, X should be array-like of shape [n_samples, sequence length (time steps), n_features],
+        If it is a dict, X should be array-like of shape [n_samples, sequence length (n_steps), n_features],
         which is time-series data for input, can contain missing values, and y should be array-like of shape
         [n_samples], which is classification labels of X.
         If it is a path string, the path should point to a data file, e.g. a h5 file, which contains
         key-value pairs like a dict, and it has to include keys as 'X' and 'y'.
 
-    return_labels : bool, default = True,
+    return_y :
         Whether to return labels in function __getitem__() if they exist in the given data. If `True`, for example,
         during training of classification models, the Dataset class will return labels in __getitem__() for model input.
         Otherwise, labels won't be included in the data returned by __getitem__(). This parameter exists because we
         need the defined Dataset class for all training/validating/testing stages. For those big datasets stored in h5
         files, they already have both X and y saved. But we don't read labels from the file for validating and testing
         with function _fetch_data_from_file(), which works for all three stages. Therefore, we need this parameter for
         distinction.
 
-    file_type : str, default = "h5py"
+    file_type :
         The type of the given file if train_set and val_set are path strings.
     """
 
     def __init__(
         self,
         data: Union[dict, str],
-        return_labels: bool = True,
-        file_type: str = "h5py",
+        return_y: bool = True,
+        file_type: str = "hdf5",
     ):
-        super().__init__(data, False, return_labels, file_type)
+        super().__init__(
+            data=data,
+            return_X_ori=False,
+            return_X_pred=False,
+            return_y=return_y,
+            file_type=file_type,
+        )
 
     def _fetch_data_from_array(self, idx: int) -> Iterable:
         return super()._fetch_data_from_array(idx)
 
     def _fetch_data_from_file(self, idx: int) -> Iterable:
         return super()._fetch_data_from_file(idx)
```

### Comparing `pypots-0.4.1/pypots/clustering/vader/model.py` & `pypots-0.5/pypots/clustering/vader/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,10 @@
 """
 The implementation of VaDER for the partially-observed time-series clustering task.
 
-Refer to the paper "Johann de Jong, Mohammad Asif Emon, Ping Wu, Reagon Karki, Meemansa Sood, Patrice Godard,
-Ashar Ahmad, Henri Vrooman, Martin Hofmann-Apitius, and Holger Fröhlich.
-Deep learning for clustering of multivariate clinical patient trajectories with missing values.
-GigaScience, 8(11):giz134, November 2019."
-
 """
 
 # Created by Wenjie Du <wenjay.du@gmail.com>
 # License: BSD-3-Clause
 
 
 import os
@@ -353,30 +348,28 @@
             f"Finished training. The best model is from epoch#{self.best_epoch}."
         )
 
     def fit(
         self,
         train_set: Union[dict, str],
         val_set: Optional[Union[dict, str]] = None,
-        file_type: str = "h5py",
+        file_type: str = "hdf5",
     ) -> None:
         # Step 1: wrap the input data with classes Dataset and DataLoader
-        training_set = DatasetForVaDER(
-            train_set, return_labels=False, file_type=file_type
-        )
+        training_set = DatasetForVaDER(train_set, return_y=False, file_type=file_type)
         training_loader = DataLoader(
             training_set,
             batch_size=self.batch_size,
             shuffle=True,
             num_workers=self.num_workers,
         )
 
         val_loader = None
         if val_set is not None:
-            val_set = DatasetForVaDER(val_set, return_labels=False, file_type=file_type)
+            val_set = DatasetForVaDER(val_set, return_y=False, file_type=file_type)
             val_loader = DataLoader(
                 val_set,
                 batch_size=self.batch_size,
                 shuffle=False,
                 num_workers=self.num_workers,
             )
 
@@ -387,44 +380,44 @@
 
         # Step 3: save the model if necessary
         self._auto_save_model_if_necessary(confirm_saving=True)
 
     def predict(
         self,
         test_set: Union[dict, str],
-        file_type: str = "h5py",
+        file_type: str = "hdf5",
         return_latent_vars: bool = False,
     ) -> dict:
         """Make predictions for the input data with the trained model.
 
         Parameters
         ----------
         test_set : dict or str
             The dataset for model validating, should be a dictionary including keys as 'X',
             or a path string locating a data file supported by PyPOTS (e.g. h5 file).
-            If it is a dict, X should be array-like of shape [n_samples, sequence length (time steps), n_features],
+            If it is a dict, X should be array-like of shape [n_samples, sequence length (n_steps), n_features],
             which is time-series data for validating, can contain missing values, and y should be array-like of shape
             [n_samples], which is classification labels of X.
             If it is a path string, the path should point to a data file, e.g. a h5 file, which contains
             key-value pairs like a dict, and it has to include keys as 'X' and 'y'.
 
-        file_type : str
+        file_type :
             The type of the given file if test_set is a path string.
 
         return_latent_vars : bool
             Whether to return the latent variables in VaDER, e.g. mu and phi, etc.
 
         Returns
         -------
-        result_dict : dict,
+        file_type :
             The dictionary containing the clustering results and latent variables if necessary.
 
         """
         self.model.eval()  # set the model as eval status to freeze it.
-        test_set = DatasetForVaDER(test_set, return_labels=False, file_type=file_type)
+        test_set = DatasetForVaDER(test_set, return_y=False, file_type=file_type)
         test_loader = DataLoader(
             test_set,
             batch_size=self.batch_size,
             shuffle=False,
             num_workers=self.num_workers,
         )
         mu_tilde_collector = []
@@ -496,37 +489,30 @@
             }
             result_dict["latent_vars"] = latent_var_collector
 
         return result_dict
 
     def cluster(
         self,
-        X: Union[dict, str],
-        file_type: str = "h5py",
+        test_set: Union[dict, str],
+        file_type: str = "hdf5",
     ) -> Union[np.ndarray]:
         """Cluster the input with the trained model.
 
-        Warnings
-        --------
-        The method cluster is deprecated. Please use `predict()` instead.
-
         Parameters
         ----------
-        X :
-            The data samples for testing, should be array-like of shape [n_samples, sequence length (time steps),
+        test_set :
+            The data samples for testing, should be array-like of shape [n_samples, sequence length (n_steps),
             n_features], or a path string locating a data file, e.g. h5 file.
 
         file_type :
             The type of the given file if X is a path string.
 
         Returns
         -------
         array-like,
             Clustering results.
 
         """
-        logger.warning(
-            "🚨DeprecationWarning: The method cluster is deprecated. Please use `predict` instead."
-        )
 
-        result_dict = self.predict(X, file_type)
+        result_dict = self.predict(test_set, file_type=file_type)
         return result_dict["clustering"]
```

### Comparing `pypots-0.4.1/pypots/data/__init__.py` & `pypots-0.5/pypots/data/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 Expose all usable data manipulation classes and functions.
 """
 
 # Created by Wenjie Du <wenjay.du@gmail.com>
 # License: BSD-3-Clause
 
-from .base import BaseDataset
+from .dataset import BaseDataset, SUPPORTED_DATASET_FILE_FORMATS
 from .generating import (
     gene_complete_random_walk,
     gene_complete_random_walk_for_anomaly_detection,
     gene_complete_random_walk_for_classification,
     gene_random_walk,
     gene_physionet2012,
 )
@@ -17,17 +17,18 @@
     list_supported_datasets,
     load_specific_dataset,
 )
 from .saving import save_dict_into_h5
 from .utils import parse_delta, sliding_window
 
 __all__ = [
-    # datasets
+    # base dataset classes
     "BaseDataset",
-    # data generation
+    "SUPPORTED_DATASET_FILE_FORMATS",
+    # dataset generation functions
     "gene_complete_random_walk",
     "gene_complete_random_walk_for_anomaly_detection",
     "gene_complete_random_walk_for_classification",
     "gene_random_walk",
     "gene_physionet2012",
     # list and load datasets
     "list_supported_datasets",
```

### Comparing `pypots-0.4.1/pypots/data/base.py` & `pypots-0.5/pypots/data/dataset/base.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,240 +1,369 @@
 """
-The base class for PyPOTS datasets.
+The base dataset class.
 """
 
 # Created by Wenjie Du <wenjay.du@gmail.com>
 # License: BSD-3-Clause
 
-from abc import abstractmethod
 from typing import Union, Optional, Tuple, Iterable
 
 import h5py
 import numpy as np
 import torch
+from numpy import ndarray
 from pygrinder import fill_and_get_mask_torch
+from torch import Tensor
 from torch.utils.data import Dataset
 
-from .utils import turn_data_into_specified_dtype
-
-# Currently we only support h5 files
-SUPPORTED_DATASET_FILE_TYPE = ["h5py"]
+from .config import SUPPORTED_DATASET_FILE_FORMATS
+from ..utils import turn_data_into_specified_dtype
 
 
 class BaseDataset(Dataset):
-    """Base dataset class in PyPOTS.
+    """Base dataset class for models in PyPOTS.
 
     Parameters
     ----------
     data :
-        The dataset for model input, should be a dictionary including keys as 'X' and 'y',
-        or a path string locating a data file.
-        If it is a dict, X should be array-like of shape [n_samples, sequence length (time steps), n_features],
-        which is time-series data for input, can contain missing values, and y should be array-like of shape
-        [n_samples], which is classification labels of X.
+        The dataset for model input, should be a dictionary or
+        a path string locating a data file that is in supported formats.
+        If it is a dict, 'X' is mandatory and 'X_ori', 'X_pred', and 'y' are optional.
+        ``X`` is time-series data for input and could contain missing values.
+        It should be array-like of shape [n_samples, n_steps (sequence length), n_features].
+        ``X_ori`` is optional. If ``X`` is constructed from ``X_ori`` with specially designed artificial missingness,
+        your model may need ``X_ori`` for evaluation or loss calculation during training (e.g. SAITS).
+        It should have the same shape as ``X``.
+        ``X_pred`` is optional, and it is the forecasting results for the model to predict in forecasting tasks.
+        ``X_pred`` should be array-like of shape [n_samples, n_steps (sequence length), n_features], and its shape
+        could different from ``X``. But remember that ``X_pred`` contains time series forecasting results of ``X``,
+        hence it has the same number of samples as ``X``, i.e. n_samples of them are the same, but their n_steps
+        and n_features could be different. ``X_pred`` could have missing values as well as ``X``.
+        ``y`` should be array-like of shape [n_samples], which is classification labels of X.
         If it is a path string, the path should point to a data file, e.g. a h5 file, which contains
-        key-value pairs like a dict, and it has to include keys as 'X' and 'y'.
+        key-value pairs like a dict, and it has to include keys as 'X', etc.
 
-    return_labels :
-        Whether to return labels in function __getitem__() if they exist in the given data. If `True`, for example,
-        during training of classification models, the Dataset class will return labels in __getitem__() for model input.
-        Otherwise, labels won't be included in the data returned by __getitem__(). This parameter exists because we
-        need the defined Dataset class for all training/validating/testing stages. For those big datasets stored in h5
-        files, they already have both X and y saved. But we don't read labels from the file for validating and testing
-        with function _fetch_data_from_file(), which works for all three stages. Therefore, we need this parameter for
-        distinction.
+    return_X_ori :
+        Whether to return X_ori and indicating_mask in function __getitem__() if it is given. If `True`, for example,
+        during training of models that need the original X, the Dataset class will return X_ori in __getitem__() for
+        model input. Otherwise, X_ori and indicating mask won't be included in the data list returned by __getitem__().
+
+    return_X_pred :
+        Whether to return X_pred and X_pred_missing_mask in function __getitem__() if it is given.
+        If `True`, for example, during training of forecasting models, the Dataset class will return forecasting X
+        in __getitem__() for model input. Otherwise, X_pred and its missing mask X_pred_missing_mask won't be included
+        in the data list returned by __getitem__().
+
+    return_y :
+        Whether to return y (i.e. labels) in function __getitem__() if they exist in the given data. If `True`,
+        for example, during training of classification models, the Dataset class will return labels in __getitem__()
+        for model input. Otherwise, labels won't be included in the data returned by __getitem__().
+        This parameter exists because we need the defined Dataset class for all training/validating/testing stages.
+        For those big datasets stored in h5 files, they already have both X and y saved.
+        But we don't read labels from the file for validating and testing with function _fetch_data_from_file(),
+        which works for all three stages. Therefore, we need this parameter for distinction.
 
     file_type :
         The type of the given file if train_set and val_set are path strings.
 
     """
 
     def __init__(
         self,
         data: Union[dict, str],
         return_X_ori: bool,
-        return_labels: bool,
-        file_type: str = "h5py",
+        return_X_pred: bool,
+        return_y: bool,
+        file_type: str = "hdf5",
     ):
         super().__init__()
         # types and shapes had been checked after X and y input into the model
         # So they are safe to use here. No need to check again.
 
         self.data = data
         self.return_X_ori = return_X_ori
-        self.return_labels = return_labels
+        self.return_X_pred = return_X_pred
+        self.return_y = return_y
+        self.file_type = file_type
+
+        # initialize the following attributes
+        self.X = None
+        self.X_ori = None
+        self.missing_mask = None
+        self.indicating_mask = None
+        self.X_pred = None
+        self.X_pred_missing_mask = None
+        self.y = None
+        self.file_handle = None
+        self.fetch_data = None
+        self.n_samples: int = 0  # num of the samples in the dataset
+        self.n_steps: int = 0  # num of the time steps in each sample
+        self.n_features: int = 0  # num of the features in each sample
+        self.n_pred_steps: int = 0  # num of the time steps in each forecasting sample
+        self.n_pred_features: int = 0  # num of the features in each forecasting sample
 
+        # check the data type and set up the fetch_data function
         if isinstance(self.data, str):  # data from file
             # check if the given file type is supported
             assert (
-                file_type in SUPPORTED_DATASET_FILE_TYPE
-            ), f"file_type should be one of {SUPPORTED_DATASET_FILE_TYPE}, but got {file_type}"
+                file_type in SUPPORTED_DATASET_FILE_FORMATS
+            ), f"file_type should be one of {SUPPORTED_DATASET_FILE_FORMATS}, but got {file_type}"
             self.file_type = file_type
 
             # open the file handle
             self.file_handle = self._open_file_handle()
             # check if X exists in the file
             assert (
                 "X" in self.file_handle.keys()
             ), "The given dataset file doesn't contains X. Please double check."
+            # check whether X_ori, X_pred, and y exist in the file if they are required
+            if self.return_X_ori:
+                assert (
+                    "X_ori" in self.file_handle.keys()
+                ), "The given dataset file doesn't contains X_ori. Please double check."
+            if self.return_X_pred:
+                assert (
+                    "X_pred" in self.file_handle.keys()
+                ), "The given dataset file doesn't contains X_pred. Please double check."
+            if self.return_y:
+                assert (
+                    "y" in self.file_handle.keys()
+                ), "The given dataset file doesn't contains y. Please double check."
+
+            # set up the function fetch_data() to fetch data from file
+            self.fetch_data = self._fetch_data_from_file
 
         else:  # data from array
+            # check if X exists in the dictionary
+            assert (
+                "X" in self.data.keys()
+            ), "The given dataset dictionary doesn't contains X. Please double check."
+            # check whether X_ori, X_pred, and y exist in the file if they are required
+            if self.return_X_ori:
+                assert (
+                    "X_ori" in self.data.keys()
+                ), "The given dataset dictionary doesn't contains X_ori. Please double check."
+            if self.return_X_pred:
+                assert (
+                    "X_pred" in self.data.keys()
+                ), "The given dataset dictionary doesn't contains X_pred. Please double check."
+            if self.return_y:
+                assert (
+                    "y" in self.data.keys()
+                ), "The given dataset dictionary doesn't contains y. Please double check."
+
             X = data["X"]
             X_ori = None if "X_ori" not in data.keys() else data["X_ori"]
+            X_pred = None if "X_pred" not in data.keys() else data["X_pred"]
             y = None if "y" not in data.keys() else data["y"]
-            self.X, self.X_ori, self.y = self._check_array_input(X, X_ori, y)
+            self.X, self.X_ori, self.X_pred, self.y = self._check_array_input(
+                X, X_ori, X_pred, y, "tensor"
+            )
 
-            if self.X_ori is not None and self.return_X_ori:
+            if self.return_X_ori:
                 # Only when X_ori is given and fixed, we fill the missing values in X here in advance.
                 # Otherwise, we may need original X with missing values to generate X_ori, e.g. in DatasetForSAITS.
                 self.X, self.missing_mask = fill_and_get_mask_torch(self.X)
 
                 self.X_ori, X_ori_missing_mask = fill_and_get_mask_torch(self.X_ori)
                 indicating_mask = X_ori_missing_mask - self.missing_mask
                 self.indicating_mask = indicating_mask.to(torch.float32)
-            else:
-                self.missing_mask = None
-                self.indicating_mask = None
-                # if return_X_ori is false, set X_ori to None as well
-                self.X_ori = None
 
-        self.n_samples, self.n_steps, self.n_features = self._get_data_sizes()
+            if self.return_X_pred:
+                self.X_pred, self.X_pred_missing_mask = fill_and_get_mask_torch(
+                    self.X_pred
+                )
 
-        # set up function fetch_data()
-        if isinstance(self.data, str):
-            self.fetch_data = self._fetch_data_from_file
-        else:
+            # set up the function fetch_data() to fetch data from array
             self.fetch_data = self._fetch_data_from_array
 
-    def _get_data_sizes(self) -> Tuple[int, int, int]:
-        """Determine the number of samples in the dataset and return the number.
+        # get the sizes of the dataset
+        (
+            self.n_samples,
+            self.n_steps,
+            self.n_features,
+            self.n_pred_steps,
+            self.n_pred_features,
+        ) = self._get_data_sizes()
+
+    def _get_data_sizes(self) -> Tuple[int, ...]:
+        """Detect the data sample sizes in the dataset and return the numbers.
 
         Returns
         -------
         n_samples :
             The number of the samples in the given dataset.
+
+        n_steps :
+            The number of each sample's time steps in the given dataset.
+
+        n_features :
+            The number of each sample's features in the given dataset.
+
+        n_pred_steps :
+            The number of each sample's forecasting time steps in the given dataset.
+            Return as 0 if the dataset does not contain X_pred which includes data samples for forecasting tasks.
+
+        n_pred_features :
+            The number of each sample's forecasting features in the given dataset.
+            Return as 0 if the dataset does not contain X_pred which includes data samples for forecasting tasks.
         """
 
+        # initialize the sizes
+        n_samples, n_steps, n_features, n_pred_steps, n_pred_features = 0, 0, 0, 0, 0
+
         if isinstance(self.data, str):
             if self.file_handle is None:
                 self.file_handle = self._open_file_handle()
             n_samples = len(self.file_handle["X"])
             first_sample = self.file_handle["X"][0]
             n_steps = len(first_sample)
             n_features = first_sample.shape[-1]
+
+            if self.return_X_pred:
+                first_pred_sample = self.file_handle["X_pred"][0]
+                n_pred_steps = len(first_pred_sample)
+                n_pred_features = first_pred_sample.shape[-1]
         else:
             n_samples = len(self.X)
             n_steps = len(self.X[0])
             n_features = self.X[0].shape[-1]
 
-        return n_samples, n_steps, n_features
+            if self.return_X_pred:
+                n_pred_steps = len(self.X_pred[0])
+                n_pred_features = self.X_pred[0].shape[-1]
+
+        return n_samples, n_steps, n_features, n_pred_steps, n_pred_features
 
     def __len__(self) -> int:
         return self.n_samples
 
     @staticmethod
     def _check_array_input(
-        X: Union[np.ndarray, torch.Tensor, list],
-        X_ori: Union[np.ndarray, torch.Tensor, list],
-        y: Optional[Union[np.ndarray, torch.Tensor, list]] = None,
+        X: Union[np.ndarray, torch.Tensor],
+        X_ori: Optional[Union[np.ndarray, torch.Tensor]] = None,
+        X_pred: Optional[Union[np.ndarray, torch.Tensor]] = None,
+        y: Optional[Union[np.ndarray, torch.Tensor]] = None,
         out_dtype: str = "tensor",
     ) -> Tuple[
-        Union[np.ndarray, torch.Tensor],
-        Union[np.ndarray, torch.Tensor],
-        Optional[Union[np.ndarray, torch.Tensor, list]],
+        Union[Tensor, ndarray],
+        Optional[Union[Tensor, ndarray]],
+        Optional[Union[Tensor, ndarray]],
+        Optional[Union[Tensor, ndarray]],
     ]:
         """Check value type and shape of input X and y
 
         Parameters
         ----------
         X :
-            Time-series data that must have a shape like [n_samples, expected_n_steps, expected_n_features].
+            The data samples for testing, should be array-like of shape [n_samples, sequence length (n_steps),
+            n_features], or a path string locating a data file, e.g. h5 file.
 
         X_ori :
             If X is with artificial missingness, X_ori is the original X without artificial missing values.
             It must have the same shape as X. If X_ori is with original missing values, should be left as NaN.
 
+        X_pred :
+            The forecasting results of X , should be array-like of shape [n_samples, sequence length (n_steps),
+            n_features], or a path string locating a data file, e.g. h5 file.
+
         y :
             Labels of time-series samples (X) that must have a shape like [n_samples] or [n_samples, n_classes].
 
         out_dtype :
             Data type of the output, should be np.ndarray or torch.Tensor
 
         Returns
         -------
         X :
 
         X_ori :
 
+        X_pred :
+
         y :
 
         """
         assert out_dtype in [
             "tensor",
             "ndarray",
         ], f'out_dtype should be "tensor" or "ndarray", but got {out_dtype}'
 
         # change the data type of X
         X = turn_data_into_specified_dtype(X, out_dtype)
-        X = X.to(torch.float32)
+        X = X.to(torch.float32) if out_dtype == "tensor" else X
 
         # check the shape of X here
         X_shape = X.shape
         assert len(X_shape) == 3, (
             f"input should have 3 dimensions [n_samples, seq_len, n_features],"
             f"but got X: {X_shape}"
         )
         if X_ori is not None:
             X_ori = turn_data_into_specified_dtype(X_ori, out_dtype)
-            X_ori = X_ori.to(torch.float32)
+            X_ori = X_ori.to(torch.float32) if out_dtype == "tensor" else X_ori
             assert (
                 X_shape == X_ori.shape
             ), f"X and X_ori must have matched shape, but got X: f{X.shape} and X_ori: {X_ori.shape}"
+
+        if X_pred is not None:
+            X_pred = turn_data_into_specified_dtype(X_pred, out_dtype)
+            X_pred = X_pred.to(torch.float32) if out_dtype == "tensor" else X_pred
+            assert len(X) == len(
+                X_pred
+            ), f"X and X_pred must have the same number of samples, but got X: f{X.shape} and X_pred: {X_pred.shape}"
+
         if y is not None:
             assert len(X) == len(y), (
                 f"lengths of X and y must match, " f"but got f{len(X)} and {len(y)}"
             )
             y = turn_data_into_specified_dtype(y, out_dtype)
+            y = y.to(torch.long) if out_dtype == "tensor" else y
 
-        return X, X_ori, y
+        return X, X_ori, X_pred, y
 
-    @abstractmethod
     def _fetch_data_from_array(self, idx: int) -> Iterable:
         """Fetch data from self.X if it is given.
 
         Parameters
         ----------
         idx :
             The index of the sample to be return.
 
         Returns
         -------
         sample :
             The collated data sample, a list including all necessary sample info.
         """
 
-        if self.X_ori is None:
-            X = self.X[idx]
-            X, missing_mask = fill_and_get_mask_torch(X)
-        else:
-            X = self.X[idx]
+        X = self.X[idx]
+
+        if self.return_X_ori:
+            # if X_ori is given, fetch missing mask from self.missing_mask that has been created in __init__()
             missing_mask = self.missing_mask[idx]
+        else:
+            X, missing_mask = fill_and_get_mask_torch(X)
 
         sample = [
             torch.tensor(idx),
             X,
             missing_mask,
         ]
 
-        if self.X_ori is not None and self.return_X_ori:
+        if self.return_X_ori:
             X_ori = self.X_ori[idx]
             indicating_mask = self.indicating_mask[idx]
             sample.extend([X_ori, indicating_mask])
 
-        if self.y is not None and self.return_labels:
+        if self.return_X_pred:
+            X_pred = self.X_pred[idx]
+            pred_missing_mask = self.X_pred[idx]
+            sample.extend([X_pred, pred_missing_mask])
+
+        if self.return_y:
             sample.append(self.y[idx].to(torch.long))
 
         return sample
 
     def _open_file_handle(self) -> h5py.File:
         """Open the file handle for reading data from the file.
 
@@ -265,15 +394,14 @@
                 f"Check out the above error log. This probably is caused by file type error. "
                 f"Please confirm that the given file {data_file_path} is an h5 file."
             )
         except Exception as e:
             raise RuntimeError(e)
         return file_handler
 
-    @abstractmethod
     def _fetch_data_from_file(self, idx: int) -> Iterable:
         """Fetch data with the lazy-loading strategy, i.e. only loading data from the file while requesting for samples.
         Here the opened file handle doesn't load the entire dataset into RAM but only load the currently accessed slice.
 
         Notes
         -----
         Multi workers reading from h5 file is tricky, and I was confronted with a problem similar to
@@ -303,22 +431,27 @@
         X, missing_mask = fill_and_get_mask_torch(X)
         sample = [
             torch.tensor(idx),
             X,
             missing_mask,
         ]
 
-        if "X_ori" in self.file_handle.keys() and self.return_X_ori:
+        if self.return_X_ori:
             X_ori = torch.from_numpy(self.file_handle["X_ori"][idx]).to(torch.float32)
             X_ori, X_ori_missing_mask = fill_and_get_mask_torch(X_ori)
             indicating_mask = (X_ori_missing_mask - missing_mask).to(torch.float32)
             sample.extend([X_ori, indicating_mask])
 
+        if self.return_X_pred:
+            X_pred = torch.from_numpy(self.file_handle["X_pred"][idx]).to(torch.float32)
+            X_pred, X_pred_missing_mask = fill_and_get_mask_torch(X_pred)
+            sample.extend([X_pred, X_pred_missing_mask])
+
         # if the dataset has labels and is for training, then fetch it from the file
-        if "y" in self.file_handle.keys() and self.return_labels:
+        if self.return_y:
             sample.append(self.file_handle["y"][idx].to(torch.long))
 
         return sample
 
     def __getitem__(self, idx: int) -> Iterable:
         """Fetch data according to index.
```

### Comparing `pypots-0.4.1/pypots/data/generating.py` & `pypots-0.5/pypots/data/generating.py`

 * *Files 2% similar despite different names*

```diff
@@ -268,16 +268,16 @@
     )
     # split into train/val/test sets
     train_X, test_X, train_y, test_y = train_test_split(X, y, test_size=0.2)
     train_X, val_X, train_y, val_y = train_test_split(train_X, train_y, test_size=0.2)
 
     if missing_rate > 0:
         # create random missing values
+        train_X_ori = train_X
         train_X = mcar(train_X, missing_rate)
-        val_X = mcar(val_X, missing_rate)
         # test set is left to mask after normalization
 
     train_X = train_X.reshape(-1, n_features)
     val_X = val_X.reshape(-1, n_features)
     test_X = test_X.reshape(-1, n_features)
     # normalization
     scaler = StandardScaler()
@@ -298,30 +298,30 @@
         "val_y": val_y,
         "test_X": test_X,
         "test_y": test_y,
         "scaler": scaler,
     }
 
     if missing_rate > 0:
-        # mask values in the validation set as ground truth
-        val_X_ori = val_X
-        val_X = mcar(val_X, missing_rate)
-
         # mask values in the test set as ground truth
-        test_X_ori = test_X
-        test_X = mcar(test_X, 0.3)
+        train_X_ori = scaler.transform(train_X_ori.reshape(-1, n_features)).reshape(
+            -1, n_steps, n_features
+        )
+        data["train_X_ori"] = train_X_ori
 
+        val_X_ori = val_X
+        val_X = mcar(val_X, missing_rate)
         data["val_X"] = val_X
         data["val_X_ori"] = val_X_ori
 
-        # test_X is for model input
+        test_X_ori = test_X
+        test_X = mcar(test_X, missing_rate)
         data["test_X"] = test_X
-        # test_X_ori is for error calc, not for model input, hence mustn't have NaNs
-        data["test_X_ori"] = np.nan_to_num(test_X_ori)
-        data["test_X_indicating_mask"] = ~np.isnan(test_X_ori) ^ ~np.isnan(test_X)
+        data["test_X_ori"] = np.nan_to_num(test_X_ori)  # fill NaNs for later error calc
+        data["test_X_indicating_mask"] = np.isnan(test_X_ori) ^ np.isnan(test_X)
 
     return data
 
 
 def gene_physionet2012(artificially_missing_rate: float = 0.1):
     """Generate a fully-prepared PhysioNet-2012 dataset for model testing.
 
@@ -418,11 +418,11 @@
 
         data["val_X"] = val_X
         data["val_X_ori"] = val_X_ori
 
         # test_X is for model input
         data["test_X"] = test_X
         # test_X_ori is for error calc, not for model input, hence mustn't have NaNs
-        data["test_X_ori"] = np.nan_to_num(test_X_ori)
-        data["test_X_indicating_mask"] = ~np.isnan(test_X_ori) ^ ~np.isnan(test_X)
+        data["test_X_ori"] = np.nan_to_num(test_X_ori)  # fill NaNs for later error calc
+        data["test_X_indicating_mask"] = np.isnan(test_X_ori) ^ np.isnan(test_X)
 
     return data
```

### Comparing `pypots-0.4.1/pypots/data/load_preprocessing.py` & `pypots-0.5/pypots/data/load_preprocessing.py`

 * *Files identical despite different names*

### Comparing `pypots-0.4.1/pypots/data/load_specific_datasets.py` & `pypots-0.5/pypots/data/load_specific_datasets.py`

 * *Files identical despite different names*

### Comparing `pypots-0.4.1/pypots/data/saving/h5.py` & `pypots-0.5/pypots/data/saving/h5.py`

 * *Files identical despite different names*

### Comparing `pypots-0.4.1/pypots/data/saving/pickle.py` & `pypots-0.5/pypots/data/saving/pickle.py`

 * *Files identical despite different names*

### Comparing `pypots-0.4.1/pypots/data/utils.py` & `pypots-0.5/pypots/data/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -132,16 +132,17 @@
     missing_mask: Union[np.ndarray, torch.Tensor]
 ) -> Union[np.ndarray, torch.Tensor]:
     """Generate the time-gap matrix (i.e. the delta metrix) from the missing mask.
     Please refer to :cite:`che2018GRUD` for its math definition.
 
     Parameters
     ----------
-    missing_mask : shape of [n_steps, n_features] or [n_samples, n_steps, n_features]
+    missing_mask :
         Binary masks indicate missing data (0 means missing values, 1 means observed values).
+        Shape of [n_steps, n_features] or [n_samples, n_steps, n_features].
 
     Returns
     -------
     delta :
         The delta matrix indicates the time gaps between observed values.
         With the same shape of missing_mask.
```

### Comparing `pypots-0.4.1/pypots/forecasting/base.py` & `pypots-0.5/pypots/forecasting/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -63,73 +63,73 @@
         )
 
     @abstractmethod
     def fit(
         self,
         train_set: Union[dict, str],
         val_set: Optional[Union[dict, str]] = None,
-        file_type: str = "h5py",
+        file_type: str = "hdf5",
     ) -> None:
         """Train the classifier on the given data.
 
         Parameters
         ----------
         train_set :
             The dataset for model training, should be a dictionary including the key 'X',
             or a path string locating a data file.
-            If it is a dict, X should be array-like of shape [n_samples, sequence length (time steps), n_features],
+            If it is a dict, X should be array-like of shape [n_samples, sequence length (n_steps), n_features],
             which is time-series data for training, can contain missing values.
             If it is a path string, the path should point to a data file, e.g. a h5 file, which contains
             key-value pairs like a dict, and it has to include the key 'X'.
 
         val_set :
             The dataset for model validating, should be a dictionary including the key 'X',
             or a path string locating a data file.
-            If it is a dict, X should be array-like of shape [n_samples, sequence length (time steps), n_features],
+            If it is a dict, X should be array-like of shape [n_samples, sequence length (n_steps), n_features],
             which is time-series data for validation, can contain missing values.
             If it is a path string, the path should point to a data file, e.g. a h5 file, which contains
             key-value pairs like a dict, and it has to include the key 'X'.
 
         file_type :
             The type of the given file if train_set and val_set are path strings.
 
         """
         raise NotImplementedError
 
     @abstractmethod
     def predict(
         self,
         test_set: Union[dict, str],
-        file_type: str = "h5py",
+        file_type: str = "hdf5",
     ) -> dict:
         raise NotImplementedError
 
     @abstractmethod
     def forecast(
         self,
-        X: dict or str,
-        file_type: str = "h5py",
+        test_set: Union[dict, str],
+        file_type: str = "hdf5",
     ) -> np.ndarray:
         """Forecast the future the input with the trained model.
 
         Parameters
         ----------
-        X :
-            Time-series data containing missing values. Shape [n_samples, sequence length (time steps), n_features].
+        test_set :
+            The data samples for testing, should be array-like of shape [n_samples, sequence length (n_steps),
+            n_features], or a path string locating a data file, e.g. h5 file.
 
         file_type :
             The type of the given file if X is a path string.
 
         Returns
         -------
-        array-like, shape [n_samples, prediction_horizon, n_features],
+        array-like, shape [n_samples, n_pred_steps, n_features],
             Forecasting results.
         """
-        # this is for old API compatibility, will be removed in the future.
-        # Please implement predict() instead.
+
         raise NotImplementedError
 
 
 class BaseNNForecaster(BaseNNModel):
     """The abstract class for all neural-network forecasting models in PyPOTS.
 
     Parameters
@@ -196,15 +196,15 @@
             num_workers,
             device,
             saving_path,
             model_saving_strategy,
         )
 
     @abstractmethod
-    def _assemble_input_for_training(self, data) -> dict:
+    def _assemble_input_for_training(self, data: list) -> dict:
         """Assemble the given data into a dictionary for training input.
 
         Parameters
         ----------
         data :
             Input data from dataloader, should be list.
 
@@ -212,15 +212,15 @@
         -------
         dict,
             A python dictionary contains the input data for model training.
         """
         raise NotImplementedError
 
     @abstractmethod
-    def _assemble_input_for_validating(self, data) -> dict:
+    def _assemble_input_for_validating(self, data: list) -> dict:
         """Assemble the given data into a dictionary for validating input.
 
         Parameters
         ----------
         data :
             Data output from dataloader, should be list.
 
@@ -228,15 +228,15 @@
         -------
         dict,
             A python dictionary contains the input data for model validating.
         """
         raise NotImplementedError
 
     @abstractmethod
-    def _assemble_input_for_testing(self, data) -> dict:
+    def _assemble_input_for_testing(self, data: list) -> dict:
         """Assemble the given data into a dictionary for testing input.
 
         Notes
         -----
         The processing functions of train/val/test stages are separated for the situation that the input of
         the three stages are different, and this situation usually happens when the Dataset/Dataloader classes
         used in the train/val/test stages are not the same, e.g. the training data and validating data in a
@@ -376,71 +376,66 @@
         )
 
     @abstractmethod
     def fit(
         self,
         train_set: Union[dict, str],
         val_set: Optional[Union[dict, str]] = None,
-        file_type: str = "h5py",
+        file_type: str = "hdf5",
     ) -> None:
         """Train the classifier on the given data.
 
         Parameters
         ----------
         train_set :
             The dataset for model training, should be a dictionary including the key 'X',
             or a path string locating a data file.
-            If it is a dict, X should be array-like of shape [n_samples, sequence length (time steps), n_features],
+            If it is a dict, X should be array-like of shape [n_samples, sequence length (n_steps), n_features],
             which is time-series data for training, can contain missing values.
             If it is a path string, the path should point to a data file, e.g. a h5 file, which contains
             key-value pairs like a dict, and it has to include the key 'X'.
 
         val_set :
             The dataset for model validating, should be a dictionary including the key 'X',
             or a path string locating a data file.
-            If it is a dict, X should be array-like of shape [n_samples, sequence length (time steps), n_features],
+            If it is a dict, X should be array-like of shape [n_samples, sequence length (n_steps), n_features],
             which is time-series data for validation, can contain missing values.
             If it is a path string, the path should point to a data file, e.g. a h5 file, which contains
             key-value pairs like a dict, and it has to include the key 'X'.
 
         file_type :
             The type of the given file if train_set and val_set are path strings.
 
         """
         raise NotImplementedError
 
     @abstractmethod
     def predict(
         self,
         test_set: Union[dict, str],
-        file_type: str = "h5py",
+        file_type: str = "hdf5",
     ) -> dict:
         raise NotImplementedError
 
     @abstractmethod
     def forecast(
         self,
-        X: dict or str,
-        file_type: str = "h5py",
+        test_set: Union[dict, str],
+        file_type: str = "hdf5",
     ) -> np.ndarray:
         """Forecast the future the input with the trained model.
 
-        Warnings
-        --------
-        The method forecast is deprecated. Please use `predict()` instead.
-
         Parameters
         ----------
-        X :
-            Time-series data containing missing values. Shape [n_samples, sequence length (time steps), n_features].
+        test_set :
+            The data samples for testing, should be array-like of shape [n_samples, sequence length (n_steps),
+            n_features], or a path string locating a data file, e.g. h5 file.
 
         file_type :
             The type of the given file if X is a path string.
 
         Returns
         -------
-        array-like, shape [n_samples, prediction_horizon, n_features],
+        array-like, shape [n_samples, n_pred_steps, n_features],
             Forecasting results.
         """
-        # this is for old API compatibility, will be removed in the future.
-        # Please implement predict() instead.
         raise NotImplementedError
```

### Comparing `pypots-0.4.1/pypots/forecasting/bttf/core.py` & `pypots-0.5/pypots/forecasting/bttf/core.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,9 @@
 """
-The implementation of BTTF (Bayesian Temporal Tensor Factorization) for the partially-observed time-series
-forecasting task.
-
-Refer to the paper "Chen, X., & Sun, L. (2021).
-Bayesian Temporal Factorization for Multidimensional Time Series Prediction.
-IEEE transactions on pattern analysis and machine intelligence."
-
-Notes
------
-This numpy implementation is the same with the official one from https://github.com/xinychen/transdim.
-
+The core wrapper assembles the submodules of BTTF forecasting model.
 """
 
 # Created by Wenjie Du <wenjay.du@gmail.com>
 # License: BSD-3-Clause
 
 import numpy as np
 from numpy.linalg import inv as inv
```

### Comparing `pypots-0.4.1/pypots/forecasting/bttf/model.py` & `pypots-0.5/pypots/forecasting/bttf/model.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,33 +1,24 @@
 """
 The implementation of BTTF (Bayesian Temporal Tensor Factorization) for the partially-observed time-series
 forecasting task.
 
-Refer to the paper "Xinyu Chen and Lijun Sun.
-Bayesian Temporal Factorization for Multidimensional Time Series Prediction.
-IEEE Transactions on Pattern Analysis and Machine Intelligence, pages 1–1, 2021."
-
-Notes
------
-This numpy implementation is the same with the official one from https://github.com/xinychen/transdim.
-
 """
 
 # Created by Wenjie Du <wenjay.du@gmail.com>
 # License: BSD-3-Clause
 
 import warnings
 from typing import Union, Optional
 
 import numpy as np
 import torch
 
 from .core import BTTF_forecast
 from ..base import BaseForecaster
-from ...utils.logging import logger
 
 
 class BTTF(BaseForecaster):
     """The implementation of the BTTF model :cite:`chen2021BTMF`.
 
     Parameters
     ----------
@@ -93,30 +84,30 @@
         self.burn_iter = burn_iter
         self.gibbs_iter = gibbs_iter
 
     def fit(
         self,
         train_set: Union[dict, str],
         val_set: Optional[Union[dict, str]] = None,
-        file_type="h5py",
+        file_type: str = "hdf5",
     ) -> None:
         """Train the forecaster on the given data.
 
         Warnings
         --------
         BTTF does not need to run fit().
         Please run func ``forecast()`` directly.
 
         """
         warnings.warn("Please run func forecast(X) directly.")
 
     def predict(
         self,
         test_set: Union[dict, str],
-        file_type: str = "h5py",
+        file_type: str = "hdf5",
     ) -> dict:
         assert not isinstance(
             test_set, str
         ), "BTTF so far does not accept file input. It needs a specified Dataset class."
 
         X = test_set["X"]
         X = X.transpose((0, 2, 1))
@@ -135,35 +126,29 @@
         result_dict = {
             "forecasting": forecasting,
         }
         return result_dict
 
     def forecast(
         self,
-        X: Union[dict, str],
-        file_type: str = "h5py",
+        test_set: Union[dict, str],
+        file_type: str = "hdf5",
     ) -> np.ndarray:
-        """Forecast the future the input with the trained model.
-
-        Warnings
-        --------
-        The method forecast is deprecated. Please use `predict()` instead.
+        """Forecast the future of the input with the trained model.
 
         Parameters
         ----------
-        X :
-            Time-series data containing missing values. Shape [n_samples, sequence length (time steps), n_features].
+        test_set :
+            The data samples for testing, should be array-like of shape [n_samples, sequence length (n_steps),
+            n_features], or a path string locating a data file, e.g. h5 file.
 
         file_type :
             The type of the given file if X is a path string.
 
         Returns
         -------
-        array-like, shape [n_samples, prediction_horizon, n_features],
+        array-like, shape [n_samples, n_pred_steps, n_features],
             Forecasting results.
         """
-        logger.warning(
-            "🚨DeprecationWarning: The method forecast is deprecated. Please use `predict` instead."
-        )
-        result_dict = self.predict(X, file_type=file_type)
-        forecasting = result_dict["forecasting"]
-        return forecasting
+
+        result_dict = self.predict(test_set, file_type=file_type)
+        return result_dict["forecasting"]
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pypots-0.4.1/pypots/forecasting/bttf/submodules.py` & `pypots-0.5/pypots/forecasting/bttf/submodules.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,8 @@
 """
-The implementation of the modules for BTTF (Bayesian Temporal Tensor Factorization).
-
-Refer to the paper "Chen, X., & Sun, L. (2021).
-Bayesian Temporal Factorization for Multidimensional Time Series Prediction.
-IEEE transactions on pattern analysis and machine intelligence."
-
-Notes
------
-This numpy implementation is the same with the official one from https://github.com/xinychen/transdim.
 
 """
 
 # Created by Wenjie Du <wenjay.du@gmail.com>
 # License: BSD-3-Clause
 
 import numpy as np
```

### Comparing `pypots-0.4.1/pypots/imputation/__init__.py` & `pypots-0.5/pypots/imputation/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,17 +8,20 @@
 # neural network imputation methods
 from .brits import BRITS
 from .csdi import CSDI
 from .gpvae import GPVAE
 from .mrnn import MRNN
 from .saits import SAITS
 from .transformer import Transformer
+from .itransformer import iTransformer
 from .timesnet import TimesNet
 from .etsformer import ETSformer
 from .fedformer import FEDformer
+from .film import FiLM
+from .frets import FreTS
 from .crossformer import Crossformer
 from .informer import Informer
 from .autoformer import Autoformer
 from .dlinear import DLinear
 from .patchtst import PatchTST
 from .usgan import USGAN
 
@@ -27,16 +30,19 @@
 from .mean import Mean
 from .median import Median
 
 __all__ = [
     # neural network imputation methods
     "SAITS",
     "Transformer",
+    "iTransformer",
     "ETSformer",
     "FEDformer",
+    "FiLM",
+    "FreTS",
     "Crossformer",
     "TimesNet",
     "PatchTST",
     "DLinear",
     "Informer",
     "Autoformer",
     "BRITS",
```

### Comparing `pypots-0.4.1/pypots/imputation/autoformer/__init__.py` & `pypots-0.5/pypots/imputation/autoformer/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -3,14 +3,18 @@
 
 Refer to the paper
 `Haixu Wu, Jiehui Xu, Jianmin Wang, and Mingsheng Long.
 Autoformer: Decomposition transformers with autocorrelation for long-term series forecasting.
 In Advances in Neural Information Processing Systems, volume 34, pages 22419–22430. Curran Associates, Inc., 2021.
 <https://proceedings.neurips.cc/paper/2021/file/bcc0d400288793e8bdcd7c19a8ac0c2b-Paper.pdf>`_
 
+Notes
+-----
+This implementation is inspired by the official one https://github.com/thuml/Autoformer
+
 """
 
 # Created by Wenjie Du <wenjay.du@gmail.com>
 # License: BSD-3-Clause
 
 
 from .model import Autoformer
```

### Comparing `pypots-0.4.1/pypots/imputation/autoformer/core.py` & `pypots-0.5/pypots/imputation/etsformer/core.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,94 +1,100 @@
 """
-
+The core wrapper assembles the submodules of ETSformer imputation model
+and takes over the forward progress of the algorithm.
 """
 
 # Created by Wenjie Du <wenjay.du@gmail.com>
 # License: BSD-3-Clause
 
-import torch
 import torch.nn as nn
 
-from ...nn.modules.autoformer import (
-    SeasonalLayerNorm,
-    AutoformerEncoderLayer,
-    AutoCorrelation,
-    AutoCorrelationLayer,
+from ...nn.modules.etsformer import (
+    ETSformerEncoderLayer,
+    ETSformerEncoder,
+    ETSformerDecoderLayer,
+    ETSformerDecoder,
 )
-from ...nn.modules.informer import InformerEncoder
-from ...nn.modules.saits import SaitsLoss
-from ...nn.modules.transformer.embedding import DataEmbedding
+from ...nn.modules.saits import SaitsLoss, SaitsEmbedding
 
 
-class _Autoformer(nn.Module):
+class _ETSformer(nn.Module):
     def __init__(
         self,
         n_steps,
         n_features,
-        n_layers,
-        n_heads,
+        n_e_layers,
+        n_d_layers,
         d_model,
+        n_heads,
         d_ffn,
-        factor,
-        moving_avg_window_size,
         dropout,
+        top_k,
         ORT_weight: float = 1,
         MIT_weight: float = 1,
-        activation="relu",
+        activation="sigmoid",
     ):
         super().__init__()
 
-        self.n_steps = n_steps
-
-        self.enc_embedding = DataEmbedding(
+        self.saits_embedding = SaitsEmbedding(
             n_features * 2,
             d_model,
+            with_pos=True,
+            n_max_steps=n_steps,
             dropout=dropout,
-            with_pos=False,
         )
-        self.encoder = InformerEncoder(
+
+        # Encoder
+        self.encoder = ETSformerEncoder(
+            [
+                ETSformerEncoderLayer(
+                    d_model,
+                    n_heads,
+                    n_features,
+                    n_steps,
+                    n_steps,
+                    top_k,
+                    d_ffn=d_ffn,
+                    dropout=dropout,
+                    activation=activation,
+                )
+                for _ in range(n_e_layers)
+            ]
+        )
+        # Decoder
+        self.decoder = ETSformerDecoder(
             [
-                AutoformerEncoderLayer(
-                    AutoCorrelationLayer(
-                        AutoCorrelation(factor, dropout),
-                        d_model,
-                        n_heads,
-                    ),
+                ETSformerDecoderLayer(
                     d_model,
-                    d_ffn,
-                    moving_avg_window_size,
-                    dropout,
-                    activation,
+                    n_heads,
+                    n_features,
+                    n_steps,
+                    dropout=dropout,
                 )
-                for _ in range(n_layers)
+                for _ in range(n_d_layers)
             ],
-            norm_layer=SeasonalLayerNorm(d_model),
         )
 
-        # for the imputation task, the output dim is the same as input dim
-        self.output_projection = nn.Linear(d_model, n_features)
+        # apply SAITS loss function to ETSformer on the imputation task
         self.saits_loss_func = SaitsLoss(ORT_weight, MIT_weight)
 
     def forward(self, inputs: dict, training: bool = True) -> dict:
         X, missing_mask = inputs["X"], inputs["missing_mask"]
 
-        # WDU: the original Autoformer paper isn't proposed for imputation task. Hence the model doesn't take
+        # WDU: the original ETSformer paper isn't proposed for imputation task. Hence the model doesn't take
         # the missing mask into account, which means, in the process, the model doesn't know which part of
-        # the input data is missing, and this may hurt the model's imputation performance. Therefore, I add the
-        # embedding layers to project the concatenation of features and masks into a hidden space, as well as
+        # the input data is missing, and this may hurt the model's imputation performance. Therefore, I apply the
+        # SAITS embedding method to project the concatenation of features and masks into a hidden space, as well as
         # the output layers to project back from the hidden space to the original space.
+        res = self.saits_embedding(X, missing_mask)
 
-        # the same as SAITS, concatenate the time series data and the missing mask for embedding
-        input_X = torch.cat([X, missing_mask], dim=2)
-        enc_out = self.enc_embedding(input_X)
-
-        # Autoformer encoder processing
-        enc_out, attns = self.encoder(enc_out)
-        # project back the original data space
-        reconstruction = self.output_projection(enc_out)
+        # ETSformer encoder processing
+        level, growths, seasons = self.encoder(res, X, attn_mask=None)
+        growth, season = self.decoder(growths, seasons)
+        reconstruction = level[:, -1:] + growth + season
 
         imputed_data = missing_mask * X + (1 - missing_mask) * reconstruction
         results = {
             "imputed_data": imputed_data,
         }
 
         # if in training mode, return results with losses
```

### Comparing `pypots-0.4.1/pypots/imputation/autoformer/data.py` & `pypots-0.5/pypots/imputation/autoformer/data.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,12 +13,12 @@
 class DatasetForAutoformer(DatasetForSAITS):
     """Actually Autoformer uses the same data strategy as SAITS, needs MIT for training."""
 
     def __init__(
         self,
         data: Union[dict, str],
         return_X_ori: bool,
-        return_labels: bool,
-        file_type: str = "h5py",
+        return_y: bool,
+        file_type: str = "hdf5",
         rate: float = 0.2,
     ):
-        super().__init__(data, return_X_ori, return_labels, file_type, rate)
+        super().__init__(data, return_X_ori, return_y, file_type, rate)
```

### Comparing `pypots-0.4.1/pypots/imputation/autoformer/model.py` & `pypots-0.5/pypots/imputation/autoformer/model.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,37 +1,28 @@
 """
 The implementation of Autoformer for the partially-observed time-series imputation task.
 
-Refer to the paper "Haixu Wu, Jiehui Xu, Jianmin Wang, and Mingsheng Long.
-Autoformer: Decomposition transformers with autocorrelation for long-term series forecasting.
-In Advances in Neural Information Processing Systems, volume 34, pages 22419–22430. Curran Associates, Inc., 2021."
-
-Notes
------
-Partial implementation uses code from https://github.com/thuml/Autoformer
-
 """
 
 # Created by Wenjie Du <wenjay.du@gmail.com>
 # License: BSD-3-Clause
 
 from typing import Union, Optional
 
 import numpy as np
 import torch
 from torch.utils.data import DataLoader
 
+from .core import _Autoformer
 from .data import DatasetForAutoformer
-from pypots.imputation.autoformer.core import _Autoformer
 from ..base import BaseNNImputer
-from ...data.base import BaseDataset
-from ...data.checking import check_X_ori_in_val_set
+from ...data.checking import key_in_data_set
+from ...data.dataset import BaseDataset
 from ...optim.adam import Adam
 from ...optim.base import Optimizer
-from ...utils.logging import logger
 
 
 class Autoformer(BaseNNImputer):
     """The PyTorch implementation of the Autoformer model.
     Autoformer is originally proposed by Wu et al. in :cite:`wu2021autoformer`.
 
     Parameters
@@ -41,20 +32,20 @@
 
     n_features :
         The number of features in the time-series data sample.
 
     n_layers :
         The number of layers in the Autoformer model.
 
-    n_heads :
-        The number of heads in each layer of Autoformer.
-
     d_model :
         The dimension of the model.
 
+    n_heads :
+        The number of heads in each layer of Autoformer.
+
     d_ffn :
         The dimension of the feed-forward network.
 
     factor :
         The factor of the auto correlation mechanism for the Autoformer model.
 
     moving_avg_window_size :
@@ -111,16 +102,16 @@
     """
 
     def __init__(
         self,
         n_steps: int,
         n_features: int,
         n_layers: int,
-        n_heads: int,
         d_model: int,
+        n_heads: int,
         d_ffn: int,
         factor: int,
         moving_avg_window_size: int,
         dropout: float = 0,
         ORT_weight: float = 1,
         MIT_weight: float = 1,
         batch_size: int = 32,
@@ -156,16 +147,16 @@
         self.MIT_weight = MIT_weight
 
         # set up the model
         self.model = _Autoformer(
             self.n_steps,
             self.n_features,
             self.n_layers,
-            self.n_heads,
             self.d_model,
+            self.n_heads,
             self.d_ffn,
             self.factor,
             self.moving_avg_window_size,
             self.dropout,
             self.ORT_weight,
             self.MIT_weight,
         )
@@ -207,32 +198,32 @@
 
         return inputs
 
     def fit(
         self,
         train_set: Union[dict, str],
         val_set: Optional[Union[dict, str]] = None,
-        file_type: str = "h5py",
+        file_type: str = "hdf5",
     ) -> None:
         # Step 1: wrap the input data with classes Dataset and DataLoader
         training_set = DatasetForAutoformer(
-            train_set, return_X_ori=False, return_labels=False, file_type=file_type
+            train_set, return_X_ori=False, return_y=False, file_type=file_type
         )
         training_loader = DataLoader(
             training_set,
             batch_size=self.batch_size,
             shuffle=True,
             num_workers=self.num_workers,
         )
         val_loader = None
         if val_set is not None:
-            if not check_X_ori_in_val_set(val_set):
+            if not key_in_data_set("X_ori", val_set):
                 raise ValueError("val_set must contain 'X_ori' for model validation.")
             val_set = DatasetForAutoformer(
-                val_set, return_X_ori=True, return_labels=False, file_type=file_type
+                val_set, return_X_ori=True, return_y=False, file_type=file_type
             )
             val_loader = DataLoader(
                 val_set,
                 batch_size=self.batch_size,
                 shuffle=False,
                 num_workers=self.num_workers,
             )
@@ -244,42 +235,46 @@
 
         # Step 3: save the model if necessary
         self._auto_save_model_if_necessary(confirm_saving=True)
 
     def predict(
         self,
         test_set: Union[dict, str],
-        file_type: str = "h5py",
+        file_type: str = "hdf5",
     ) -> dict:
         """Make predictions for the input data with the trained model.
 
         Parameters
         ----------
         test_set : dict or str
             The dataset for model validating, should be a dictionary including keys as 'X',
             or a path string locating a data file supported by PyPOTS (e.g. h5 file).
-            If it is a dict, X should be array-like of shape [n_samples, sequence length (time steps), n_features],
+            If it is a dict, X should be array-like of shape [n_samples, sequence length (n_steps), n_features],
             which is time-series data for validating, can contain missing values, and y should be array-like of shape
             [n_samples], which is classification labels of X.
             If it is a path string, the path should point to a data file, e.g. a h5 file, which contains
             key-value pairs like a dict, and it has to include keys as 'X' and 'y'.
 
-        file_type : str
+        file_type :
             The type of the given file if test_set is a path string.
 
         Returns
         -------
-        result_dict : dict,
+        file_type :
             The dictionary containing the clustering results and latent variables if necessary.
 
         """
         # Step 1: wrap the input data with classes Dataset and DataLoader
         self.model.eval()  # set the model as eval status to freeze it.
         test_set = BaseDataset(
-            test_set, return_X_ori=False, return_labels=False, file_type=file_type
+            test_set,
+            return_X_ori=False,
+            return_X_pred=False,
+            return_y=False,
+            file_type=file_type,
         )
         test_loader = DataLoader(
             test_set,
             batch_size=self.batch_size,
             shuffle=False,
             num_workers=self.num_workers,
         )
@@ -297,36 +292,29 @@
         result_dict = {
             "imputation": imputation,
         }
         return result_dict
 
     def impute(
         self,
-        X: Union[dict, str],
-        file_type="h5py",
+        test_set: Union[dict, str],
+        file_type: str = "hdf5",
     ) -> np.ndarray:
         """Impute missing values in the given data with the trained model.
 
-        Warnings
-        --------
-        The method impute is deprecated. Please use `predict()` instead.
-
         Parameters
         ----------
-        X :
-            The data samples for testing, should be array-like of shape [n_samples, sequence length (time steps),
+        test_set :
+            The data samples for testing, should be array-like of shape [n_samples, sequence length (n_steps),
             n_features], or a path string locating a data file, e.g. h5 file.
 
         file_type :
             The type of the given file if X is a path string.
 
         Returns
         -------
-        array-like, shape [n_samples, sequence length (time steps), n_features],
+        array-like, shape [n_samples, sequence length (n_steps), n_features],
             Imputed data.
         """
-        logger.warning(
-            "🚨DeprecationWarning: The method impute is deprecated. Please use `predict` instead."
-        )
 
-        results_dict = self.predict(X, file_type=file_type)
-        return results_dict["imputation"]
+        result_dict = self.predict(test_set, file_type=file_type)
+        return result_dict["imputation"]
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pypots-0.4.1/pypots/imputation/base.py` & `pypots-0.5/pypots/imputation/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -64,74 +64,73 @@
         )
 
     @abstractmethod
     def fit(
         self,
         train_set: Union[dict, str],
         val_set: Optional[Union[dict, str]] = None,
-        file_type: str = "h5py",
+        file_type: str = "hdf5",
     ) -> None:
         """Train the imputer on the given data.
 
         Parameters
         ----------
         train_set :
             The dataset for model training, should be a dictionary including the key 'X',
             or a path string locating a data file.
-            If it is a dict, X should be array-like of shape [n_samples, sequence length (time steps), n_features],
+            If it is a dict, X should be array-like of shape [n_samples, sequence length (n_steps), n_features],
             which is time-series data for training, can contain missing values.
             If it is a path string, the path should point to a data file, e.g. a h5 file, which contains
             key-value pairs like a dict, and it has to include the key 'X'.
 
         val_set :
             The dataset for model validating, should be a dictionary including the key 'X',
             or a path string locating a data file.
-            If it is a dict, X should be array-like of shape [n_samples, sequence length (time steps), n_features],
+            If it is a dict, X should be array-like of shape [n_samples, sequence length (n_steps), n_features],
             which is time-series data for validating, can contain missing values.
             If it is a path string, the path should point to a data file, e.g. a h5 file, which contains
             key-value pairs like a dict, and it has to include the key 'X'.
 
-        file_type : str, default = "h5py",
+        file_type :
             The type of the given file if train_set and val_set are path strings.
 
         """
         raise NotImplementedError
 
     @abstractmethod
     def predict(
         self,
         test_set: Union[dict, str],
-        file_type: str = "h5py",
+        file_type: str = "hdf5",
     ) -> dict:
         raise NotImplementedError
 
     @abstractmethod
     def impute(
         self,
-        X: Union[dict, str],
-        file_type: str = "h5py",
+        test_set: Union[dict, str],
+        file_type: str = "hdf5",
     ) -> np.ndarray:
         """Impute missing values in the given data with the trained model.
 
         Parameters
         ----------
-        X :
-            The data samples for testing, should be array-like of shape [n_samples, sequence length (time steps),
+        test_set :
+            The data samples for testing, should be array-like of shape [n_samples, sequence length (n_steps),
             n_features], or a path string locating a data file, e.g. h5 file.
 
         file_type :
             The type of the given file if X is a path string.
 
         Returns
         -------
-        array-like, shape [n_samples, sequence length (time steps), n_features],
+        array-like, shape [n_samples, sequence length (n_steps), n_features],
             Imputed data.
         """
-        # this is for old API compatibility, will be removed in the future.
-        # Please implement predict() instead.
+
         raise NotImplementedError
 
 
 class BaseNNImputer(BaseNNModel):
     """The abstract class for all neural-network imputation models in PyPOTS.
 
     Parameters
@@ -203,15 +202,15 @@
 
     @abstractmethod
     def _assemble_input_for_training(self, data: list) -> dict:
         """Assemble the given data into a dictionary for training input.
 
         Parameters
         ----------
-        data : list,
+        data :
             Input data from dataloader, should be list.
 
         Returns
         -------
         dict,
             A python dictionary contains the input data for model training.
         """
@@ -219,15 +218,15 @@
 
     @abstractmethod
     def _assemble_input_for_validating(self, data: list) -> dict:
         """Assemble the given data into a dictionary for validating input.
 
         Parameters
         ----------
-        data : list,
+        data :
             Data output from dataloader, should be list.
 
         Returns
         -------
         dict,
             A python dictionary contains the input data for model validating.
         """
@@ -243,15 +242,15 @@
         the three stages are different, and this situation usually happens when the Dataset/Dataloader classes
         used in the train/val/test stages are not the same, e.g. the training data and validating data in a
         classification task contains labels, but the testing data (from the production environment) generally
         doesn't have labels.
 
         Parameters
         ----------
-        data : list,
+        data :
             Data output from dataloader, should be list.
 
         Returns
         -------
         dict,
             A python dictionary contains the input data for model testing.
         """
@@ -379,72 +378,67 @@
         )
 
     @abstractmethod
     def fit(
         self,
         train_set: Union[dict, str],
         val_set: Optional[Union[dict, str]] = None,
-        file_type: str = "h5py",
+        file_type: str = "hdf5",
     ) -> None:
         """Train the imputer on the given data.
 
         Parameters
         ----------
         train_set :
             The dataset for model training, should be a dictionary including the key 'X',
             or a path string locating a data file.
-            If it is a dict, X should be array-like of shape [n_samples, sequence length (time steps), n_features],
+            If it is a dict, X should be array-like of shape [n_samples, sequence length (n_steps), n_features],
             which is time-series data for training, can contain missing values.
             If it is a path string, the path should point to a data file, e.g. a h5 file, which contains
             key-value pairs like a dict, and it has to include the key 'X'.
 
         val_set :
             The dataset for model validating, should be a dictionary including the key 'X',
             or a path string locating a data file.
-            If it is a dict, X should be array-like of shape [n_samples, sequence length (time steps), n_features],
+            If it is a dict, X should be array-like of shape [n_samples, sequence length (n_steps), n_features],
             which is time-series data for validating, can contain missing values.
             If it is a path string, the path should point to a data file, e.g. a h5 file, which contains
             key-value pairs like a dict, and it has to include the key 'X'.
 
-        file_type : str, default = "h5py",
+        file_type :
             The type of the given file if train_set and val_set are path strings.
 
         """
         raise NotImplementedError
 
     @abstractmethod
     def predict(
         self,
         test_set: Union[dict, str],
-        file_type: str = "h5py",
+        file_type: str = "hdf5",
     ) -> dict:
         raise NotImplementedError
 
     @abstractmethod
     def impute(
         self,
-        X: Union[dict, str],
-        file_type: str = "h5py",
+        test_set: Union[dict, str],
+        file_type: str = "hdf5",
     ) -> np.ndarray:
         """Impute missing values in the given data with the trained model.
 
-        Warnings
-        --------
-        The method impute is deprecated. Please use `predict()` instead.
-
         Parameters
         ----------
-        X :
-            The data samples for testing, should be array-like of shape [n_samples, sequence length (time steps),
+        test_set :
+            The data samples for testing, should be array-like of shape [n_samples, sequence length (n_steps),
             n_features], or a path string locating a data file, e.g. h5 file.
 
         file_type :
             The type of the given file if X is a path string.
 
         Returns
         -------
-        array-like, shape [n_samples, sequence length (time steps), n_features],
+        array-like, shape [n_samples, sequence length (n_steps), n_features],
             Imputed data.
         """
-        # this is for old API compatibility, will be removed in the future.
-        # Please implement predict() instead.
+
         raise NotImplementedError
```

### Comparing `pypots-0.4.1/pypots/imputation/brits/data.py` & `pypots-0.5/pypots/imputation/mrnn/data.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,66 +1,72 @@
 """
-Dataset class for model BRITS.
+Dataset class for the imputation model M-RNN.
 """
 
 # Created by Wenjie Du <wenjay.du@gmail.com>
 # License: BSD-3-Clause
 
 from typing import Union, Iterable
 
 import torch
 from pygrinder import fill_and_get_mask_torch
 
-from ...data.base import BaseDataset
+from ...data.dataset import BaseDataset
 from ...data.utils import _parse_delta_torch
 
 
-class DatasetForBRITS(BaseDataset):
+class DatasetForMRNN(BaseDataset):
     """Dataset class for BRITS.
 
     Parameters
     ----------
-    data : dict or str,
+    data :
         The dataset for model input, should be a dictionary including keys as 'X' and 'y',
         or a path string locating a data file.
-        If it is a dict, X should be array-like of shape [n_samples, sequence length (time steps), n_features],
+        If it is a dict, X should be array-like of shape [n_samples, sequence length (n_steps), n_features],
         which is time-series data for input, can contain missing values, and y should be array-like of shape
         [n_samples], which is classification labels of X.
         If it is a path string, the path should point to a data file, e.g. a h5 file, which contains
         key-value pairs like a dict, and it has to include keys as 'X' and 'y'.
 
-    return_labels : bool, default = True,
+    return_y :
         Whether to return labels in function __getitem__() if they exist in the given data. If `True`, for example,
         during training of classification models, the Dataset class will return labels in __getitem__() for model input.
         Otherwise, labels won't be included in the data returned by __getitem__(). This parameter exists because we
         need the defined Dataset class for all training/validating/testing stages. For those big datasets stored in h5
         files, they already have both X and y saved. But we don't read labels from the file for validating and testing
         with function _fetch_data_from_file(), which works for all three stages. Therefore, we need this parameter for
         distinction.
 
-    file_type : str, default = "h5py"
+    file_type :
         The type of the given file if train_set and val_set are path strings.
     """
 
     def __init__(
         self,
         data: Union[dict, str],
         return_X_ori: bool,
-        return_labels: bool,
-        file_type: str = "h5py",
+        return_y: bool,
+        file_type: str = "hdf5",
     ):
-        super().__init__(data, return_X_ori, return_labels, file_type)
+        super().__init__(
+            data=data,
+            return_X_ori=return_X_ori,
+            return_X_pred=False,
+            return_y=return_y,
+            file_type=file_type,
+        )
 
         if not isinstance(self.data, str):
             # calculate all delta here.
-            if self.X_ori is None:
-                forward_X, forward_missing_mask = fill_and_get_mask_torch(self.X)
-            else:
+            if self.return_X_ori:
                 forward_missing_mask = self.missing_mask
                 forward_X = self.X
+            else:
+                forward_X, forward_missing_mask = fill_and_get_mask_torch(self.X)
 
             forward_delta = _parse_delta_torch(forward_missing_mask)
             backward_X = torch.flip(forward_X, dims=[1])
             backward_missing_mask = torch.flip(forward_missing_mask, dims=[1])
             backward_delta = _parse_delta_torch(backward_missing_mask)
 
             self.processed_data = {
@@ -77,20 +83,20 @@
             }
 
     def _fetch_data_from_array(self, idx: int) -> Iterable:
         """Fetch data from self.X if it is given.
 
         Parameters
         ----------
-        idx : int,
+        idx :
             The index of the sample to be return.
 
         Returns
         -------
-        sample : list,
+        sample :
             A list contains
 
             index : int tensor,
                 The index of the sample.
 
             X : tensor,
                 The feature vector for model input.
@@ -112,34 +118,34 @@
             self.processed_data["forward"]["delta"][idx],
             # for backward
             self.processed_data["backward"]["X"][idx],
             self.processed_data["backward"]["missing_mask"][idx],
             self.processed_data["backward"]["delta"][idx],
         ]
 
-        if self.X_ori is not None and self.return_X_ori:
+        if self.return_X_ori:
             sample.extend([self.X_ori[idx], self.indicating_mask[idx]])
 
-        if self.y is not None and self.return_labels:
+        if self.return_y:
             sample.append(self.y[idx].to(torch.long))
 
         return sample
 
     def _fetch_data_from_file(self, idx: int) -> Iterable:
         """Fetch data with the lazy-loading strategy, i.e. only loading data from the file while requesting for samples.
         Here the opened file handle doesn't load the entire dataset into RAM but only load the currently accessed slice.
 
         Parameters
         ----------
-        idx : int,
+        idx :
             The index of the sample to be return.
 
         Returns
         -------
-        sample : list,
+        sample :
             The collated data sample, a list including all necessary sample info.
         """
 
         if self.file_handle is None:
             self.file_handle = self._open_file_handle()
 
         X = torch.from_numpy(self.file_handle["X"][idx]).to(torch.float32)
@@ -165,18 +171,18 @@
             forward["deltas"],
             # for backward
             backward["X"],
             backward["missing_mask"],
             backward["deltas"],
         ]
 
-        if "X_ori" in self.file_handle.keys() and self.return_X_ori:
+        if self.return_X_ori:
             X_ori = torch.from_numpy(self.file_handle["X_ori"][idx]).to(torch.float32)
             X_ori, X_ori_missing_mask = fill_and_get_mask_torch(X_ori)
             indicating_mask = X_ori_missing_mask - missing_mask
             sample.extend([X_ori, indicating_mask])
 
         # if the dataset has labels and is for training, then fetch it from the file
-        if "y" in self.file_handle.keys() and self.return_labels:
+        if self.return_y:
             sample.append(torch.tensor(self.file_handle["y"][idx], dtype=torch.long))
 
         return sample
```

### Comparing `pypots-0.4.1/pypots/imputation/brits/model.py` & `pypots-0.5/pypots/imputation/brits/model.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,37 +1,27 @@
 """
 The implementation of BRITS for the partially-observed time-series imputation task.
 
-Refer to the paper "Wei Cao, Dong Wang, Jian Li, Hao Zhou, Lei Li, and Yitan Li.
-BRITS: Bidirectional recurrent imputation for time series.
-In Advances in Neural Information Processing Systems, volume 31. Curran Associates, Inc., 2018."
-
-Notes
------
-Partial implementation uses code from https://github.com/caow13/BRITS.
-The bugs in the original implementation are fixed here.
-
 """
 
 # Created by Wenjie Du <wenjay.du@gmail.com>
 # License: BSD-3-Clause
 
 from typing import Union, Optional
 
 import numpy as np
 import torch
 from torch.utils.data import DataLoader
 
 from .core import _BRITS
 from .data import DatasetForBRITS
 from ..base import BaseNNImputer
-from ...data.checking import check_X_ori_in_val_set
+from ...data.checking import key_in_data_set
 from ...optim.adam import Adam
 from ...optim.base import Optimizer
-from ...utils.logging import logger
 
 
 class BRITS(BaseNNImputer):
     """The PyTorch implementation of the BRITS model :cite:`cao2018BRITS`.
 
     Parameters
     ----------
@@ -190,32 +180,32 @@
     def _assemble_input_for_testing(self, data: list) -> dict:
         return self._assemble_input_for_training(data)
 
     def fit(
         self,
         train_set: Union[dict, str],
         val_set: Optional[Union[dict, str]] = None,
-        file_type: str = "h5py",
+        file_type: str = "hdf5",
     ) -> None:
         # Step 1: wrap the input data with classes Dataset and DataLoader
         training_set = DatasetForBRITS(
-            train_set, return_X_ori=False, return_labels=False, file_type=file_type
+            train_set, return_X_ori=False, return_y=False, file_type=file_type
         )
         training_loader = DataLoader(
             training_set,
             batch_size=self.batch_size,
             shuffle=True,
             num_workers=self.num_workers,
         )
         val_loader = None
         if val_set is not None:
-            if not check_X_ori_in_val_set(val_set):
+            if not key_in_data_set("X_ori", val_set):
                 raise ValueError("val_set must contain 'X_ori' for model validation.")
             val_set = DatasetForBRITS(
-                val_set, return_X_ori=True, return_labels=False, file_type=file_type
+                val_set, return_X_ori=True, return_y=False, file_type=file_type
             )
             val_loader = DataLoader(
                 val_set,
                 batch_size=self.batch_size,
                 shuffle=False,
                 num_workers=self.num_workers,
             )
@@ -227,19 +217,19 @@
 
         # Step 3: save the model if necessary
         self._auto_save_model_if_necessary(confirm_saving=True)
 
     def predict(
         self,
         test_set: Union[dict, str],
-        file_type: str = "h5py",
+        file_type: str = "hdf5",
     ) -> dict:
         self.model.eval()  # set the model as eval status to freeze it.
         test_set = DatasetForBRITS(
-            test_set, return_X_ori=False, return_labels=False, file_type=file_type
+            test_set, return_X_ori=False, return_y=False, file_type=file_type
         )
         test_loader = DataLoader(
             test_set,
             batch_size=self.batch_size,
             shuffle=False,
             num_workers=self.num_workers,
         )
@@ -256,35 +246,29 @@
         result_dict = {
             "imputation": imputation,
         }
         return result_dict
 
     def impute(
         self,
-        X: Union[dict, str],
-        file_type="h5py",
+        test_set: Union[dict, str],
+        file_type: str = "hdf5",
     ) -> np.ndarray:
         """Impute missing values in the given data with the trained model.
 
-        Warnings
-        --------
-        The method impute is deprecated. Please use `predict()` instead.
-
         Parameters
         ----------
-        X :
-            The data samples for testing, should be array-like of shape [n_samples, sequence length (time steps),
+        test_set :
+            The data samples for testing, should be array-like of shape [n_samples, sequence length (n_steps),
             n_features], or a path string locating a data file, e.g. h5 file.
 
         file_type :
             The type of the given file if X is a path string.
 
         Returns
         -------
-        array-like, shape [n_samples, sequence length (time steps), n_features],
+        array-like, shape [n_samples, sequence length (n_steps), n_features],
             Imputed data.
         """
-        logger.warning(
-            "🚨DeprecationWarning: The method impute is deprecated. Please use `predict` instead."
-        )
-        results_dict = self.predict(X, file_type=file_type)
-        return results_dict["imputation"]
+
+        result_dict = self.predict(test_set, file_type=file_type)
+        return result_dict["imputation"]
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pypots-0.4.1/pypots/imputation/crossformer/core.py` & `pypots-0.5/pypots/imputation/crossformer/core.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 """
-
+The core wrapper assembles the submodules of Crossformer imputation model
+and takes over the forward progress of the algorithm.
 """
 
 # Created by Wenjie Du <wenjay.du@gmail.com>
 # License: BSD-3-Clause
 
 from math import ceil
 
 import torch
 import torch.nn as nn
 from einops import rearrange
 
 from ...nn.modules.crossformer import CrossformerEncoder, ScaleBlock
 from ...nn.modules.patchtst import PredictionHead, PatchEmbedding
-from ...nn.modules.saits import SaitsLoss
+from ...nn.modules.saits import SaitsLoss, SaitsEmbedding
 
 
 class _Crossformer(nn.Module):
     def __init__(
         self,
         n_steps,
         n_features,
         n_layers,
-        n_heads,
         d_model,
+        n_heads,
         d_ffn,
         factor,
         seg_len,
         win_size,
         dropout,
         ORT_weight: float = 1,
         MIT_weight: float = 1,
@@ -68,30 +69,34 @@
                     factor,
                 )
                 for layer in range(n_layers)
             ]
         )
 
         self.head = PredictionHead(d_model, out_seg_num, n_steps, dropout)
-        self.embedding = nn.Linear(n_features * 2, d_model)
+        self.saits_embedding = SaitsEmbedding(
+            n_features * 2,
+            d_model,
+            with_pos=False,
+        )
         self.output_projection = nn.Linear(d_model, n_features)
 
         # apply SAITS loss function to Crossformer on the imputation task
         self.saits_loss_func = SaitsLoss(ORT_weight, MIT_weight)
 
     def forward(self, inputs: dict, training: bool = True) -> dict:
         X, missing_mask = inputs["X"], inputs["missing_mask"]
 
         # WDU: the original Crossformer paper isn't proposed for imputation task. Hence the model doesn't take
         # the missing mask into account, which means, in the process, the model doesn't know which part of
-        # the input data is missing, and this may hurt the model's imputation performance. Therefore, I add the
-        # embedding layers to project the concatenation of features and masks into a hidden space, as well as
+        # the input data is missing, and this may hurt the model's imputation performance. Therefore, I apply the
+        # SAITS embedding method to project the concatenation of features and masks into a hidden space, as well as
         # the output layers to project back from the hidden space to the original space.
-        # embedding
-        input_X = self.embedding(torch.cat([X, missing_mask], dim=2))
+        input_X = self.saits_embedding(X, missing_mask)
+
         x_enc = self.enc_value_embedding(input_X.permute(0, 2, 1))
         x_enc = rearrange(
             x_enc, "(b d) seg_num d_model -> b d seg_num d_model", d=self.d_model
         )
         x_enc += self.enc_pos_embedding
 
         # Crossformer processing
```

### Comparing `pypots-0.4.1/pypots/imputation/crossformer/data.py` & `pypots-0.5/pypots/imputation/frets/data.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 """
-Dataset class for Crossformer.
+Dataset class for the imputation model FreTS.
 """
 
 # Created by Wenjie Du <wenjay.du@gmail.com>
 # License: BSD-3-Clause
 
 from typing import Union
 
 from ..saits.data import DatasetForSAITS
 
 
-class DatasetForCrossformer(DatasetForSAITS):
-    """Actually Crossformer uses the same data strategy as SAITS, needs MIT for training."""
+class DatasetForFreTS(DatasetForSAITS):
+    """Actually FreTS uses the same data strategy as SAITS, needs MIT for training."""
 
     def __init__(
         self,
         data: Union[dict, str],
         return_X_ori: bool,
-        return_labels: bool,
-        file_type: str = "h5py",
+        return_y: bool,
+        file_type: str = "hdf5",
         rate: float = 0.2,
     ):
-        super().__init__(data, return_X_ori, return_labels, file_type, rate)
+        super().__init__(data, return_X_ori, return_y, file_type, rate)
```

### Comparing `pypots-0.4.1/pypots/imputation/crossformer/model.py` & `pypots-0.5/pypots/imputation/crossformer/model.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,38 +1,28 @@
 """
 The implementation of Crossformer for the partially-observed time-series imputation task.
 
-Refer to the paper "Yunhao Zhang and Junchi Yan.
-Crossformer: Transformer utilizing cross-dimension dependency for multivariate time series forecasting.
-In The 11th ICLR, 2023."
-
-Notes
------
-Partial implementation uses code from
-https://github.com/Thinklab-SJTU/Crossformer and https://github.com/thuml/Time-Series-Library
-
 """
 
 # Created by Wenjie Du <wenjay.du@gmail.com>
 # License: BSD-3-Clause
 
 from typing import Union, Optional
 
 import numpy as np
 import torch
 from torch.utils.data import DataLoader
 
+from .core import _Crossformer
 from .data import DatasetForCrossformer
-from pypots.imputation.crossformer.core import _Crossformer
 from ..base import BaseNNImputer
-from ...data.base import BaseDataset
-from ...data.checking import check_X_ori_in_val_set
+from ...data.checking import key_in_data_set
+from ...data.dataset import BaseDataset
 from ...optim.adam import Adam
 from ...optim.base import Optimizer
-from ...utils.logging import logger
 
 
 class Crossformer(BaseNNImputer):
     """The PyTorch implementation of the Crossformer model.
     Crossformer is originally proposed by Zhang et al. in :cite:`zhang2023crossformer`.
 
     Parameters
@@ -42,20 +32,20 @@
 
     n_features :
         The number of features in the time-series data sample.
 
     n_layers :
         The number of layers in the 1st and 2nd DMSA blocks in the SAITS model.
 
-    n_heads:
-        The number of heads in the multi-head attention mechanism.
-
     d_model :
         The dimension of the model.
 
+    n_heads:
+        The number of heads in the multi-head attention mechanism.
+
     d_ffn :
         The dimension of the feed-forward network.
 
     factor :
         The num of routers in Cross-Dimension Stage of TSA (c).
 
     seg_len :
@@ -115,16 +105,16 @@
     """
 
     def __init__(
         self,
         n_steps: int,
         n_features: int,
         n_layers: int,
-        n_heads: int,
         d_model: int,
+        n_heads: int,
         d_ffn: int,
         factor: int,
         seg_len: int,
         win_size: int,
         dropout: float = 0,
         ORT_weight: float = 1,
         MIT_weight: float = 1,
@@ -162,16 +152,16 @@
         self.MIT_weight = MIT_weight
 
         # set up the model
         self.model = _Crossformer(
             self.n_steps,
             self.n_features,
             self.n_layers,
-            self.n_heads,
             self.d_model,
+            self.n_heads,
             self.d_ffn,
             self.factor,
             self.seg_len,
             self.win_size,
             self.dropout,
             self.ORT_weight,
             self.MIT_weight,
@@ -214,32 +204,32 @@
 
         return inputs
 
     def fit(
         self,
         train_set: Union[dict, str],
         val_set: Optional[Union[dict, str]] = None,
-        file_type: str = "h5py",
+        file_type: str = "hdf5",
     ) -> None:
         # Step 1: wrap the input data with classes Dataset and DataLoader
         training_set = DatasetForCrossformer(
-            train_set, return_X_ori=False, return_labels=False, file_type=file_type
+            train_set, return_X_ori=False, return_y=False, file_type=file_type
         )
         training_loader = DataLoader(
             training_set,
             batch_size=self.batch_size,
             shuffle=True,
             num_workers=self.num_workers,
         )
         val_loader = None
         if val_set is not None:
-            if not check_X_ori_in_val_set(val_set):
+            if not key_in_data_set("X_ori", val_set):
                 raise ValueError("val_set must contain 'X_ori' for model validation.")
             val_set = DatasetForCrossformer(
-                val_set, return_X_ori=True, return_labels=False, file_type=file_type
+                val_set, return_X_ori=True, return_y=False, file_type=file_type
             )
             val_loader = DataLoader(
                 val_set,
                 batch_size=self.batch_size,
                 shuffle=False,
                 num_workers=self.num_workers,
             )
@@ -251,42 +241,46 @@
 
         # Step 3: save the model if necessary
         self._auto_save_model_if_necessary(confirm_saving=True)
 
     def predict(
         self,
         test_set: Union[dict, str],
-        file_type: str = "h5py",
+        file_type: str = "hdf5",
     ) -> dict:
         """Make predictions for the input data with the trained model.
 
         Parameters
         ----------
         test_set : dict or str
             The dataset for model validating, should be a dictionary including keys as 'X',
             or a path string locating a data file supported by PyPOTS (e.g. h5 file).
-            If it is a dict, X should be array-like of shape [n_samples, sequence length (time steps), n_features],
+            If it is a dict, X should be array-like of shape [n_samples, sequence length (n_steps), n_features],
             which is time-series data for validating, can contain missing values, and y should be array-like of shape
             [n_samples], which is classification labels of X.
             If it is a path string, the path should point to a data file, e.g. a h5 file, which contains
             key-value pairs like a dict, and it has to include keys as 'X' and 'y'.
 
-        file_type : str
+        file_type :
             The type of the given file if test_set is a path string.
 
         Returns
         -------
-        result_dict : dict,
+        file_type :
             The dictionary containing the clustering results and latent variables if necessary.
 
         """
         # Step 1: wrap the input data with classes Dataset and DataLoader
         self.model.eval()  # set the model as eval status to freeze it.
         test_set = BaseDataset(
-            test_set, return_X_ori=False, return_labels=False, file_type=file_type
+            test_set,
+            return_X_ori=False,
+            return_X_pred=False,
+            return_y=False,
+            file_type=file_type,
         )
         test_loader = DataLoader(
             test_set,
             batch_size=self.batch_size,
             shuffle=False,
             num_workers=self.num_workers,
         )
@@ -304,36 +298,29 @@
         result_dict = {
             "imputation": imputation,
         }
         return result_dict
 
     def impute(
         self,
-        X: Union[dict, str],
-        file_type="h5py",
+        test_set: Union[dict, str],
+        file_type: str = "hdf5",
     ) -> np.ndarray:
         """Impute missing values in the given data with the trained model.
 
-        Warnings
-        --------
-        The method impute is deprecated. Please use `predict()` instead.
-
         Parameters
         ----------
-        X :
-            The data samples for testing, should be array-like of shape [n_samples, sequence length (time steps),
+        test_set :
+            The data samples for testing, should be array-like of shape [n_samples, sequence length (n_steps),
             n_features], or a path string locating a data file, e.g. h5 file.
 
         file_type :
             The type of the given file if X is a path string.
 
         Returns
         -------
-        array-like, shape [n_samples, sequence length (time steps), n_features],
+        array-like, shape [n_samples, sequence length (n_steps), n_features],
             Imputed data.
         """
-        logger.warning(
-            "🚨DeprecationWarning: The method impute is deprecated. Please use `predict` instead."
-        )
 
-        results_dict = self.predict(X, file_type=file_type)
-        return results_dict["imputation"]
+        result_dict = self.predict(test_set, file_type=file_type)
+        return result_dict["imputation"]
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pypots-0.4.1/pypots/imputation/csdi/data.py` & `pypots-0.5/pypots/imputation/csdi/data.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,35 +1,50 @@
 """
-
+Dataset class for the imputation model CSDI.
 """
 
 # Created by Wenjie Du <wenjay.du@gmail.com>
 # License: BSD-3-Clause
 
 from typing import Union, Iterable
 
 import numpy as np
 import torch
 from pygrinder import fill_and_get_mask_torch
 
-from ...data.base import BaseDataset
+from ...data.dataset import BaseDataset
 
 
 class DatasetForCSDI(BaseDataset):
-    """Dataset for CSDI model."""
+    """Dataset for CSDI model.
+
+    Notes
+    -----
+    In CSDI official code, `observed_mask` indicates all observed values in raw data.
+    `gt_mask` indicates all observed values in the input data.
+    `observed_mask` - `gt_mask` = `indicating_mask` in our code.
+    `cond_mask`, for testing, it is `gt_mask`; for training, it is `observed_mask`
+    includes some artificially missing values.
+
+    """
 
     def __init__(
         self,
         data: Union[dict, str],
         target_strategy: str,
         return_X_ori: bool,
-        return_labels: bool,
-        file_type: str = "h5py",
+        file_type: str = "hdf5",
     ):
-        super().__init__(data, return_X_ori, return_labels, file_type)
+        super().__init__(
+            data=data,
+            return_X_ori=return_X_ori,
+            return_X_pred=False,
+            return_y=False,
+            file_type=file_type,
+        )
         assert target_strategy in ["random", "hist", "mix"]
         self.target_strategy = target_strategy
 
     @staticmethod
     def get_rand_mask(observed_mask):
         rand_for_mask = torch.rand_like(observed_mask) * observed_mask
         rand_for_mask = rand_for_mask.reshape(-1)
@@ -51,20 +66,20 @@
         return cond_mask
 
     def _fetch_data_from_array(self, idx: int) -> Iterable:
         """Fetch data according to index.
 
         Parameters
         ----------
-        idx : int,
+        idx :
             The index to fetch the specified sample.
 
         Returns
         -------
-        sample : list,
+        sample :
             A list contains
 
             index : int tensor,
                 The index of the sample.
 
             observed_data : tensor,
                 Time-series data with all observed values for model input.
@@ -76,15 +91,15 @@
                 The mask records all originally and artificially missing values to the model.
 
             observed_tp : tensor,
                 The time points (timestamp) of the observed data.
 
         """
 
-        if self.X_ori is not None and self.return_X_ori:
+        if self.return_X_ori:
             observed_data = self.X_ori[idx]
             cond_mask = self.missing_mask[idx]
             indicating_mask = self.indicating_mask[idx]
         else:
             observed_data = self.X[idx]
             observed_data, observed_mask = fill_and_get_mask_torch(observed_data)
             if self.target_strategy == "random":
@@ -113,31 +128,31 @@
             torch.tensor(idx),
             observed_data,
             indicating_mask,
             cond_mask,
             observed_tp,
         ]
 
-        if self.y is not None and self.return_labels:
+        if self.return_y:
             sample.append(self.y[idx].to(torch.long))
 
         return sample
 
     def _fetch_data_from_file(self, idx: int) -> Iterable:
         """Fetch data with the lazy-loading strategy, i.e. only loading data from the file while requesting for samples.
         Here the opened file handle doesn't load the entire dataset into RAM but only load the currently accessed slice.
 
         Parameters
         ----------
-        idx : int,
+        idx :
             The index of the sample to be return.
 
         Returns
         -------
-        sample : list,
+        sample :
             A list contains
 
             index : int tensor,
                 The index of the sample.
 
             observed_data : tensor,
                 Time-series data with all observed values for model input.
@@ -152,15 +167,15 @@
                 The time points (timestamp) of the observed data.
 
         """
 
         if self.file_handle is None:
             self.file_handle = self._open_file_handle()
 
-        if "X_ori" in self.file_handle.keys() and self.return_X_ori:
+        if self.return_X_ori:
             observed_data = torch.from_numpy(self.file_handle["X_ori"][idx]).to(
                 torch.float32
             )
             observed_data, observed_mask = fill_and_get_mask_torch(observed_data)
             X = torch.from_numpy(self.file_handle["X"][idx]).to(torch.float32)
             _, cond_mask = fill_and_get_mask_torch(X)
             indicating_mask = observed_mask - cond_mask
@@ -199,43 +214,42 @@
             torch.tensor(idx),
             observed_data,
             indicating_mask,
             cond_mask,
             observed_tp,
         ]
 
-        if "y" in self.file_handle.keys() and self.return_labels:
+        if self.return_y:
             sample.append(torch.tensor(self.file_handle["y"][idx], dtype=torch.long))
 
         return sample
 
 
 class TestDatasetForCSDI(DatasetForCSDI):
     """Test dataset for CSDI model."""
 
     def __init__(
         self,
         data: Union[dict, str],
         return_X_ori: bool,
-        return_labels: bool,
-        file_type: str = "h5py",
+        file_type: str = "hdf5",
     ):
-        super().__init__(data, "random", return_X_ori, return_labels, file_type)
+        super().__init__(data, "random", return_X_ori, file_type)
 
     def _fetch_data_from_array(self, idx: int) -> Iterable:
         """Fetch data according to index.
 
         Parameters
         ----------
-        idx : int,
+        idx :
             The index to fetch the specified sample.
 
         Returns
         -------
-        sample : list,
+        sample :
             A list contains
 
             index : int tensor,
                 The index of the sample.
 
             observed_data : tensor,
                 Time-series data with all observed values for model input.
@@ -260,31 +274,31 @@
         sample = [
             torch.tensor(idx),
             observed_data,
             cond_mask,
             observed_tp,
         ]
 
-        if self.y is not None and self.return_labels:
+        if self.return_y:
             sample.append(self.y[idx].to(torch.long))
 
         return sample
 
     def _fetch_data_from_file(self, idx: int) -> Iterable:
         """Fetch data with the lazy-loading strategy, i.e. only loading data from the file while requesting for samples.
         Here the opened file handle doesn't load the entire dataset into RAM but only load the currently accessed slice.
 
         Parameters
         ----------
-        idx : int,
+        idx :
             The index of the sample to be return.
 
         Returns
         -------
-        sample : list,
+        sample :
             A list contains
 
             index : int tensor,
                 The index of the sample.
 
             observed_data : tensor,
                 Time-series data with all observed values for model input.
@@ -315,11 +329,11 @@
         sample = [
             torch.tensor(idx),
             observed_data,
             cond_mask,
             observed_tp,
         ]
 
-        if "y" in self.file_handle.keys() and self.return_labels:
+        if self.return_y:
             sample.append(torch.tensor(self.file_handle["y"][idx], dtype=torch.long))
 
         return sample
```

### Comparing `pypots-0.4.1/pypots/imputation/csdi/model.py` & `pypots-0.5/pypots/imputation/csdi/model.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,10 @@
 """
 The implementation of CSDI for the partially-observed time-series imputation task.
 
-Refer to the paper "Yusuke Tashiro, Jiaming Song, Yang Song, and Stefano Ermon.
-CSDI: Conditional Score-based Diffusion Models for Probabilistic Time Series Imputation.
-In NeurIPS, 2021."
-
-Notes
------
-Partial implementation uses code from the official implementation https://github.com/ermongroup/CSDI.
-
 """
 
 # Created by Wenjie Du <wenjay.du@gmail.com>
 # License: BSD-3-Clause
 
 import os
 from typing import Union, Optional
@@ -25,25 +17,28 @@
     import nni
 except ImportError:
     pass
 
 from .core import _CSDI
 from .data import DatasetForCSDI, TestDatasetForCSDI
 from ..base import BaseNNImputer
-from ...data.checking import check_X_ori_in_val_set
+from ...data.checking import key_in_data_set
 from ...optim.adam import Adam
 from ...optim.base import Optimizer
 from ...utils.logging import logger
 
 
 class CSDI(BaseNNImputer):
     """The PyTorch implementation of the CSDI model :cite:`tashiro2021csdi`.
 
     Parameters
     ----------
+    n_steps :
+        The number of time steps in the time-series data sample.
+
     n_features :
         The number of features in the time-series data sample.
 
     n_layers :
         The number of layers in the CSDI model.
 
     n_heads :
@@ -118,14 +113,15 @@
         better than in previous epochs.
         The "all" strategy will save every model after each epoch training.
 
     """
 
     def __init__(
         self,
+        n_steps: int,
         n_features: int,
         n_layers: int,
         n_heads: int,
         n_channels: int,
         d_time_embedding: int,
         d_feature_embedding: int,
         d_diffusion_embedding: int,
@@ -151,22 +147,23 @@
             num_workers,
             device,
             saving_path,
             model_saving_strategy,
         )
         assert target_strategy in ["mix", "random"]
         assert schedule in ["quad", "linear"]
+        self.n_steps = n_steps
         self.target_strategy = target_strategy
 
         # set up the model
         self.model = _CSDI(
+            n_features,
             n_layers,
             n_heads,
             n_channels,
-            n_features,
             d_time_embedding,
             d_feature_embedding,
             d_diffusion_embedding,
             is_unconditional,
             n_diffusion_steps,
             schedule,
             beta_start,
@@ -192,18 +189,18 @@
             "X_ori": X_ori.permute(0, 2, 1),  # ori observed part for model hint
             "indicating_mask": indicating_mask.permute(0, 2, 1),  # for loss calc
             "cond_mask": cond_mask.permute(0, 2, 1),  # for masking X_ori
             "observed_tp": observed_tp,
         }
         return inputs
 
-    def _assemble_input_for_validating(self, data) -> dict:
+    def _assemble_input_for_validating(self, data: list) -> dict:
         return self._assemble_input_for_training(data)
 
-    def _assemble_input_for_testing(self, data) -> dict:
+    def _assemble_input_for_testing(self, data: list) -> dict:
         (
             indices,
             X,
             cond_mask,
             observed_tp,
         ) = self._send_data_to_given_device(data)
 
@@ -327,40 +324,38 @@
             f"Finished training. The best model is from epoch#{self.best_epoch}."
         )
 
     def fit(
         self,
         train_set: Union[dict, str],
         val_set: Optional[Union[dict, str]] = None,
-        file_type: str = "h5py",
+        file_type: str = "hdf5",
         n_sampling_times: int = 1,
     ) -> None:
         # Step 1: wrap the input data with classes Dataset and DataLoader
         training_set = DatasetForCSDI(
             train_set,
             self.target_strategy,
             return_X_ori=False,
-            return_labels=False,
             file_type=file_type,
         )
         training_loader = DataLoader(
             training_set,
             batch_size=self.batch_size,
             shuffle=True,
             num_workers=self.num_workers,
         )
         val_loader = None
         if val_set is not None:
-            if not check_X_ori_in_val_set(val_set):
+            if not key_in_data_set("X_ori", val_set):
                 raise ValueError("val_set must contain 'X_ori' for model validation.")
             val_set = DatasetForCSDI(
                 val_set,
                 self.target_strategy,
                 return_X_ori=True,
-                return_labels=False,
                 file_type=file_type,
             )
             val_loader = DataLoader(
                 val_set,
                 batch_size=self.batch_size,
                 shuffle=False,
                 num_workers=self.num_workers,
@@ -373,31 +368,31 @@
 
         # Step 3: save the model if necessary
         self._auto_save_model_if_necessary(confirm_saving=True)
 
     def predict(
         self,
         test_set: Union[dict, str],
-        file_type: str = "h5py",
+        file_type: str = "hdf5",
         n_sampling_times: int = 1,
     ) -> dict:
         """
 
         Parameters
         ----------
         test_set : dict or str
             The dataset for model validating, should be a dictionary including keys as 'X' and 'y',
             or a path string locating a data file.
-            If it is a dict, X should be array-like of shape [n_samples, sequence length (time steps), n_features],
+            If it is a dict, X should be array-like of shape [n_samples, sequence length (n_steps), n_features],
             which is time-series data for validating, can contain missing values, and y should be array-like of shape
             [n_samples], which is classification labels of X.
             If it is a path string, the path should point to a data file, e.g. a h5 file, which contains
             key-value pairs like a dict, and it has to include keys as 'X' and 'y'.
 
-        file_type : str
+        file_type :
             The type of the given file if test_set is a path string.
 
         n_sampling_times:
             The number of sampling times for the model to sample from the diffusion process.
 
         Returns
         -------
@@ -406,17 +401,15 @@
             It should be a dictionary including a key named 'imputation'.
 
         """
         assert n_sampling_times > 0, "n_sampling_times should be greater than 0."
 
         # Step 1: wrap the input data with classes Dataset and DataLoader
         self.model.eval()  # set the model as eval status to freeze it.
-        test_set = TestDatasetForCSDI(
-            test_set, return_X_ori=False, return_labels=False, file_type=file_type
-        )
+        test_set = TestDatasetForCSDI(test_set, return_X_ori=False, file_type=file_type)
         test_loader = DataLoader(
             test_set,
             batch_size=self.batch_size,
             shuffle=False,
             num_workers=self.num_workers,
         )
         imputation_collector = []
@@ -438,35 +431,29 @@
         result_dict = {
             "imputation": imputation,
         }
         return result_dict
 
     def impute(
         self,
-        X: Union[dict, str],
-        file_type="h5py",
+        test_set: Union[dict, str],
+        file_type: str = "hdf5",
     ) -> np.ndarray:
         """Impute missing values in the given data with the trained model.
 
-        Warnings
-        --------
-        The method impute is deprecated. Please use `predict()` instead.
-
         Parameters
         ----------
-        X :
-            The data samples for testing, should be array-like of shape [n_samples, sequence length (time steps),
+        test_set :
+            The data samples for testing, should be array-like of shape [n_samples, sequence length (n_steps),
             n_features], or a path string locating a data file, e.g. h5 file.
 
         file_type :
             The type of the given file if X is a path string.
 
         Returns
         -------
-        array-like, shape [n_samples, sequence length (time steps), n_features],
+        array-like, shape [n_samples, sequence length (n_steps), n_features],
             Imputed data.
         """
-        logger.warning(
-            "🚨DeprecationWarning: The method impute is deprecated. Please use `predict` instead."
-        )
-        results_dict = self.predict(X, file_type=file_type)
-        return results_dict["imputation"]
+
+        result_dict = self.predict(test_set, file_type=file_type)
+        return result_dict["imputation"]
```

### Comparing `pypots-0.4.1/pypots/imputation/dlinear/core.py` & `pypots-0.5/pypots/imputation/dlinear/core.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 """
-
+The core wrapper assembles the submodules of DLinear imputation model
+and takes over the forward progress of the algorithm.
 """
 
 # Created by Wenjie Du <wenjay.du@gmail.com>
 # License: BSD-3-Clause
 
 from typing import Optional
 
-import torch
 import torch.nn as nn
 
 from ...nn.modules.autoformer import SeriesDecompositionBlock
 from ...nn.modules.dlinear import BackboneDLinear
-from ...nn.modules.saits import SaitsLoss
+from ...nn.modules.saits import SaitsLoss, SaitsEmbedding
 
 
 class _DLinear(nn.Module):
     def __init__(
         self,
         n_steps: int,
         n_features: int,
@@ -32,16 +32,20 @@
         self.n_features = n_features
         self.individual = individual
 
         self.series_decomp = SeriesDecompositionBlock(moving_avg_window_size)
         self.backbone = BackboneDLinear(n_steps, n_features, individual, d_model)
 
         if not individual:
-            self.linear_seasonal_embedding = nn.Linear(n_features * 2, d_model)
-            self.linear_trend_embedding = nn.Linear(n_features * 2, d_model)
+            self.seasonal_saits_embedding = SaitsEmbedding(
+                n_features * 2, d_model, with_pos=False
+            )
+            self.trend_saits_embedding = SaitsEmbedding(
+                n_features * 2, d_model, with_pos=False
+            )
             self.linear_seasonal_output = nn.Linear(d_model, n_features)
             self.linear_trend_output = nn.Linear(d_model, n_features)
 
         # apply SAITS loss function to Transformer on the imputation task
         self.saits_loss_func = SaitsLoss(ORT_weight, MIT_weight)
 
     def forward(self, inputs: dict, training: bool = True) -> dict:
@@ -49,22 +53,20 @@
 
         # input preprocessing and embedding for DLinear
         seasonal_init, trend_init = self.series_decomp(X)
 
         if not self.individual:
             # WDU: the original DLinear paper isn't proposed for imputation task. Hence the model doesn't take
             # the missing mask into account, which means, in the process, the model doesn't know which part of
-            # the input data is missing, and this may hurt the model's imputation performance. Therefore, I add the
-            # embedding layers to project the concatenation of features and masks into a hidden space, as well as
+            # the input data is missing, and this may hurt the model's imputation performance. Therefore, I apply the
+            # SAITS embedding method to project the concatenation of features and masks into a hidden space, as well as
             # the output layers to project the seasonal and trend from the hidden space to the original space.
             # But this is only for the non-individual mode.
-            seasonal_init = torch.cat([seasonal_init, missing_mask], dim=2)
-            trend_init = torch.cat([trend_init, missing_mask], dim=2)
-            seasonal_init = self.linear_seasonal_embedding(seasonal_init)
-            trend_init = self.linear_trend_embedding(trend_init)
+            seasonal_init = self.seasonal_saits_embedding(seasonal_init, missing_mask)
+            trend_init = self.trend_saits_embedding(trend_init, missing_mask)
 
         seasonal_output, trend_output = self.backbone(seasonal_init, trend_init)
 
         if not self.individual:
             seasonal_output = self.linear_seasonal_output(seasonal_output)
             trend_output = self.linear_trend_output(trend_output)
```

### Comparing `pypots-0.4.1/pypots/imputation/dlinear/data.py` & `pypots-0.5/pypots/imputation/film/data.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 """
-Dataset class for DLinear.
+Dataset class for the imputation model FiLM.
 """
 
 # Created by Wenjie Du <wenjay.du@gmail.com>
 # License: BSD-3-Clause
 
 from typing import Union
 
 from ..saits.data import DatasetForSAITS
 
 
-class DatasetForDLinear(DatasetForSAITS):
-    """Actually DLinear uses the same data strategy as SAITS, needs MIT for training."""
+class DatasetForFiLM(DatasetForSAITS):
+    """Actually FiLM uses the same data strategy as SAITS, needs MIT for training."""
 
     def __init__(
         self,
         data: Union[dict, str],
         return_X_ori: bool,
-        return_labels: bool,
-        file_type: str = "h5py",
+        return_y: bool,
+        file_type: str = "hdf5",
         rate: float = 0.2,
     ):
-        super().__init__(data, return_X_ori, return_labels, file_type, rate)
+        super().__init__(data, return_X_ori, return_y, file_type, rate)
```

### Comparing `pypots-0.4.1/pypots/imputation/dlinear/model.py` & `pypots-0.5/pypots/imputation/dlinear/model.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,38 +1,28 @@
 """
 The implementation of DLinear for the partially-observed time-series imputation task.
 
-Refer to the paper "Ailing Zeng, Muxi Chen, Lei Zhang, and Qiang Xu.
-Are transformers effective for time series forecasting?
-In AAAI, volume 37, pages 11121–11128, Jun. 2023.".
-
-Notes
------
-Partial implementation uses code from
-https://github.com/cure-lab/LTSF-Linear and https://github.com/thuml/Time-Series-Library
-
 """
 
 # Created by Wenjie Du <wenjay.du@gmail.com>
 # License: BSD-3-Clause
 
 from typing import Union, Optional
 
 import numpy as np
 import torch
 from torch.utils.data import DataLoader
 
+from .core import _DLinear
 from .data import DatasetForDLinear
-from pypots.imputation.dlinear.core import _DLinear
 from ..base import BaseNNImputer
-from ...data.base import BaseDataset
-from ...data.checking import check_X_ori_in_val_set
+from ...data.checking import key_in_data_set
+from ...data.dataset import BaseDataset
 from ...optim.adam import Adam
 from ...optim.base import Optimizer
-from ...utils.logging import logger
 
 
 class DLinear(BaseNNImputer):
     """The PyTorch implementation of the DLinear model.
     DLinear is originally proposed by Zeng et al. in :cite:`zeng2023dlinear`.
 
     Parameters
@@ -185,32 +175,32 @@
 
         return inputs
 
     def fit(
         self,
         train_set: Union[dict, str],
         val_set: Optional[Union[dict, str]] = None,
-        file_type: str = "h5py",
+        file_type: str = "hdf5",
     ) -> None:
         # Step 1: wrap the input data with classes Dataset and DataLoader
         training_set = DatasetForDLinear(
-            train_set, return_X_ori=False, return_labels=False, file_type=file_type
+            train_set, return_X_ori=False, return_y=False, file_type=file_type
         )
         training_loader = DataLoader(
             training_set,
             batch_size=self.batch_size,
             shuffle=True,
             num_workers=self.num_workers,
         )
         val_loader = None
         if val_set is not None:
-            if not check_X_ori_in_val_set(val_set):
+            if not key_in_data_set("X_ori", val_set):
                 raise ValueError("val_set must contain 'X_ori' for model validation.")
             val_set = DatasetForDLinear(
-                val_set, return_X_ori=True, return_labels=False, file_type=file_type
+                val_set, return_X_ori=True, return_y=False, file_type=file_type
             )
             val_loader = DataLoader(
                 val_set,
                 batch_size=self.batch_size,
                 shuffle=False,
                 num_workers=self.num_workers,
             )
@@ -222,42 +212,46 @@
 
         # Step 3: save the model if necessary
         self._auto_save_model_if_necessary(confirm_saving=True)
 
     def predict(
         self,
         test_set: Union[dict, str],
-        file_type: str = "h5py",
+        file_type: str = "hdf5",
     ) -> dict:
         """Make predictions for the input data with the trained model.
 
         Parameters
         ----------
         test_set : dict or str
             The dataset for model validating, should be a dictionary including keys as 'X',
             or a path string locating a data file supported by PyPOTS (e.g. h5 file).
-            If it is a dict, X should be array-like of shape [n_samples, sequence length (time steps), n_features],
+            If it is a dict, X should be array-like of shape [n_samples, sequence length (n_steps), n_features],
             which is time-series data for validating, can contain missing values, and y should be array-like of shape
             [n_samples], which is classification labels of X.
             If it is a path string, the path should point to a data file, e.g. a h5 file, which contains
             key-value pairs like a dict, and it has to include keys as 'X' and 'y'.
 
-        file_type : str
+        file_type :
             The type of the given file if test_set is a path string.
 
         Returns
         -------
-        result_dict : dict,
+        file_type :
             The dictionary containing the clustering results and latent variables if necessary.
 
         """
         # Step 1: wrap the input data with classes Dataset and DataLoader
         self.model.eval()  # set the model as eval status to freeze it.
         test_set = BaseDataset(
-            test_set, return_X_ori=False, return_labels=False, file_type=file_type
+            test_set,
+            return_X_ori=False,
+            return_X_pred=False,
+            return_y=False,
+            file_type=file_type,
         )
         test_loader = DataLoader(
             test_set,
             batch_size=self.batch_size,
             shuffle=False,
             num_workers=self.num_workers,
         )
@@ -275,36 +269,29 @@
         result_dict = {
             "imputation": imputation,
         }
         return result_dict
 
     def impute(
         self,
-        X: Union[dict, str],
-        file_type="h5py",
+        test_set: Union[dict, str],
+        file_type: str = "hdf5",
     ) -> np.ndarray:
         """Impute missing values in the given data with the trained model.
 
-        Warnings
-        --------
-        The method impute is deprecated. Please use `predict()` instead.
-
         Parameters
         ----------
-        X :
-            The data samples for testing, should be array-like of shape [n_samples, sequence length (time steps),
+        test_set :
+            The data samples for testing, should be array-like of shape [n_samples, sequence length (n_steps),
             n_features], or a path string locating a data file, e.g. h5 file.
 
         file_type :
             The type of the given file if X is a path string.
 
         Returns
         -------
-        array-like, shape [n_samples, sequence length (time steps), n_features],
+        array-like, shape [n_samples, sequence length (n_steps), n_features],
             Imputed data.
         """
-        logger.warning(
-            "🚨DeprecationWarning: The method impute is deprecated. Please use `predict` instead."
-        )
 
-        results_dict = self.predict(X, file_type=file_type)
-        return results_dict["imputation"]
+        result_dict = self.predict(test_set, file_type=file_type)
+        return result_dict["imputation"]
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pypots-0.4.1/pypots/imputation/etsformer/core.py` & `pypots-0.5/pypots/imputation/informer/core.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,102 +1,93 @@
 """
-
+The core wrapper assembles the submodules of Informer imputation model
+and takes over the forward progress of the algorithm.
 """
 
 # Created by Wenjie Du <wenjay.du@gmail.com>
 # License: BSD-3-Clause
 
-import torch
 import torch.nn as nn
 
-from ...nn.modules.etsformer import (
-    ETSformerEncoderLayer,
-    ETSformerEncoder,
-    ETSformerDecoderLayer,
-    ETSformerDecoder,
+from ...nn.modules.informer import (
+    ProbAttention,
+    ConvLayer,
+    InformerEncoderLayer,
+    InformerEncoder,
 )
-from ...nn.modules.saits import SaitsLoss
-from ...nn.modules.transformer.embedding import DataEmbedding
+from ...nn.modules.saits import SaitsLoss, SaitsEmbedding
+from ...nn.modules.transformer import MultiHeadAttention
 
 
-class _ETSformer(nn.Module):
+class _Informer(nn.Module):
     def __init__(
         self,
         n_steps,
         n_features,
-        n_e_layers,
-        n_d_layers,
-        n_heads,
+        n_layers,
         d_model,
+        n_heads,
         d_ffn,
+        factor,
         dropout,
-        top_k,
         ORT_weight: float = 1,
         MIT_weight: float = 1,
-        activation="sigmoid",
+        distil=False,
+        activation="relu",
     ):
         super().__init__()
 
-        self.enc_embedding = DataEmbedding(
+        self.saits_embedding = SaitsEmbedding(
             n_features * 2,
             d_model,
+            with_pos=True,
+            n_max_steps=n_steps,
             dropout=dropout,
         )
-
-        # Encoder
-        self.encoder = ETSformerEncoder(
-            [
-                ETSformerEncoderLayer(
-                    d_model,
-                    n_heads,
-                    n_features,
-                    n_steps,
-                    n_steps,
-                    top_k,
-                    dim_feedforward=d_ffn,
-                    dropout=dropout,
-                    activation=activation,
-                )
-                for _ in range(n_e_layers)
-            ]
-        )
-        # Decoder
-        self.decoder = ETSformerDecoder(
+        self.encoder = InformerEncoder(
             [
-                ETSformerDecoderLayer(
+                InformerEncoderLayer(
+                    MultiHeadAttention(
+                        ProbAttention(False, factor, dropout),
+                        d_model,
+                        n_heads,
+                        d_model // n_heads,
+                        d_model // n_heads,
+                    ),
                     d_model,
-                    n_heads,
-                    n_features,
-                    n_steps,
-                    dropout=dropout,
+                    d_ffn,
+                    dropout,
+                    activation,
                 )
-                for _ in range(n_d_layers)
+                for _ in range(n_layers)
             ],
+            [ConvLayer(d_model) for _ in range(n_layers - 1)] if distil else None,
+            norm_layer=nn.LayerNorm(d_model),
         )
 
-        # apply SAITS loss function to ETSformer on the imputation task
+        # for the imputation task, the output dim is the same as input dim
+        self.output_projection = nn.Linear(d_model, n_features)
+
         self.saits_loss_func = SaitsLoss(ORT_weight, MIT_weight)
 
     def forward(self, inputs: dict, training: bool = True) -> dict:
         X, missing_mask = inputs["X"], inputs["missing_mask"]
 
-        # WDU: the original ETSformer paper isn't proposed for imputation task. Hence the model doesn't take
+        # WDU: the original Informer paper isn't proposed for imputation task. Hence the model doesn't take
         # the missing mask into account, which means, in the process, the model doesn't know which part of
-        # the input data is missing, and this may hurt the model's imputation performance. Therefore, I add the
-        # embedding layers to project the concatenation of features and masks into a hidden space, as well as
+        # the input data is missing, and this may hurt the model's imputation performance. Therefore, I apply the
+        # SAITS embedding method to project the concatenation of features and masks into a hidden space, as well as
         # the output layers to project back from the hidden space to the original space.
+        enc_out = self.saits_embedding(X, missing_mask)
+
+        # Informer encoder processing
+        enc_out, attns = self.encoder(enc_out)
 
-        # the same as SAITS, concatenate the time series data and the missing mask for embedding
-        input_X = torch.cat([X, missing_mask], dim=2)
-        res = self.enc_embedding(input_X)
-
-        # ETSformer encoder processing
-        level, growths, seasons = self.encoder(res, X, attn_mask=None)
-        growth, season = self.decoder(growths, seasons)
-        reconstruction = level[:, -1:] + growth + season
+        # project back the original data space
+        reconstruction = self.output_projection(enc_out)
 
         imputed_data = missing_mask * X + (1 - missing_mask) * reconstruction
         results = {
             "imputed_data": imputed_data,
         }
 
         # if in training mode, return results with losses
```

### Comparing `pypots-0.4.1/pypots/imputation/etsformer/data.py` & `pypots-0.5/pypots/imputation/etsformer/data.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Dataset class for ETSformer.
+Dataset class for the imputation model ETSformer.
 """
 
 # Created by Wenjie Du <wenjay.du@gmail.com>
 # License: BSD-3-Clause
 
 from typing import Union
 
@@ -13,12 +13,12 @@
 class DatasetForETSformer(DatasetForSAITS):
     """Actually ETSformer uses the same data strategy as SAITS, needs MIT for training."""
 
     def __init__(
         self,
         data: Union[dict, str],
         return_X_ori: bool,
-        return_labels: bool,
-        file_type: str = "h5py",
+        return_y: bool,
+        file_type: str = "hdf5",
         rate: float = 0.2,
     ):
-        super().__init__(data, return_X_ori, return_labels, file_type, rate)
+        super().__init__(data, return_X_ori, return_y, file_type, rate)
```

### Comparing `pypots-0.4.1/pypots/imputation/etsformer/model.py` & `pypots-0.5/pypots/imputation/informer/model.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,68 +1,56 @@
 """
-The implementation of ETSformer for the partially-observed time-series imputation task.
-
-Refer to the paper "Gerald Woo, Chenghao Liu, Doyen Sahoo, Akshat Kumar, and Steven Hoi.
-ETSformer: Exponential smoothing transformers for time-series forecasting.
-In ICLR, 2023."
-
-Notes
------
-Partial implementation uses code from https://github.com/salesforce/ETSformer
+The implementation of Informer for the partially-observed time-series imputation task.
 
 """
 
 # Created by Wenjie Du <wenjay.du@gmail.com>
 # License: BSD-3-Clause
 
 from typing import Union, Optional
 
 import numpy as np
 import torch
 from torch.utils.data import DataLoader
 
-from .data import DatasetForETSformer
-from pypots.imputation.etsformer.core import _ETSformer
+from .core import _Informer
+from .data import DatasetForInformer
 from ..base import BaseNNImputer
-from ...data.base import BaseDataset
-from ...data.checking import check_X_ori_in_val_set
+from ...data.checking import key_in_data_set
+from ...data.dataset import BaseDataset
 from ...optim.adam import Adam
 from ...optim.base import Optimizer
-from ...utils.logging import logger
 
 
-class ETSformer(BaseNNImputer):
-    """The PyTorch implementation of the ETSformer model.
-    ETSformer is originally proposed by Woo et al. in :cite:`woo2023etsformer`.
+class Informer(BaseNNImputer):
+    """The PyTorch implementation of the Informer model.
+    Informer is originally proposed by Wu et al. in :cite:`zhou2021informer`.
 
     Parameters
     ----------
     n_steps :
         The number of time steps in the time-series data sample.
 
     n_features :
         The number of features in the time-series data sample.
 
-    n_e_layers :
-        The number of layers in the ETSformer encoder.
-
-    n_d_layers :
-        The number of layers in the ETSformer decoder.
-
-    n_heads :
-        The number of heads in each layer of ETSformer.
+    n_layers :
+        The number of layers in the Informer model.
 
     d_model :
         The dimension of the model.
 
+    n_heads :
+        The number of heads in each layer of Informer.
+
     d_ffn :
         The dimension of the feed-forward network.
 
-    top_k :
-        Top-K Fourier bases.
+    factor :
+        The factor of the ProbSparse self-attention mechanism for the Informer model.
 
     dropout :
         The dropout rate for the model.
 
     ORT_weight :
         The weight for the ORT loss, the same as SAITS.
 
@@ -108,22 +96,21 @@
         better than in previous epochs.
         The "all" strategy will save every model after each epoch training.
 
     """
 
     def __init__(
         self,
-        n_steps,
-        n_features,
-        n_e_layers,
-        n_d_layers,
-        n_heads,
-        d_model,
-        d_ffn,
-        top_k,
+        n_steps: int,
+        n_features: int,
+        n_layers: int,
+        d_model: int,
+        n_heads: int,
+        d_ffn: int,
+        factor: int,
         dropout: float = 0,
         ORT_weight: float = 1,
         MIT_weight: float = 1,
         batch_size: int = 32,
         epochs: int = 100,
         patience: int = None,
         optimizer: Optional[Optimizer] = Adam(),
@@ -142,34 +129,32 @@
             model_saving_strategy,
         )
 
         self.n_steps = n_steps
         self.n_features = n_features
         # model hype-parameters
         self.n_heads = n_heads
-        self.n_e_layers = n_e_layers
-        self.n_d_layers = n_d_layers
+        self.n_layers = n_layers
         self.d_model = d_model
         self.d_ffn = d_ffn
+        self.factor = factor
         self.dropout = dropout
-        self.top_k = top_k
         self.ORT_weight = ORT_weight
         self.MIT_weight = MIT_weight
 
         # set up the model
-        self.model = _ETSformer(
+        self.model = _Informer(
             self.n_steps,
             self.n_features,
-            self.n_e_layers,
-            self.n_d_layers,
-            self.n_heads,
+            self.n_layers,
             self.d_model,
+            self.n_heads,
             self.d_ffn,
+            self.factor,
             self.dropout,
-            self.top_k,
             self.ORT_weight,
             self.MIT_weight,
         )
         self._send_model_to_given_device()
         self._print_model_size()
 
         # set up the optimizer
@@ -207,32 +192,32 @@
 
         return inputs
 
     def fit(
         self,
         train_set: Union[dict, str],
         val_set: Optional[Union[dict, str]] = None,
-        file_type: str = "h5py",
+        file_type: str = "hdf5",
     ) -> None:
         # Step 1: wrap the input data with classes Dataset and DataLoader
-        training_set = DatasetForETSformer(
-            train_set, return_X_ori=False, return_labels=False, file_type=file_type
+        training_set = DatasetForInformer(
+            train_set, return_X_ori=False, return_y=False, file_type=file_type
         )
         training_loader = DataLoader(
             training_set,
             batch_size=self.batch_size,
             shuffle=True,
             num_workers=self.num_workers,
         )
         val_loader = None
         if val_set is not None:
-            if not check_X_ori_in_val_set(val_set):
+            if not key_in_data_set("X_ori", val_set):
                 raise ValueError("val_set must contain 'X_ori' for model validation.")
-            val_set = DatasetForETSformer(
-                val_set, return_X_ori=True, return_labels=False, file_type=file_type
+            val_set = DatasetForInformer(
+                val_set, return_X_ori=True, return_y=False, file_type=file_type
             )
             val_loader = DataLoader(
                 val_set,
                 batch_size=self.batch_size,
                 shuffle=False,
                 num_workers=self.num_workers,
             )
@@ -244,42 +229,46 @@
 
         # Step 3: save the model if necessary
         self._auto_save_model_if_necessary(confirm_saving=True)
 
     def predict(
         self,
         test_set: Union[dict, str],
-        file_type: str = "h5py",
+        file_type: str = "hdf5",
     ) -> dict:
         """Make predictions for the input data with the trained model.
 
         Parameters
         ----------
         test_set : dict or str
             The dataset for model validating, should be a dictionary including keys as 'X',
             or a path string locating a data file supported by PyPOTS (e.g. h5 file).
-            If it is a dict, X should be array-like of shape [n_samples, sequence length (time steps), n_features],
+            If it is a dict, X should be array-like of shape [n_samples, sequence length (n_steps), n_features],
             which is time-series data for validating, can contain missing values, and y should be array-like of shape
             [n_samples], which is classification labels of X.
             If it is a path string, the path should point to a data file, e.g. a h5 file, which contains
             key-value pairs like a dict, and it has to include keys as 'X' and 'y'.
 
-        file_type : str
+        file_type :
             The type of the given file if test_set is a path string.
 
         Returns
         -------
-        result_dict : dict,
+        file_type :
             The dictionary containing the clustering results and latent variables if necessary.
 
         """
         # Step 1: wrap the input data with classes Dataset and DataLoader
         self.model.eval()  # set the model as eval status to freeze it.
         test_set = BaseDataset(
-            test_set, return_X_ori=False, return_labels=False, file_type=file_type
+            test_set,
+            return_X_ori=False,
+            return_X_pred=False,
+            return_y=False,
+            file_type=file_type,
         )
         test_loader = DataLoader(
             test_set,
             batch_size=self.batch_size,
             shuffle=False,
             num_workers=self.num_workers,
         )
@@ -297,36 +286,29 @@
         result_dict = {
             "imputation": imputation,
         }
         return result_dict
 
     def impute(
         self,
-        X: Union[dict, str],
-        file_type="h5py",
+        test_set: Union[dict, str],
+        file_type: str = "hdf5",
     ) -> np.ndarray:
         """Impute missing values in the given data with the trained model.
 
-        Warnings
-        --------
-        The method impute is deprecated. Please use `predict()` instead.
-
         Parameters
         ----------
-        X :
-            The data samples for testing, should be array-like of shape [n_samples, sequence length (time steps),
+        test_set :
+            The data samples for testing, should be array-like of shape [n_samples, sequence length (n_steps),
             n_features], or a path string locating a data file, e.g. h5 file.
 
         file_type :
             The type of the given file if X is a path string.
 
         Returns
         -------
-        array-like, shape [n_samples, sequence length (time steps), n_features],
+        array-like, shape [n_samples, sequence length (n_steps), n_features],
             Imputed data.
         """
-        logger.warning(
-            "🚨DeprecationWarning: The method impute is deprecated. Please use `predict` instead."
-        )
 
-        results_dict = self.predict(X, file_type=file_type)
-        return results_dict["imputation"]
+        result_dict = self.predict(test_set, file_type=file_type)
+        return result_dict["imputation"]
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pypots-0.4.1/pypots/imputation/fedformer/__init__.py` & `pypots-0.5/pypots/imputation/fedformer/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,14 +3,18 @@
 
 Refer to the paper
 `Tian Zhou, Ziqing Ma, Qingsong Wen, Xue Wang, Liang Sun, and Rong Jin.
 FEDformer: Frequency enhanced decomposed transformer for long-term series forecasting.
 In ICML, volume 162 of Proceedings of Machine Learning Research, pages 27268–27286. PMLR, 17–23 Jul 2022.
 <https://proceedings.mlr.press/v162/zhou22g/zhou22g.pdf>`_
 
+Notes
+-----
+This implementation is inspired by the official one https://github.com/MAZiqing/FEDformer
+
 """
 
 # Created by Wenjie Du <wenjay.du@gmail.com>
 # License: BSD-3-Clause
 
 
 from .model import FEDformer
```

### Comparing `pypots-0.4.1/pypots/imputation/fedformer/core.py` & `pypots-0.5/pypots/imputation/fedformer/core.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,53 +1,54 @@
 """
-
+The core wrapper assembles the submodules of FEDformer imputation model
+and takes over the forward progress of the algorithm.
 """
 
 # Created by Wenjie Du <wenjay.du@gmail.com>
 # License: BSD-3-Clause
 
-import torch
 import torch.nn as nn
 
 from ...nn.modules.fedformer import FEDformerEncoder
-from ...nn.modules.saits import SaitsLoss
-from ...nn.modules.transformer.embedding import DataEmbedding
+from ...nn.modules.saits import SaitsLoss, SaitsEmbedding
 
 
 class _FEDformer(nn.Module):
     def __init__(
         self,
         n_steps,
         n_features,
         n_layers,
-        n_heads,
         d_model,
+        n_heads,
         d_ffn,
         moving_avg_window_size,
         dropout,
         version="Fourier",
         modes=32,
         mode_select="random",
         ORT_weight: float = 1,
         MIT_weight: float = 1,
         activation="relu",
     ):
         super().__init__()
 
-        self.enc_embedding = DataEmbedding(
+        self.saits_embedding = SaitsEmbedding(
             n_features * 2,
             d_model,
+            with_pos=True,
+            n_max_steps=n_steps,
             dropout=dropout,
         )
 
         self.encoder = FEDformerEncoder(
             n_steps,
             n_layers,
-            n_heads,
             d_model,
+            n_heads,
             d_ffn,
             moving_avg_window_size,
             dropout,
             version,
             modes,
             mode_select,
             activation,
@@ -58,21 +59,18 @@
         self.saits_loss_func = SaitsLoss(ORT_weight, MIT_weight)
 
     def forward(self, inputs: dict, training: bool = True) -> dict:
         X, missing_mask = inputs["X"], inputs["missing_mask"]
 
         # WDU: the original FEDformer paper isn't proposed for imputation task. Hence the model doesn't take
         # the missing mask into account, which means, in the process, the model doesn't know which part of
-        # the input data is missing, and this may hurt the model's imputation performance. Therefore, I add the
-        # embedding layers to project the concatenation of features and masks into a hidden space, as well as
+        # the input data is missing, and this may hurt the model's imputation performance. Therefore, I apply the
+        # SAITS embedding method to project the concatenation of features and masks into a hidden space, as well as
         # the output layers to project back from the hidden space to the original space.
-
-        # the same as SAITS, concatenate the time series data and the missing mask for embedding
-        input_X = torch.cat([X, missing_mask], dim=2)
-        enc_out = self.enc_embedding(input_X)
+        enc_out = self.saits_embedding(X, missing_mask)
 
         # FEDformer encoder processing
         enc_out, attns = self.encoder(enc_out)
         reconstruction = self.output_projection(enc_out)
 
         imputed_data = missing_mask * X + (1 - missing_mask) * reconstruction
         results = {
```

### Comparing `pypots-0.4.1/pypots/imputation/fedformer/data.py` & `pypots-0.5/pypots/imputation/fedformer/data.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Dataset class for FEDformer.
+Dataset class for the imputation model FEDformer.
 """
 
 # Created by Wenjie Du <wenjay.du@gmail.com>
 # License: BSD-3-Clause
 
 from typing import Union
 
@@ -13,12 +13,12 @@
 class DatasetForFEDformer(DatasetForSAITS):
     """Actually FEDformer uses the same data strategy as SAITS, needs MIT for training."""
 
     def __init__(
         self,
         data: Union[dict, str],
         return_X_ori: bool,
-        return_labels: bool,
-        file_type: str = "h5py",
+        return_y: bool,
+        file_type: str = "hdf5",
         rate: float = 0.2,
     ):
-        super().__init__(data, return_X_ori, return_labels, file_type, rate)
+        super().__init__(data, return_X_ori, return_y, file_type, rate)
```

### Comparing `pypots-0.4.1/pypots/imputation/fedformer/model.py` & `pypots-0.5/pypots/imputation/etsformer/model.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,80 +1,63 @@
 """
-The implementation of FEDformer for the partially-observed time-series imputation task.
-
-Refer to the paper "Tian Zhou, Ziqing Ma, Qingsong Wen, Xue Wang, Liang Sun, and Rong Jin.
-FEDformer: Frequency enhanced decomposed transformer for long-term series forecasting.
-In ICML, volume 162 of Proceedings of Machine Learning Research, pages 27268–27286. PMLR, 17–23 Jul 2022.".
-
-Notes
------
-Partial implementation uses code from https://github.com/MAZiqing/FEDformer
+The implementation of ETSformer for the partially-observed time-series imputation task.
 
 """
 
 # Created by Wenjie Du <wenjay.du@gmail.com>
 # License: BSD-3-Clause
 
 from typing import Union, Optional
 
 import numpy as np
 import torch
 from torch.utils.data import DataLoader
 
-from .core import _FEDformer
-from .data import DatasetForFEDformer
+from .core import _ETSformer
+from .data import DatasetForETSformer
 from ..base import BaseNNImputer
-from ...data.base import BaseDataset
-from ...data.checking import check_X_ori_in_val_set
+from ...data.checking import key_in_data_set
+from ...data.dataset import BaseDataset
 from ...optim.adam import Adam
 from ...optim.base import Optimizer
-from ...utils.logging import logger
 
 
-class FEDformer(BaseNNImputer):
-    """The PyTorch implementation of the FEDformer model.
-    FEDformer is originally proposed by Woo et al. in :cite:`zhou2022fedformer`.
+class ETSformer(BaseNNImputer):
+    """The PyTorch implementation of the ETSformer model.
+    ETSformer is originally proposed by Woo et al. in :cite:`woo2023etsformer`.
 
     Parameters
     ----------
     n_steps :
         The number of time steps in the time-series data sample.
 
     n_features :
         The number of features in the time-series data sample.
 
-    n_layers :
-        The number of layers in the FEDformer.
+    n_e_layers :
+        The number of layers in the ETSformer encoder.
 
-    n_heads :
-        The number of heads in the multi-head attention mechanism.
+    n_d_layers :
+        The number of layers in the ETSformer decoder.
 
     d_model :
         The dimension of the model.
 
+    n_heads :
+        The number of heads in each layer of ETSformer.
+
     d_ffn :
         The dimension of the feed-forward network.
 
-    moving_avg_window_size :
-        The window size of moving average.
+    top_k :
+        Top-K Fourier bases.
 
     dropout :
         The dropout rate for the model.
 
-    version :
-        The version of the model. It has to be one of ["Wavelets", "Fourier"].
-        The default value is "Fourier".
-
-    modes :
-        The number of modes to be selected. The default value is 32.
-
-    mode_select :
-        Get modes on frequency domain. It has to "random" or "low". The default value is "random".
-        'random' means sampling randomly; 'low' means sampling the lowest modes;
-
     ORT_weight :
         The weight for the ORT loss, the same as SAITS.
 
     MIT_weight :
         The weight for the MIT loss, the same as SAITS.
 
     batch_size :
@@ -118,23 +101,21 @@
 
     """
 
     def __init__(
         self,
         n_steps,
         n_features,
-        n_layers,
-        n_heads,
+        n_e_layers,
+        n_d_layers,
         d_model,
+        n_heads,
         d_ffn,
-        moving_avg_window_size,
+        top_k,
         dropout: float = 0,
-        version="Fourier",
-        modes=32,
-        mode_select="random",
         ORT_weight: float = 1,
         MIT_weight: float = 1,
         batch_size: int = 32,
         epochs: int = 100,
         patience: int = None,
         optimizer: Optional[Optimizer] = Adam(),
         num_workers: int = 0,
@@ -151,39 +132,35 @@
             saving_path,
             model_saving_strategy,
         )
 
         self.n_steps = n_steps
         self.n_features = n_features
         # model hype-parameters
-        self.n_layers = n_layers
         self.n_heads = n_heads
+        self.n_e_layers = n_e_layers
+        self.n_d_layers = n_d_layers
         self.d_model = d_model
         self.d_ffn = d_ffn
-        self.moving_avg_window_size = moving_avg_window_size
         self.dropout = dropout
-        self.version = version
-        self.modes = modes
-        self.mode_select = mode_select
+        self.top_k = top_k
         self.ORT_weight = ORT_weight
         self.MIT_weight = MIT_weight
 
         # set up the model
-        self.model = _FEDformer(
+        self.model = _ETSformer(
             self.n_steps,
             self.n_features,
-            self.n_layers,
-            self.n_heads,
+            self.n_e_layers,
+            self.n_d_layers,
             self.d_model,
+            self.n_heads,
             self.d_ffn,
-            self.moving_avg_window_size,
             self.dropout,
-            self.version,
-            self.modes,
-            self.mode_select,
+            self.top_k,
             self.ORT_weight,
             self.MIT_weight,
         )
         self._send_model_to_given_device()
         self._print_model_size()
 
         # set up the optimizer
@@ -221,32 +198,32 @@
 
         return inputs
 
     def fit(
         self,
         train_set: Union[dict, str],
         val_set: Optional[Union[dict, str]] = None,
-        file_type: str = "h5py",
+        file_type: str = "hdf5",
     ) -> None:
         # Step 1: wrap the input data with classes Dataset and DataLoader
-        training_set = DatasetForFEDformer(
-            train_set, return_X_ori=False, return_labels=False, file_type=file_type
+        training_set = DatasetForETSformer(
+            train_set, return_X_ori=False, return_y=False, file_type=file_type
         )
         training_loader = DataLoader(
             training_set,
             batch_size=self.batch_size,
             shuffle=True,
             num_workers=self.num_workers,
         )
         val_loader = None
         if val_set is not None:
-            if not check_X_ori_in_val_set(val_set):
+            if not key_in_data_set("X_ori", val_set):
                 raise ValueError("val_set must contain 'X_ori' for model validation.")
-            val_set = DatasetForFEDformer(
-                val_set, return_X_ori=True, return_labels=False, file_type=file_type
+            val_set = DatasetForETSformer(
+                val_set, return_X_ori=True, return_y=False, file_type=file_type
             )
             val_loader = DataLoader(
                 val_set,
                 batch_size=self.batch_size,
                 shuffle=False,
                 num_workers=self.num_workers,
             )
@@ -258,42 +235,46 @@
 
         # Step 3: save the model if necessary
         self._auto_save_model_if_necessary(confirm_saving=True)
 
     def predict(
         self,
         test_set: Union[dict, str],
-        file_type: str = "h5py",
+        file_type: str = "hdf5",
     ) -> dict:
         """Make predictions for the input data with the trained model.
 
         Parameters
         ----------
         test_set : dict or str
             The dataset for model validating, should be a dictionary including keys as 'X',
             or a path string locating a data file supported by PyPOTS (e.g. h5 file).
-            If it is a dict, X should be array-like of shape [n_samples, sequence length (time steps), n_features],
+            If it is a dict, X should be array-like of shape [n_samples, sequence length (n_steps), n_features],
             which is time-series data for validating, can contain missing values, and y should be array-like of shape
             [n_samples], which is classification labels of X.
             If it is a path string, the path should point to a data file, e.g. a h5 file, which contains
             key-value pairs like a dict, and it has to include keys as 'X' and 'y'.
 
-        file_type : str
+        file_type :
             The type of the given file if test_set is a path string.
 
         Returns
         -------
-        result_dict : dict,
+        file_type :
             The dictionary containing the clustering results and latent variables if necessary.
 
         """
         # Step 1: wrap the input data with classes Dataset and DataLoader
         self.model.eval()  # set the model as eval status to freeze it.
         test_set = BaseDataset(
-            test_set, return_X_ori=False, return_labels=False, file_type=file_type
+            test_set,
+            return_X_ori=False,
+            return_X_pred=False,
+            return_y=False,
+            file_type=file_type,
         )
         test_loader = DataLoader(
             test_set,
             batch_size=self.batch_size,
             shuffle=False,
             num_workers=self.num_workers,
         )
@@ -311,36 +292,29 @@
         result_dict = {
             "imputation": imputation,
         }
         return result_dict
 
     def impute(
         self,
-        X: Union[dict, str],
-        file_type="h5py",
+        test_set: Union[dict, str],
+        file_type: str = "hdf5",
     ) -> np.ndarray:
         """Impute missing values in the given data with the trained model.
 
-        Warnings
-        --------
-        The method impute is deprecated. Please use `predict()` instead.
-
         Parameters
         ----------
-        X :
-            The data samples for testing, should be array-like of shape [n_samples, sequence length (time steps),
+        test_set :
+            The data samples for testing, should be array-like of shape [n_samples, sequence length (n_steps),
             n_features], or a path string locating a data file, e.g. h5 file.
 
         file_type :
             The type of the given file if X is a path string.
 
         Returns
         -------
-        array-like, shape [n_samples, sequence length (time steps), n_features],
+        array-like, shape [n_samples, sequence length (n_steps), n_features],
             Imputed data.
         """
-        logger.warning(
-            "🚨DeprecationWarning: The method impute is deprecated. Please use `predict` instead."
-        )
 
-        results_dict = self.predict(X, file_type=file_type)
-        return results_dict["imputation"]
+        result_dict = self.predict(test_set, file_type=file_type)
+        return result_dict["imputation"]
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pypots-0.4.1/pypots/imputation/gpvae/__init__.py` & `pypots-0.5/pypots/imputation/gpvae/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,14 +3,18 @@
 
 Refer to the paper
 `Vincent Fortuin, Dmitry Baranchuk, Gunnar Rätsch, and Stephan Mandt.
 GP-VAE: Deep probabilistic time series imputation.
 In International conference on artificial intelligence and statistics, pages 1651–1661. PMLR, 2020.
 <http://proceedings.mlr.press/v108/fortuin20a/fortuin20a.pdf>`_
 
+Notes
+-----
+This implementation is inspired by the official one https://github.com/ratschlab/GP-VAE
+
 """
 
 # Created by Jun Wang <jwangfx@connect.ust.hk>
 # License: BSD-3-Clause
 
 from .model import GPVAE
```

### Comparing `pypots-0.4.1/pypots/imputation/gpvae/core.py` & `pypots-0.5/pypots/imputation/gpvae/core.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 """
-The implementation of GP-VAE for the partially-observed time-series imputation task.
-
-Refer to the paper Fortuin V, Baranchuk D, Rätsch G, et al.
-GP-VAE: Deep probabilistic time series imputation. AISTATS. PMLR, 2020: 1651-1661.
+The core wrapper assembles the submodules of GP-VAE imputation model
+and takes over the forward progress of the algorithm.
 
 """
 
 # Created by Jun Wang <jwangfx@connect.ust.hk> and Wenjie Du <wenjay.du@gmail.com>
 # License: BSD-3-Clause
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pypots-0.4.1/pypots/imputation/gpvae/data.py` & `pypots-0.5/pypots/imputation/gpvae/data.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,68 +1,74 @@
 """
-Dataset class for model GP-VAE.
+Dataset class for the imputation model GP-VAE.
 """
 
 # Created by Jun Wang <jwangfx@connect.ust.hk> and Wenjie Du <wenjay.du@gmail.com>
 # License: BSD-3-Clause
 
 from typing import Union, Iterable
 
 import torch
 from pygrinder import fill_and_get_mask_torch
-from ...data.base import BaseDataset
+from ...data.dataset import BaseDataset
 
 
 class DatasetForGPVAE(BaseDataset):
     """Dataset class for GP-VAE.
 
     Parameters
     ----------
-    data : dict or str,
+    data :
         The dataset for model input, should be a dictionary including keys as 'X' and 'y',
         or a path string locating a data file.
-        If it is a dict, X should be array-like of shape [n_samples, sequence length (time steps), n_features],
+        If it is a dict, X should be array-like of shape [n_samples, sequence length (n_steps), n_features],
         which is time-series data for input, can contain missing values, and y should be array-like of shape
         [n_samples], which is classification labels of X.
         If it is a path string, the path should point to a data file, e.g. a h5 file, which contains
         key-value pairs like a dict, and it has to include keys as 'X' and 'y'.
 
-    return_labels : bool, default = True,
+    return_y :
         Whether to return labels in function __getitem__() if they exist in the given data. If `True`, for example,
         during training of classification models, the Dataset class will return labels in __getitem__() for model input.
         Otherwise, labels won't be included in the data returned by __getitem__(). This parameter exists because we
         need the defined Dataset class for all training/validating/testing stages. For those big datasets stored in h5
         files, they already have both X and y saved. But we don't read labels from the file for validating and testing
         with function _fetch_data_from_file(), which works for all three stages. Therefore, we need this parameter for
         distinction.
 
-    file_type : str, default = "h5py"
+    file_type :
         The type of the given file if train_set and val_set are path strings.
     """
 
     def __init__(
         self,
         data: Union[dict, str],
         return_X_ori: bool,
-        return_labels: bool,
-        file_type: str = "h5py",
+        return_y: bool,
+        file_type: str = "hdf5",
     ):
-        super().__init__(data, return_X_ori, return_labels, file_type)
+        super().__init__(
+            data=data,
+            return_X_ori=return_X_ori,
+            return_X_pred=False,
+            return_y=return_y,
+            file_type=file_type,
+        )
 
     def _fetch_data_from_array(self, idx: int) -> Iterable:
         """Fetch data from self.X if it is given.
 
         Parameters
         ----------
-        idx : int,
+        idx :
             The index of the sample to be return.
 
         Returns
         -------
-        sample : list,
+        sample :
             A list contains
 
             index : int tensor,
                 The index of the sample.
 
             X : tensor,
                 The feature vector for model input.
@@ -74,57 +80,57 @@
                 The delta matrix contains time gaps of missing values.
 
             label (optional) : tensor,
                 The target label of the time-series sample.
         """
         X = self.X[idx]
 
-        if self.X_ori is not None and self.return_X_ori:
+        if self.return_X_ori:
             X = self.X[idx]
             missing_mask = self.missing_mask[idx]
             X_ori = self.X_ori[idx]
             indicating_mask = self.indicating_mask[idx]
             sample = [torch.tensor(idx), X, missing_mask, X_ori, indicating_mask]
         else:
             X, missing_mask = fill_and_get_mask_torch(X)
             sample = [torch.tensor(idx), X, missing_mask]
 
-        if self.y is not None and self.return_labels:
+        if self.return_y:
             sample.append(self.y[idx].to(torch.long))
 
         return sample
 
     def _fetch_data_from_file(self, idx: int) -> Iterable:
         """Fetch data with the lazy-loading strategy, i.e. only loading data from the file while requesting for samples.
         Here the opened file handle doesn't load the entire dataset into RAM but only load the currently accessed slice.
 
         Parameters
         ----------
-        idx : int,
+        idx :
             The index of the sample to be return.
 
         Returns
         -------
-        sample : list,
+        sample :
             The collated data sample, a list including all necessary sample info.
         """
 
         if self.file_handle is None:
             self.file_handle = self._open_file_handle()
 
-        if "X_ori" in self.file_handle.keys() and self.return_X_ori:
+        if self.return_X_ori:
             X = torch.from_numpy(self.file_handle["X"][idx]).to(torch.float32)
             X_ori = torch.from_numpy(self.file_handle["X_ori"][idx]).to(torch.float32)
             X_ori, X_ori_missing_mask = fill_and_get_mask_torch(X_ori)
             X, missing_mask = fill_and_get_mask_torch(X)
             indicating_mask = (X_ori_missing_mask - missing_mask).to(torch.float32)
             sample = [torch.tensor(idx), X, missing_mask, X_ori, indicating_mask]
         else:
             X = torch.from_numpy(self.file_handle["X"][idx]).to(torch.float32)
             X, missing_mask = fill_and_get_mask_torch(X)
             sample = [torch.tensor(idx), X, missing_mask]
 
         # if the dataset has labels and is for training, then fetch it from the file
-        if "y" in self.file_handle.keys() and self.return_labels:
+        if self.return_y:
             sample.append(torch.tensor(self.file_handle["y"][idx], dtype=torch.long))
 
         return sample
```

### Comparing `pypots-0.4.1/pypots/imputation/gpvae/model.py` & `pypots-0.5/pypots/imputation/gpvae/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,10 @@
 """
 The implementation of GP-VAE for the partially-observed time-series imputation task.
 
-Refer to the paper "Vincent Fortuin, Dmitry Baranchuk, Gunnar Rätsch, and Stephan Mandt.
-GP-VAE: Deep probabilistic time series imputation.
-In International conference on artificial intelligence and statistics, pages 1651–1661. PMLR, 2020."
-
 """
 
 # Created by Jun Wang <jwangfx@connect.ust.hk> and Wenjie Du <wenjay.du@gmail.com>
 # License: BSD-3-Clause
 
 
 import os
@@ -23,15 +19,15 @@
 except ImportError:
     pass
 
 
 from .core import _GPVAE
 from .data import DatasetForGPVAE
 from ..base import BaseNNImputer
-from ...data.checking import check_X_ori_in_val_set
+from ...data.checking import key_in_data_set
 from ...optim.adam import Adam
 from ...optim.base import Optimizer
 from ...utils.logging import logger
 from ...utils.metrics import calc_mse
 
 
 class GPVAE(BaseNNImputer):
@@ -357,32 +353,32 @@
             f"Finished training. The best model is from epoch#{self.best_epoch}."
         )
 
     def fit(
         self,
         train_set: Union[dict, str],
         val_set: Optional[Union[dict, str]] = None,
-        file_type: str = "h5py",
+        file_type: str = "hdf5",
     ) -> None:
         # Step 1: wrap the input data with classes Dataset and DataLoader
         training_set = DatasetForGPVAE(
-            train_set, return_X_ori=False, return_labels=False, file_type=file_type
+            train_set, return_X_ori=False, return_y=False, file_type=file_type
         )
         training_loader = DataLoader(
             training_set,
             batch_size=self.batch_size,
             shuffle=True,
             num_workers=self.num_workers,
         )
         val_loader = None
         if val_set is not None:
-            if not check_X_ori_in_val_set(val_set):
+            if not key_in_data_set("X_ori", val_set):
                 raise ValueError("val_set must contain 'X_ori' for model validation.")
             val_set = DatasetForGPVAE(
-                val_set, return_X_ori=True, return_labels=False, file_type=file_type
+                val_set, return_X_ori=True, return_y=False, file_type=file_type
             )
             val_loader = DataLoader(
                 val_set,
                 batch_size=self.batch_size,
                 shuffle=False,
                 num_workers=self.num_workers,
             )
@@ -394,31 +390,31 @@
 
         # Step 3: save the model if necessary
         self._auto_save_model_if_necessary(confirm_saving=True)
 
     def predict(
         self,
         test_set: Union[dict, str],
-        file_type: str = "h5py",
+        file_type: str = "hdf5",
         n_sampling_times: int = 1,
     ) -> dict:
         """
 
         Parameters
         ----------
         test_set : dict or str
             The dataset for model validating, should be a dictionary including keys as 'X' and 'y',
             or a path string locating a data file.
-            If it is a dict, X should be array-like of shape [n_samples, sequence length (time steps), n_features],
+            If it is a dict, X should be array-like of shape [n_samples, sequence length (n_steps), n_features],
             which is time-series data for validating, can contain missing values, and y should be array-like of shape
             [n_samples], which is classification labels of X.
             If it is a path string, the path should point to a data file, e.g. a h5 file, which contains
             key-value pairs like a dict, and it has to include keys as 'X' and 'y'.
 
-        file_type : str
+        file_type :
             The type of the given file if test_set is a path string.
 
         n_sampling_times:
             The number of sampling times for the model to produce predictions.
 
         Returns
         -------
@@ -427,15 +423,15 @@
             It should be a dictionary including a key named 'imputation'.
 
         """
         assert n_sampling_times > 0, "n_sampling_times should be greater than 0."
 
         self.model.eval()  # set the model as eval status to freeze it.
         test_set = DatasetForGPVAE(
-            test_set, return_X_ori=False, return_labels=False, file_type=file_type
+            test_set, return_X_ori=False, return_y=False, file_type=file_type
         )
         test_loader = DataLoader(
             test_set,
             batch_size=self.batch_size,
             shuffle=False,
             num_workers=self.num_workers,
         )
@@ -454,38 +450,29 @@
         result_dict = {
             "imputation": imputation,
         }
         return result_dict
 
     def impute(
         self,
-        X: Union[dict, str],
-        file_type="h5py",
-        n_sampling_times: int = 1,
+        test_set: Union[dict, str],
+        file_type: str = "hdf5",
     ) -> np.ndarray:
         """Impute missing values in the given data with the trained model.
 
-        Warnings
-        --------
-        The method impute is deprecated. Please use `predict()` instead.
-
         Parameters
         ----------
-        X :
-            The data samples for testing, should be array-like of shape [n_samples, sequence length (time steps),
+        test_set :
+            The data samples for testing, should be array-like of shape [n_samples, sequence length (n_steps),
             n_features], or a path string locating a data file, e.g. h5 file.
 
         file_type :
             The type of the given file if X is a path string.
 
         Returns
         -------
-        array-like, shape [n_samples, sequence length (time steps), n_features],
+        array-like, shape [n_samples, sequence length (n_steps), n_features],
             Imputed data.
         """
-        logger.warning(
-            "🚨DeprecationWarning: The method impute is deprecated. Please use `predict` instead."
-        )
-        results_dict = self.predict(
-            X, file_type=file_type, n_sampling_times=n_sampling_times
-        )
+
+        results_dict = self.predict(test_set, file_type=file_type)
         return results_dict["imputation"]
```

### Comparing `pypots-0.4.1/pypots/imputation/informer/__init__.py` & `pypots-0.5/pypots/imputation/informer/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,14 +3,18 @@
 
 Refer to the paper
 `Haoyi Zhou, Shanghang Zhang, Jieqi Peng, Shuai Zhang, Jianxin Li, Hui Xiong, and Wancai Zhang.
 Informer: Beyond efficient transformer for long sequence time-series forecasting.
 In Proceedings of the AAAI conference on artificial intelligence, volume 35, pages 11106–11115, 2021.
 <https://ojs.aaai.org/index.php/AAAI/article/download/17325/17132>`_
 
+Notes
+-----
+This implementation is inspired by the official one https://github.com/zhouhaoyi/Informer2020
+
 """
 
 # Created by Wenjie Du <wenjay.du@gmail.com>
 # License: BSD-3-Clause
 
 
 from .model import Informer
```

### Comparing `pypots-0.4.1/pypots/imputation/informer/core.py` & `pypots-0.5/pypots/imputation/film/core.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,95 +1,71 @@
 """
-
+The core wrapper assembles the submodules of FiLM imputation model
+and takes over the forward progress of the algorithm.
 """
 
 # Created by Wenjie Du <wenjay.du@gmail.com>
 # License: BSD-3-Clause
 
-import torch
 import torch.nn as nn
 
-from ...nn.modules.informer import (
-    ProbAttention,
-    ConvLayer,
-    InformerEncoderLayer,
-    InformerEncoder,
-)
-from ...nn.modules.saits import SaitsLoss
-from ...nn.modules.transformer import MultiHeadAttention
-from ...nn.modules.transformer.embedding import DataEmbedding
+from ...nn.modules.film import BackboneFiLM
+from ...nn.modules.saits import SaitsLoss, SaitsEmbedding
 
 
-class _Informer(nn.Module):
+class _FiLM(nn.Module):
     def __init__(
         self,
         n_steps,
         n_features,
-        n_layers,
-        n_heads,
+        window_size,
+        multiscale,
+        modes1,
+        ratio,
+        mode_type,
         d_model,
-        d_ffn,
-        factor,
-        dropout,
         ORT_weight: float = 1,
         MIT_weight: float = 1,
-        distil=False,
-        activation="relu",
     ):
         super().__init__()
 
-        self.enc_embedding = DataEmbedding(
+        self.saits_embedding = SaitsEmbedding(
             n_features * 2,
             d_model,
-            dropout=dropout,
+            with_pos=False,
         )
-        self.encoder = InformerEncoder(
-            [
-                InformerEncoderLayer(
-                    MultiHeadAttention(
-                        n_heads,
-                        d_model,
-                        d_model // n_heads,
-                        d_model // n_heads,
-                        ProbAttention(False, factor, dropout),
-                    ),
-                    d_model,
-                    d_ffn,
-                    dropout,
-                    activation,
-                )
-                for _ in range(n_layers)
-            ],
-            [ConvLayer(d_model) for _ in range(n_layers - 1)] if distil else None,
-            norm_layer=nn.LayerNorm(d_model),
+        self.backbone = BackboneFiLM(
+            n_steps,
+            d_model,
+            n_steps,
+            window_size,
+            multiscale,
+            modes1,
+            ratio,
+            mode_type,
         )
 
         # for the imputation task, the output dim is the same as input dim
         self.output_projection = nn.Linear(d_model, n_features)
-
         self.saits_loss_func = SaitsLoss(ORT_weight, MIT_weight)
 
     def forward(self, inputs: dict, training: bool = True) -> dict:
         X, missing_mask = inputs["X"], inputs["missing_mask"]
 
-        # WDU: the original Informer paper isn't proposed for imputation task. Hence the model doesn't take
+        # WDU: the original FiLM paper isn't proposed for imputation task. Hence the model doesn't take
         # the missing mask into account, which means, in the process, the model doesn't know which part of
-        # the input data is missing, and this may hurt the model's imputation performance. Therefore, I add the
-        # embedding layers to project the concatenation of features and masks into a hidden space, as well as
-        # the output layers to project back from the hidden space to the original space.
-
-        # the same as SAITS, concatenate the time series data and the missing mask for embedding
-        input_X = torch.cat([X, missing_mask], dim=2)
-        enc_out = self.enc_embedding(input_X)
-
-        # Informer encoder processing
-        enc_out, attns = self.encoder(enc_out)
-
-        # project back the original data space
-        reconstruction = self.output_projection(enc_out)
+        # the input data is missing, and this may hurt the model's imputation performance. Therefore, I apply the
+        # SAITS embedding method to project the concatenation of features and masks into a hidden space, as well as
+        # the output layers to pro
+        # ject back from the hidden space to the original space.
+        X_embedding = self.saits_embedding(X, missing_mask)
+
+        # FiLM processing
+        backbone_output = self.backbone(X_embedding)
+        reconstruction = self.output_projection(backbone_output)
 
         imputed_data = missing_mask * X + (1 - missing_mask) * reconstruction
         results = {
             "imputed_data": imputed_data,
         }
 
         # if in training mode, return results with losses
```

### Comparing `pypots-0.4.1/pypots/imputation/informer/data.py` & `pypots-0.5/pypots/imputation/informer/data.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Dataset class for Informer.
+Dataset class for the imputation model Informer.
 """
 
 # Created by Wenjie Du <wenjay.du@gmail.com>
 # License: BSD-3-Clause
 
 from typing import Union
 
@@ -13,12 +13,12 @@
 class DatasetForInformer(DatasetForSAITS):
     """Actually Informer uses the same data strategy as SAITS, needs MIT for training."""
 
     def __init__(
         self,
         data: Union[dict, str],
         return_X_ori: bool,
-        return_labels: bool,
-        file_type: str = "h5py",
+        return_y: bool,
+        file_type: str = "hdf5",
         rate: float = 0.2,
     ):
-        super().__init__(data, return_X_ori, return_labels, file_type, rate)
+        super().__init__(data, return_X_ori, return_y, file_type, rate)
```

### Comparing `pypots-0.4.1/pypots/imputation/informer/model.py` & `pypots-0.5/pypots/imputation/timesnet/model.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,75 +1,64 @@
 """
-The implementation of Informer for the partially-observed time-series imputation task.
-
-Refer to the paper "Haoyi Zhou, Shanghang Zhang, Jieqi Peng, Shuai Zhang, Jianxin Li, Hui Xiong, and Wancai Zhang.
-Informer: Beyond efficient transformer for long sequence time-series forecasting.
-In Proceedings of the AAAI conference on artificial intelligence, volume 35, pages 11106–11115, 2021.".
-
-Notes
------
-Partial implementation uses code from
-https://github.com/zhouhaoyi/Informer2020 and https://github.com/thuml/Time-Series-Library
+The implementation of TimesNet for the partially-observed time-series imputation task.
 
 """
 
 # Created by Wenjie Du <wenjay.du@gmail.com>
 # License: BSD-3-Clause
 
 from typing import Union, Optional
 
 import numpy as np
 import torch
 from torch.utils.data import DataLoader
 
-from .core import _Informer
-from .data import DatasetForInformer
+from .core import _TimesNet
+from .data import DatasetForTimesNet
 from ..base import BaseNNImputer
-from ...data.base import BaseDataset
-from ...data.checking import check_X_ori_in_val_set
+from ...data.checking import key_in_data_set
+from ...data.dataset import BaseDataset
 from ...optim.adam import Adam
 from ...optim.base import Optimizer
-from ...utils.logging import logger
 
 
-class Informer(BaseNNImputer):
-    """The PyTorch implementation of the Informer model.
-    Informer is originally proposed by Wu et al. in :cite:`zhou2021informer`.
+class TimesNet(BaseNNImputer):
+    """The PyTorch implementation of the TimesNet model.
+    TimesNet is originally proposed by Wu et al. in :cite:`wu2023timesnet`.
 
     Parameters
     ----------
     n_steps :
         The number of time steps in the time-series data sample.
 
     n_features :
         The number of features in the time-series data sample.
 
     n_layers :
-        The number of layers in the Informer model.
+        The number of layers in the TimesNet model.
 
-    n_heads :
-        The number of heads in each layer of Informer.
+    top_k :
+        The number of top-k amplitude values to be selected to  obtain the most significant frequencies.
 
     d_model :
         The dimension of the model.
 
     d_ffn :
         The dimension of the feed-forward network.
 
-    factor :
-        The factor of the ProbSparse self-attention mechanism for the Informer model.
+    n_kernels :
+        The number of 2D kernels (2D convolutional layers) to use in the submodule InceptionBlockV1.
 
     dropout :
         The dropout rate for the model.
 
-    ORT_weight :
-        The weight for the ORT loss, the same as SAITS.
-
-    MIT_weight :
-        The weight for the MIT loss, the same as SAITS.
+    apply_nonstationary_norm :
+        Whether to apply non-stationary normalization to the input data for TimesNet.
+        Please refer to :cite:`liu2022nonstationary` for details about non-stationary normalization,
+        which is not the idea of the original TimesNet paper. Hence, we make it optional and default not to use here.
 
     batch_size :
         The batch size for training and evaluating the model.
 
     epochs :
         The number of epochs for training the model.
 
@@ -109,21 +98,20 @@
     """
 
     def __init__(
         self,
         n_steps: int,
         n_features: int,
         n_layers: int,
-        n_heads: int,
+        top_k: int,
         d_model: int,
         d_ffn: int,
-        factor: int,
+        n_kernels: int,
         dropout: float = 0,
-        ORT_weight: float = 1,
-        MIT_weight: float = 1,
+        apply_nonstationary_norm: bool = False,
         batch_size: int = 32,
         epochs: int = 100,
         patience: int = None,
         optimizer: Optional[Optimizer] = Adam(),
         num_workers: int = 0,
         device: Optional[Union[str, torch.device, list]] = None,
         saving_path: str = None,
@@ -138,35 +126,33 @@
             saving_path,
             model_saving_strategy,
         )
 
         self.n_steps = n_steps
         self.n_features = n_features
         # model hype-parameters
-        self.n_heads = n_heads
         self.n_layers = n_layers
+        self.top_k = top_k
         self.d_model = d_model
         self.d_ffn = d_ffn
-        self.factor = factor
+        self.n_kernels = n_kernels
         self.dropout = dropout
-        self.ORT_weight = ORT_weight
-        self.MIT_weight = MIT_weight
+        self.apply_nonstationary_norm = apply_nonstationary_norm
 
         # set up the model
-        self.model = _Informer(
+        self.model = _TimesNet(
+            self.n_layers,
             self.n_steps,
             self.n_features,
-            self.n_layers,
-            self.n_heads,
+            self.top_k,
             self.d_model,
             self.d_ffn,
-            self.factor,
+            self.n_kernels,
             self.dropout,
-            self.ORT_weight,
-            self.MIT_weight,
+            self.apply_nonstationary_norm,
         )
         self._send_model_to_given_device()
         self._print_model_size()
 
         # set up the optimizer
         self.optimizer = optimizer
         self.optimizer.init_optimizer(self.model.parameters())
@@ -202,32 +188,32 @@
 
         return inputs
 
     def fit(
         self,
         train_set: Union[dict, str],
         val_set: Optional[Union[dict, str]] = None,
-        file_type: str = "h5py",
+        file_type: str = "hdf5",
     ) -> None:
         # Step 1: wrap the input data with classes Dataset and DataLoader
-        training_set = DatasetForInformer(
-            train_set, return_X_ori=False, return_labels=False, file_type=file_type
+        training_set = DatasetForTimesNet(
+            train_set, return_X_ori=False, return_y=False, file_type=file_type
         )
         training_loader = DataLoader(
             training_set,
             batch_size=self.batch_size,
             shuffle=True,
             num_workers=self.num_workers,
         )
         val_loader = None
         if val_set is not None:
-            if not check_X_ori_in_val_set(val_set):
+            if not key_in_data_set("X_ori", val_set):
                 raise ValueError("val_set must contain 'X_ori' for model validation.")
-            val_set = DatasetForInformer(
-                val_set, return_X_ori=True, return_labels=False, file_type=file_type
+            val_set = DatasetForTimesNet(
+                val_set, return_X_ori=True, return_y=False, file_type=file_type
             )
             val_loader = DataLoader(
                 val_set,
                 batch_size=self.batch_size,
                 shuffle=False,
                 num_workers=self.num_workers,
             )
@@ -239,42 +225,46 @@
 
         # Step 3: save the model if necessary
         self._auto_save_model_if_necessary(confirm_saving=True)
 
     def predict(
         self,
         test_set: Union[dict, str],
-        file_type: str = "h5py",
+        file_type: str = "hdf5",
     ) -> dict:
         """Make predictions for the input data with the trained model.
 
         Parameters
         ----------
         test_set : dict or str
             The dataset for model validating, should be a dictionary including keys as 'X',
             or a path string locating a data file supported by PyPOTS (e.g. h5 file).
-            If it is a dict, X should be array-like of shape [n_samples, sequence length (time steps), n_features],
+            If it is a dict, X should be array-like of shape [n_samples, sequence length (n_steps), n_features],
             which is time-series data for validating, can contain missing values, and y should be array-like of shape
             [n_samples], which is classification labels of X.
             If it is a path string, the path should point to a data file, e.g. a h5 file, which contains
             key-value pairs like a dict, and it has to include keys as 'X' and 'y'.
 
-        file_type : str
+        file_type :
             The type of the given file if test_set is a path string.
 
         Returns
         -------
-        result_dict : dict,
+        file_type :
             The dictionary containing the clustering results and latent variables if necessary.
 
         """
         # Step 1: wrap the input data with classes Dataset and DataLoader
         self.model.eval()  # set the model as eval status to freeze it.
         test_set = BaseDataset(
-            test_set, return_X_ori=False, return_labels=False, file_type=file_type
+            test_set,
+            return_X_ori=False,
+            return_X_pred=False,
+            return_y=False,
+            file_type=file_type,
         )
         test_loader = DataLoader(
             test_set,
             batch_size=self.batch_size,
             shuffle=False,
             num_workers=self.num_workers,
         )
@@ -292,36 +282,29 @@
         result_dict = {
             "imputation": imputation,
         }
         return result_dict
 
     def impute(
         self,
-        X: Union[dict, str],
-        file_type="h5py",
+        test_set: Union[dict, str],
+        file_type: str = "hdf5",
     ) -> np.ndarray:
         """Impute missing values in the given data with the trained model.
 
-        Warnings
-        --------
-        The method impute is deprecated. Please use `predict()` instead.
-
         Parameters
         ----------
-        X :
-            The data samples for testing, should be array-like of shape [n_samples, sequence length (time steps),
+        test_set :
+            The data samples for testing, should be array-like of shape [n_samples, sequence length (n_steps),
             n_features], or a path string locating a data file, e.g. h5 file.
 
         file_type :
             The type of the given file if X is a path string.
 
         Returns
         -------
-        array-like, shape [n_samples, sequence length (time steps), n_features],
+        array-like, shape [n_samples, sequence length (n_steps), n_features],
             Imputed data.
         """
-        logger.warning(
-            "🚨DeprecationWarning: The method impute is deprecated. Please use `predict` instead."
-        )
 
-        results_dict = self.predict(X, file_type=file_type)
-        return results_dict["imputation"]
+        result_dict = self.predict(test_set, file_type=file_type)
+        return result_dict["imputation"]
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pypots-0.4.1/pypots/imputation/locf/core.py` & `pypots-0.5/pypots/imputation/locf/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-
+The core wrapper assembles the submodules of LOCF imputation model.
 """
 
 # Created by Wenjie Du <wenjay.du@gmail.com>
 # License: BSD-3-Clause
 
 import numpy as np
 import torch
```

### Comparing `pypots-0.4.1/pypots/imputation/locf/model.py` & `pypots-0.5/pypots/imputation/locf/model.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 
 import h5py
 import numpy as np
 import torch
 
 from .core import locf_numpy, locf_torch
 from ..base import BaseImputer
-from ...utils.logging import logger
 
 
 class LOCF(BaseImputer):
     """LOCF (Last Observed Carried Forward) imputation method. A naive imputation method that fills missing values
     with the last observed value. When time-series data gets inverse on the time dimension, this method can also be
     seen as NOCB (Next Observation Carried Backward). Simple but commonly used in practice.
 
@@ -51,15 +50,15 @@
         assert first_step_imputation in ["nan", "zero", "backward", "median"]
         self.first_step_imputation = first_step_imputation
 
     def fit(
         self,
         train_set: Union[dict, str],
         val_set: Optional[Union[dict, str]] = None,
-        file_type: str = "h5py",
+        file_type: str = "hdf5",
     ) -> None:
         """Train the imputer on the given data.
 
         Warnings
         --------
         LOCF does not need to run fit().
         Please run func ``predict()`` directly.
@@ -69,30 +68,30 @@
             "LOCF (Last Observed Carried Forward) imputation class has no parameter to train. "
             "Please run func `predict()` directly."
         )
 
     def predict(
         self,
         test_set: Union[dict, str],
-        file_type: str = "h5py",
+        file_type: str = "hdf5",
     ) -> dict:
         """Make predictions for the input data with the trained model.
 
         Parameters
         ----------
         test_set : dict or str
             The dataset for model validating, should be a dictionary including keys as 'X',
             or a path string locating a data file supported by PyPOTS (e.g. h5 file).
-            If it is a dict, X should be array-like of shape [n_samples, sequence length (time steps), n_features],
+            If it is a dict, X should be array-like of shape [n_samples, sequence length (n_steps), n_features],
             which is time-series data for validating, can contain missing values, and y should be array-like of shape
             [n_samples], which is classification labels of X.
             If it is a path string, the path should point to a data file, e.g. a h5 file, which contains
             key-value pairs like a dict, and it has to include keys as 'X' and 'y'.
 
-        file_type : str
+        file_type :
             The type of the given file if test_set is a path string.
 
         Returns
         -------
         result_dict: dict
             Prediction results in a Python Dictionary for the given samples.
             It should be a dictionary including keys as 'imputation', 'classification', 'clustering', and 'forecasting'.
@@ -123,35 +122,29 @@
         result_dict = {
             "imputation": imputed_data,
         }
         return result_dict
 
     def impute(
         self,
-        X: Union[dict, str],
-        file_type="h5py",
+        test_set: Union[dict, str],
+        file_type: str = "hdf5",
     ) -> np.ndarray:
         """Impute missing values in the given data with the trained model.
 
-        Warnings
-        --------
-        The method impute is deprecated. Please use `predict()` instead.
-
         Parameters
         ----------
-        X :
-            The data samples for testing, should be array-like of shape [n_samples, sequence length (time steps),
+        test_set :
+            The data samples for testing, should be array-like of shape [n_samples, sequence length (n_steps),
             n_features], or a path string locating a data file, e.g. h5 file.
 
         file_type :
             The type of the given file if X is a path string.
 
         Returns
         -------
-        array-like, shape [n_samples, sequence length (time steps), n_features],
+        array-like, shape [n_samples, sequence length (n_steps), n_features],
             Imputed data.
         """
-        logger.warning(
-            "🚨DeprecationWarning: The method impute is deprecated. Please use `predict` instead."
-        )
-        results_dict = self.predict(X, file_type=file_type)
-        return results_dict["imputation"]
+
+        result_dict = self.predict(test_set, file_type=file_type)
+        return result_dict["imputation"]
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pypots-0.4.1/pypots/imputation/mean/model.py` & `pypots-0.5/pypots/imputation/mean/model.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,30 +10,29 @@
 from typing import Union, Optional
 
 import h5py
 import numpy as np
 import torch
 
 from ..base import BaseImputer
-from ...utils.logging import logger
 
 
 class Mean(BaseImputer):
     """Mean value imputation method."""
 
     def __init__(
         self,
     ):
         super().__init__()
 
     def fit(
         self,
         train_set: Union[dict, str],
         val_set: Optional[Union[dict, str]] = None,
-        file_type: str = "h5py",
+        file_type: str = "hdf5",
     ) -> None:
         """Train the imputer on the given data.
 
         Warnings
         --------
         Mean imputation class does not need to run fit().
         Please run func ``predict()`` directly.
@@ -43,30 +42,30 @@
             "Mean imputation class has no parameter to train. "
             "Please run func `predict()` directly."
         )
 
     def predict(
         self,
         test_set: Union[dict, str],
-        file_type: str = "h5py",
+        file_type: str = "hdf5",
     ) -> dict:
         """Make predictions for the input data with the trained model.
 
         Parameters
         ----------
         test_set : dict or str
             The dataset for model validating, should be a dictionary including keys as 'X',
             or a path string locating a data file supported by PyPOTS (e.g. h5 file).
-            If it is a dict, X should be array-like of shape [n_samples, sequence length (time steps), n_features],
+            If it is a dict, X should be array-like of shape [n_samples, sequence length (n_steps), n_features],
             which is time-series data for validating, can contain missing values, and y should be array-like of shape
             [n_samples], which is classification labels of X.
             If it is a path string, the path should point to a data file, e.g. a h5 file, which contains
             key-value pairs like a dict, and it has to include keys as 'X' and 'y'.
 
-        file_type : str
+        file_type :
             The type of the given file if test_set is a path string.
 
         Returns
         -------
         result_dict: dict
             Prediction results in a Python Dictionary for the given samples.
             It should be a dictionary including keys as 'imputation', 'classification', 'clustering', and 'forecasting'.
@@ -109,35 +108,29 @@
         result_dict = {
             "imputation": imputed_data,
         }
         return result_dict
 
     def impute(
         self,
-        X: Union[dict, str],
-        file_type="h5py",
+        test_set: Union[dict, str],
+        file_type: str = "hdf5",
     ) -> np.ndarray:
         """Impute missing values in the given data with the trained model.
 
-        Warnings
-        --------
-        The method impute is deprecated. Please use `predict()` instead.
-
         Parameters
         ----------
-        X :
-            The data samples for testing, should be array-like of shape [n_samples, sequence length (time steps),
+        test_set :
+            The data samples for testing, should be array-like of shape [n_samples, sequence length (n_steps),
             n_features], or a path string locating a data file, e.g. h5 file.
 
         file_type :
             The type of the given file if X is a path string.
 
         Returns
         -------
-        array-like, shape [n_samples, sequence length (time steps), n_features],
+        array-like, shape [n_samples, sequence length (n_steps), n_features],
             Imputed data.
         """
-        logger.warning(
-            "🚨DeprecationWarning: The method impute is deprecated. Please use `predict` instead."
-        )
-        results_dict = self.predict(X, file_type=file_type)
-        return results_dict["imputation"]
+
+        result_dict = self.predict(test_set, file_type=file_type)
+        return result_dict["imputation"]
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pypots-0.4.1/pypots/imputation/median/model.py` & `pypots-0.5/pypots/imputation/median/model.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,30 +10,29 @@
 from typing import Union, Optional
 
 import h5py
 import numpy as np
 import torch
 
 from ..base import BaseImputer
-from ...utils.logging import logger
 
 
 class Median(BaseImputer):
     """Median value imputation method."""
 
     def __init__(
         self,
     ):
         super().__init__()
 
     def fit(
         self,
         train_set: Union[dict, str],
         val_set: Optional[Union[dict, str]] = None,
-        file_type: str = "h5py",
+        file_type: str = "hdf5",
     ) -> None:
         """Train the imputer on the given data.
 
         Warnings
         --------
         Median imputation class does not need to run fit().
         Please run func ``predict()`` directly.
@@ -43,30 +42,30 @@
             "Median imputation class has no parameter to train. "
             "Please run func `predict()` directly."
         )
 
     def predict(
         self,
         test_set: Union[dict, str],
-        file_type: str = "h5py",
+        file_type: str = "hdf5",
     ) -> dict:
         """Make predictions for the input data with the trained model.
 
         Parameters
         ----------
         test_set : dict or str
             The dataset for model validating, should be a dictionary including keys as 'X',
             or a path string locating a data file supported by PyPOTS (e.g. h5 file).
-            If it is a dict, X should be array-like of shape [n_samples, sequence length (time steps), n_features],
+            If it is a dict, X should be array-like of shape [n_samples, sequence length (n_steps), n_features],
             which is time-series data for validating, can contain missing values, and y should be array-like of shape
             [n_samples], which is classification labels of X.
             If it is a path string, the path should point to a data file, e.g. a h5 file, which contains
             key-value pairs like a dict, and it has to include keys as 'X' and 'y'.
 
-        file_type : str
+        file_type :
             The type of the given file if test_set is a path string.
 
         Returns
         -------
         result_dict: dict
             Prediction results in a Python Dictionary for the given samples.
             It should be a dictionary including keys as 'imputation', 'classification', 'clustering', and 'forecasting'.
@@ -110,35 +109,29 @@
         result_dict = {
             "imputation": imputed_data,
         }
         return result_dict
 
     def impute(
         self,
-        X: Union[dict, str],
-        file_type="h5py",
+        test_set: Union[dict, str],
+        file_type: str = "hdf5",
     ) -> np.ndarray:
         """Impute missing values in the given data with the trained model.
 
-        Warnings
-        --------
-        The method impute is deprecated. Please use `predict()` instead.
-
         Parameters
         ----------
-        X :
-            The data samples for testing, should be array-like of shape [n_samples, sequence length (time steps),
+        test_set :
+            The data samples for testing, should be array-like of shape [n_samples, sequence length (n_steps),
             n_features], or a path string locating a data file, e.g. h5 file.
 
         file_type :
             The type of the given file if X is a path string.
 
         Returns
         -------
-        array-like, shape [n_samples, sequence length (time steps), n_features],
+        array-like, shape [n_samples, sequence length (n_steps), n_features],
             Imputed data.
         """
-        logger.warning(
-            "🚨DeprecationWarning: The method impute is deprecated. Please use `predict` instead."
-        )
-        results_dict = self.predict(X, file_type=file_type)
-        return results_dict["imputation"]
+
+        result_dict = self.predict(test_set, file_type=file_type)
+        return result_dict["imputation"]
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pypots-0.4.1/pypots/imputation/mrnn/core.py` & `pypots-0.5/pypots/imputation/mrnn/core.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 """
-PyTorch MRNN model for the time-series imputation task.
-This implementation is inspired by the official one https://github.com/jsyoon0823/MRNN.
-Some part of the code is from https://github.com/WenjieDu/SAITS.
+The core wrapper assembles the submodules of M-RNN imputation model
+and takes over the forward progress of the algorithm.
 """
 
 # Created by Wenjie Du <wenjay.du@gmail.com>
 # License: BSD-3-Clause
 
 
 import torch.nn as nn
```

### Comparing `pypots-0.4.1/pypots/imputation/mrnn/data.py` & `pypots-0.5/pypots/imputation/brits/data.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,66 +1,72 @@
 """
-Dataset class for model MRNN.
+Dataset class for the imputation model BRITS.
 """
 
 # Created by Wenjie Du <wenjay.du@gmail.com>
 # License: BSD-3-Clause
 
 from typing import Union, Iterable
 
 import torch
 from pygrinder import fill_and_get_mask_torch
 
-from ...data.base import BaseDataset
+from ...data.dataset import BaseDataset
 from ...data.utils import _parse_delta_torch
 
 
-class DatasetForMRNN(BaseDataset):
+class DatasetForBRITS(BaseDataset):
     """Dataset class for BRITS.
 
     Parameters
     ----------
-    data : dict or str,
+    data :
         The dataset for model input, should be a dictionary including keys as 'X' and 'y',
         or a path string locating a data file.
-        If it is a dict, X should be array-like of shape [n_samples, sequence length (time steps), n_features],
+        If it is a dict, X should be array-like of shape [n_samples, sequence length (n_steps), n_features],
         which is time-series data for input, can contain missing values, and y should be array-like of shape
         [n_samples], which is classification labels of X.
         If it is a path string, the path should point to a data file, e.g. a h5 file, which contains
         key-value pairs like a dict, and it has to include keys as 'X' and 'y'.
 
-    return_labels : bool, default = True,
+    return_y :
         Whether to return labels in function __getitem__() if they exist in the given data. If `True`, for example,
         during training of classification models, the Dataset class will return labels in __getitem__() for model input.
         Otherwise, labels won't be included in the data returned by __getitem__(). This parameter exists because we
         need the defined Dataset class for all training/validating/testing stages. For those big datasets stored in h5
         files, they already have both X and y saved. But we don't read labels from the file for validating and testing
         with function _fetch_data_from_file(), which works for all three stages. Therefore, we need this parameter for
         distinction.
 
-    file_type : str, default = "h5py"
+    file_type :
         The type of the given file if train_set and val_set are path strings.
     """
 
     def __init__(
         self,
         data: Union[dict, str],
         return_X_ori: bool,
-        return_labels: bool,
-        file_type: str = "h5py",
+        return_y: bool,
+        file_type: str = "hdf5",
     ):
-        super().__init__(data, return_X_ori, return_labels, file_type)
+        super().__init__(
+            data=data,
+            return_X_ori=return_X_ori,
+            return_X_pred=False,
+            return_y=return_y,
+            file_type=file_type,
+        )
 
         if not isinstance(self.data, str):
             # calculate all delta here.
-            if self.X_ori is None:
-                forward_X, forward_missing_mask = fill_and_get_mask_torch(self.X)
-            else:
+            if self.return_X_ori:
                 forward_missing_mask = self.missing_mask
                 forward_X = self.X
+            else:
+                forward_X, forward_missing_mask = fill_and_get_mask_torch(self.X)
 
             forward_delta = _parse_delta_torch(forward_missing_mask)
             backward_X = torch.flip(forward_X, dims=[1])
             backward_missing_mask = torch.flip(forward_missing_mask, dims=[1])
             backward_delta = _parse_delta_torch(backward_missing_mask)
 
             self.processed_data = {
@@ -77,20 +83,20 @@
             }
 
     def _fetch_data_from_array(self, idx: int) -> Iterable:
         """Fetch data from self.X if it is given.
 
         Parameters
         ----------
-        idx : int,
+        idx :
             The index of the sample to be return.
 
         Returns
         -------
-        sample : list,
+        sample :
             A list contains
 
             index : int tensor,
                 The index of the sample.
 
             X : tensor,
                 The feature vector for model input.
@@ -112,34 +118,34 @@
             self.processed_data["forward"]["delta"][idx],
             # for backward
             self.processed_data["backward"]["X"][idx],
             self.processed_data["backward"]["missing_mask"][idx],
             self.processed_data["backward"]["delta"][idx],
         ]
 
-        if self.X_ori is not None and self.return_X_ori:
+        if self.return_X_ori:
             sample.extend([self.X_ori[idx], self.indicating_mask[idx]])
 
-        if self.y is not None and self.return_labels:
+        if self.return_y:
             sample.append(self.y[idx].to(torch.long))
 
         return sample
 
     def _fetch_data_from_file(self, idx: int) -> Iterable:
         """Fetch data with the lazy-loading strategy, i.e. only loading data from the file while requesting for samples.
         Here the opened file handle doesn't load the entire dataset into RAM but only load the currently accessed slice.
 
         Parameters
         ----------
-        idx : int,
+        idx :
             The index of the sample to be return.
 
         Returns
         -------
-        sample : list,
+        sample :
             The collated data sample, a list including all necessary sample info.
         """
 
         if self.file_handle is None:
             self.file_handle = self._open_file_handle()
 
         X = torch.from_numpy(self.file_handle["X"][idx]).to(torch.float32)
@@ -165,18 +171,18 @@
             forward["deltas"],
             # for backward
             backward["X"],
             backward["missing_mask"],
             backward["deltas"],
         ]
 
-        if "X_ori" in self.file_handle.keys() and self.return_X_ori:
+        if self.return_X_ori:
             X_ori = torch.from_numpy(self.file_handle["X_ori"][idx]).to(torch.float32)
             X_ori, X_ori_missing_mask = fill_and_get_mask_torch(X_ori)
             indicating_mask = X_ori_missing_mask - missing_mask
             sample.extend([X_ori, indicating_mask])
 
         # if the dataset has labels and is for training, then fetch it from the file
-        if "y" in self.file_handle.keys() and self.return_labels:
+        if self.return_y:
             sample.append(torch.tensor(self.file_handle["y"][idx], dtype=torch.long))
 
         return sample
```

### Comparing `pypots-0.4.1/pypots/imputation/mrnn/model.py` & `pypots-0.5/pypots/imputation/mrnn/model.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,10 @@
 """
 PyTorch M-RNN model for the time-series imputation task.
 
-Refer to the paper "Jinsung Yoon, William R. Zame, and Mihaela van der Schaar.
-Estimating missing data in temporal data streams using multi-directional recurrent neural networks.
-EEE Transactions on Biomedical Engineering, 66(5):14771490, 2019."
-
-This implementation is inspired by the official one https://github.com/jsyoon0823/MRNN.
-Some part of the code is from https://github.com/WenjieDu/SAITS.
-
 """
 
 # Created by Wenjie Du <wenjay.du@gmail.com>
 # License: BSD-3-Clause
 
 
 from typing import Union, Optional
@@ -19,18 +12,17 @@
 import numpy as np
 import torch
 from torch.utils.data import DataLoader
 
 from .core import _MRNN
 from .data import DatasetForMRNN
 from ..base import BaseNNImputer
-from ...data.checking import check_X_ori_in_val_set
+from ...data.checking import key_in_data_set
 from ...optim.adam import Adam
 from ...optim.base import Optimizer
-from ...utils.logging import logger
 
 
 class MRNN(BaseNNImputer):
     """The PyTorch implementation of the MRNN model :cite:`yoon2019MRNN`.
 
     Parameters
     ----------
@@ -190,32 +182,32 @@
     def _assemble_input_for_testing(self, data: list) -> dict:
         return self._assemble_input_for_training(data)
 
     def fit(
         self,
         train_set: Union[dict, str],
         val_set: Optional[Union[dict, str]] = None,
-        file_type: str = "h5py",
+        file_type: str = "hdf5",
     ) -> None:
         # Step 1: wrap the input data with classes Dataset and DataLoader
         training_set = DatasetForMRNN(
-            train_set, return_X_ori=False, return_labels=False, file_type=file_type
+            train_set, return_X_ori=False, return_y=False, file_type=file_type
         )
         training_loader = DataLoader(
             training_set,
             batch_size=self.batch_size,
             shuffle=True,
             num_workers=self.num_workers,
         )
         val_loader = None
         if val_set is not None:
-            if not check_X_ori_in_val_set(val_set):
+            if not key_in_data_set("X_ori", val_set):
                 raise ValueError("val_set must contain 'X_ori' for model validation.")
             val_set = DatasetForMRNN(
-                val_set, return_X_ori=True, return_labels=False, file_type=file_type
+                val_set, return_X_ori=True, return_y=False, file_type=file_type
             )
             val_loader = DataLoader(
                 val_set,
                 batch_size=self.batch_size,
                 shuffle=False,
                 num_workers=self.num_workers,
             )
@@ -227,19 +219,19 @@
 
         # Step 3: save the model if necessary
         self._auto_save_model_if_necessary(confirm_saving=True)
 
     def predict(
         self,
         test_set: Union[dict, str],
-        file_type="h5py",
+        file_type: str = "hdf5",
     ) -> dict:
         self.model.eval()  # set the model as eval status to freeze it.
         test_set = DatasetForMRNN(
-            test_set, return_X_ori=False, return_labels=False, file_type=file_type
+            test_set, return_X_ori=False, return_y=False, file_type=file_type
         )
         test_loader = DataLoader(
             test_set,
             batch_size=self.batch_size,
             shuffle=False,
             num_workers=self.num_workers,
         )
@@ -256,35 +248,29 @@
         result_dict = {
             "imputation": imputation,
         }
         return result_dict
 
     def impute(
         self,
-        X: Union[dict, str],
-        file_type="h5py",
+        test_set: Union[dict, str],
+        file_type: str = "hdf5",
     ) -> np.ndarray:
         """Impute missing values in the given data with the trained model.
 
-        Warnings
-        --------
-        The method impute is deprecated. Please use `predict()` instead.
-
         Parameters
         ----------
-        X :
-            The data samples for testing, should be array-like of shape [n_samples, sequence length (time steps),
+        test_set :
+            The data samples for testing, should be array-like of shape [n_samples, sequence length (n_steps),
             n_features], or a path string locating a data file, e.g. h5 file.
 
         file_type :
             The type of the given file if X is a path string.
 
         Returns
         -------
-        array-like, shape [n_samples, sequence length (time steps), n_features],
+        array-like, shape [n_samples, sequence length (n_steps), n_features],
             Imputed data.
         """
-        logger.warning(
-            "🚨DeprecationWarning: The method impute is deprecated. Please use `predict` instead."
-        )
-        results_dict = self.predict(X, file_type=file_type)
-        return results_dict["imputation"]
+
+        result_dict = self.predict(test_set, file_type=file_type)
+        return result_dict["imputation"]
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pypots-0.4.1/pypots/imputation/patchtst/core.py` & `pypots-0.5/pypots/imputation/patchtst/core.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,66 +1,73 @@
 """
-
+The core wrapper assembles the submodules of PatchTST imputation model
+and takes over the forward progress of the algorithm.
 """
 
 # Created by Wenjie Du <wenjay.du@gmail.com>
 # License: BSD-3-Clause
 
-import torch
 import torch.nn as nn
 
 from ...nn.modules.patchtst import PatchEmbedding, PatchtstEncoder, PredictionHead
-from ...nn.modules.saits import SaitsLoss
+from ...nn.modules.saits import SaitsLoss, SaitsEmbedding
 
 
 class _PatchTST(nn.Module):
     def __init__(
         self,
         n_steps: int,
         n_features: int,
         n_layers: int,
-        n_heads: int,
         d_model: int,
-        d_ffn: int,
+        n_heads: int,
         d_k: int,
         d_v: int,
+        d_ffn: int,
         patch_len: int,
         stride: int,
         dropout: float,
         attn_dropout: float,
         ORT_weight: float = 1,
         MIT_weight: float = 1,
     ):
         super().__init__()
 
         n_patches = int((n_steps - patch_len) / stride + 2)  # number of patches
         padding = stride
 
-        self.embedding = nn.Linear(n_features * 2, d_model)
+        self.saits_embedding = SaitsEmbedding(n_features * 2, d_model, with_pos=False)
         self.patch_embedding = PatchEmbedding(
             d_model, patch_len, stride, padding, dropout
         )
         self.encoder = PatchtstEncoder(
-            n_layers, n_heads, d_model, d_ffn, d_k, d_v, dropout, attn_dropout
+            n_layers,
+            d_model,
+            n_heads,
+            d_k,
+            d_v,
+            d_ffn,
+            dropout,
+            attn_dropout,
         )
         self.head = PredictionHead(d_model, n_patches, n_steps, dropout)
         self.output_projection = nn.Linear(d_model, n_features)
         self.saits_loss_func = SaitsLoss(ORT_weight, MIT_weight)
 
     def forward(self, inputs: dict, training: bool = True) -> dict:
         X, missing_mask = inputs["X"], inputs["missing_mask"]
 
         # WDU: the original PatchTST paper isn't proposed for imputation task. Hence the model doesn't take
         # the missing mask into account, which means, in the process, the model doesn't know which part of
-        # the input data is missing, and this may hurt the model's imputation performance. Therefore, I add the
-        # embedding layers to project the concatenation of features and masks into a hidden space, as well as
+        # the input data is missing, and this may hurt the model's imputation performance. Therefore, I apply the
+        # SAITS embedding method to project the concatenation of features and masks into a hidden space, as well as
         # the output layers to project back from the hidden space to the original space.
+        input_X = self.saits_embedding(X, missing_mask)
 
-        # do patching and embedding
-        input_X = self.embedding(torch.cat([X, missing_mask], dim=2))
+        # do patch  embedding
         enc_out = self.patch_embedding(
             input_X.permute(0, 2, 1)
         )  # [bz * d_model, n_patches, d_model]
 
         # PatchTST encoder processing
         enc_out, attns = self.encoder(enc_out)
```

### Comparing `pypots-0.4.1/pypots/imputation/patchtst/data.py` & `pypots-0.5/pypots/imputation/patchtst/data.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Dataset class for PatchTST.
+Dataset class for the imputation model PatchTST.
 """
 
 # Created by Wenjie Du <wenjay.du@gmail.com>
 # License: BSD-3-Clause
 
 from typing import Union
 
@@ -13,12 +13,12 @@
 class DatasetForPatchTST(DatasetForSAITS):
     """Actually PatchTST uses the same data strategy as SAITS, needs MIT for training."""
 
     def __init__(
         self,
         data: Union[dict, str],
         return_X_ori: bool,
-        return_labels: bool,
-        file_type: str = "h5py",
+        return_y: bool,
+        file_type: str = "hdf5",
         rate: float = 0.2,
     ):
-        super().__init__(data, return_X_ori, return_labels, file_type, rate)
+        super().__init__(data, return_X_ori, return_y, file_type, rate)
```

### Comparing `pypots-0.4.1/pypots/imputation/patchtst/model.py` & `pypots-0.5/pypots/imputation/patchtst/model.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,35 +1,30 @@
 """
 The implementation of PatchTST for the partially-observed time-series imputation task.
 
 Refer to the paper "Yuqi Nie, Nam H Nguyen, Phanwadee Sinthong, and Jayant Kalagnanam.
 A time series is worth 64 words: Long-term forecasting with transformers.
 In The ICLR, 2023."
 
-Notes
------
-Partial implementation uses code from
-https://github.com/yuqinie98/PatchTST and https://github.com/thuml/Time-Series-Library
-
 """
 
 # Created by Wenjie Du <wenjay.du@gmail.com>
 # License: BSD-3-Clause
 
 from typing import Union, Optional
 
 import numpy as np
 import torch
 from torch.utils.data import DataLoader
 
+from .core import _PatchTST
 from .data import DatasetForPatchTST
-from pypots.imputation.patchtst.core import _PatchTST
 from ..base import BaseNNImputer
-from ...data.base import BaseDataset
-from ...data.checking import check_X_ori_in_val_set
+from ...data.checking import key_in_data_set
+from ...data.dataset import BaseDataset
 from ...optim.adam import Adam
 from ...optim.base import Optimizer
 from ...utils.logging import logger
 
 
 class PatchTST(BaseNNImputer):
     """The PyTorch implementation of the PatchTST model.
@@ -48,29 +43,29 @@
 
     stride :
         The stride for patch embedding.
 
     n_layers :
         The number of layers in the PatchTST model.
 
+    d_model :
+        The dimension of the model.
+
     n_heads :
         The number of heads in each layer of PatchTST.
 
     d_k :
         The dimension of the `keys` (K) and the `queries` (Q) in the DMSA mechanism.
         ``d_k`` should be the result of ``d_model`` divided by ``n_heads``. Although ``d_k`` can be directly calculated
         with given ``d_model`` and ``n_heads``, we want it be explicitly given together with ``d_v`` by users to ensure
         users be aware of them and to avoid any potential mistakes.
 
     d_v :
         The dimension of the `values` (V) in the DMSA mechanism.
 
-    d_model :
-        The dimension of the model.
-
     d_ffn :
         The dimension of the feed-forward network.
 
     dropout :
         The dropout rate for the model.
 
     ORT_weight :
@@ -123,18 +118,18 @@
     def __init__(
         self,
         n_steps: int,
         n_features: int,
         patch_len: int,
         stride: int,
         n_layers: int,
+        d_model: int,
         n_heads: int,
         d_k: int,
         d_v: int,
-        d_model: int,
         d_ffn: int,
         dropout: float,
         attn_dropout: float,
         ORT_weight: float = 1,
         MIT_weight: float = 1,
         batch_size: int = 32,
         epochs: int = 100,
@@ -181,19 +176,19 @@
         self.MIT_weight = MIT_weight
 
         # set up the model
         self.model = _PatchTST(
             self.n_steps,
             self.n_features,
             self.n_layers,
-            self.n_heads,
             self.d_model,
-            self.d_ffn,
+            self.n_heads,
             self.d_k,
             self.d_v,
+            self.d_ffn,
             self.patch_len,
             self.stride,
             self.dropout,
             self.attn_dropout,
             self.ORT_weight,
             self.MIT_weight,
         )
@@ -235,32 +230,32 @@
 
         return inputs
 
     def fit(
         self,
         train_set: Union[dict, str],
         val_set: Optional[Union[dict, str]] = None,
-        file_type: str = "h5py",
+        file_type: str = "hdf5",
     ) -> None:
         # Step 1: wrap the input data with classes Dataset and DataLoader
         training_set = DatasetForPatchTST(
-            train_set, return_X_ori=False, return_labels=False, file_type=file_type
+            train_set, return_X_ori=False, return_y=False, file_type=file_type
         )
         training_loader = DataLoader(
             training_set,
             batch_size=self.batch_size,
             shuffle=True,
             num_workers=self.num_workers,
         )
         val_loader = None
         if val_set is not None:
-            if not check_X_ori_in_val_set(val_set):
+            if not key_in_data_set("X_ori", val_set):
                 raise ValueError("val_set must contain 'X_ori' for model validation.")
             val_set = DatasetForPatchTST(
-                val_set, return_X_ori=True, return_labels=False, file_type=file_type
+                val_set, return_X_ori=True, return_y=False, file_type=file_type
             )
             val_loader = DataLoader(
                 val_set,
                 batch_size=self.batch_size,
                 shuffle=False,
                 num_workers=self.num_workers,
             )
@@ -272,42 +267,46 @@
 
         # Step 3: save the model if necessary
         self._auto_save_model_if_necessary(confirm_saving=True)
 
     def predict(
         self,
         test_set: Union[dict, str],
-        file_type: str = "h5py",
+        file_type: str = "hdf5",
     ) -> dict:
         """Make predictions for the input data with the trained model.
 
         Parameters
         ----------
         test_set : dict or str
             The dataset for model validating, should be a dictionary including keys as 'X',
             or a path string locating a data file supported by PyPOTS (e.g. h5 file).
-            If it is a dict, X should be array-like of shape [n_samples, sequence length (time steps), n_features],
+            If it is a dict, X should be array-like of shape [n_samples, sequence length (n_steps), n_features],
             which is time-series data for validating, can contain missing values, and y should be array-like of shape
             [n_samples], which is classification labels of X.
             If it is a path string, the path should point to a data file, e.g. a h5 file, which contains
             key-value pairs like a dict, and it has to include keys as 'X' and 'y'.
 
-        file_type : str
+        file_type :
             The type of the given file if test_set is a path string.
 
         Returns
         -------
-        result_dict : dict,
+        file_type :
             The dictionary containing the clustering results and latent variables if necessary.
 
         """
         # Step 1: wrap the input data with classes Dataset and DataLoader
         self.model.eval()  # set the model as eval status to freeze it.
         test_set = BaseDataset(
-            test_set, return_X_ori=False, return_labels=False, file_type=file_type
+            test_set,
+            return_X_ori=False,
+            return_X_pred=False,
+            return_y=False,
+            file_type=file_type,
         )
         test_loader = DataLoader(
             test_set,
             batch_size=self.batch_size,
             shuffle=False,
             num_workers=self.num_workers,
         )
@@ -325,36 +324,29 @@
         result_dict = {
             "imputation": imputation,
         }
         return result_dict
 
     def impute(
         self,
-        X: Union[dict, str],
-        file_type="h5py",
+        test_set: Union[dict, str],
+        file_type: str = "hdf5",
     ) -> np.ndarray:
         """Impute missing values in the given data with the trained model.
 
-        Warnings
-        --------
-        The method impute is deprecated. Please use `predict()` instead.
-
         Parameters
         ----------
-        X :
-            The data samples for testing, should be array-like of shape [n_samples, sequence length (time steps),
+        test_set :
+            The data samples for testing, should be array-like of shape [n_samples, sequence length (n_steps),
             n_features], or a path string locating a data file, e.g. h5 file.
 
         file_type :
             The type of the given file if X is a path string.
 
         Returns
         -------
-        array-like, shape [n_samples, sequence length (time steps), n_features],
+        array-like, shape [n_samples, sequence length (n_steps), n_features],
             Imputed data.
         """
-        logger.warning(
-            "🚨DeprecationWarning: The method impute is deprecated. Please use `predict` instead."
-        )
 
-        results_dict = self.predict(X, file_type=file_type)
-        return results_dict["imputation"]
+        result_dict = self.predict(test_set, file_type=file_type)
+        return result_dict["imputation"]
```

### Comparing `pypots-0.4.1/pypots/imputation/saits/core.py` & `pypots-0.5/pypots/imputation/saits/core.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,42 +1,36 @@
 """
-The implementation of SAITS for the partially-observed time-series imputation task.
-
-Refer to the paper "Du, W., Cote, D., & Liu, Y. (2023). SAITS: Self-Attention-based Imputation for Time Series.
-Expert systems with applications."
-
-Notes
------
-Partial implementation uses code from https://github.com/WenjieDu/SAITS.
+The core wrapper assembles the submodules of SAITS imputation model
+and takes over the forward progress of the algorithm.
 
 """
 
 # Created by Wenjie Du <wenjay.du@gmail.com>
 # License: BSD-3-Clause
 
 from typing import Callable
 
 import torch
 import torch.nn as nn
 
-from pypots.utils.metrics import calc_mae
 from ...nn.modules.saits import BackboneSAITS
+from ...utils.metrics import calc_mae
 
 
 class _SAITS(nn.Module):
     def __init__(
         self,
         n_layers: int,
         n_steps: int,
         n_features: int,
         d_model: int,
-        d_ffn: int,
         n_heads: int,
         d_k: int,
         d_v: int,
+        d_ffn: int,
         dropout: float,
         attn_dropout: float,
         diagonal_attention_mask: bool = True,
         ORT_weight: float = 1,
         MIT_weight: float = 1,
         customized_loss_func: Callable = calc_mae,
     ):
@@ -45,22 +39,22 @@
         self.n_steps = n_steps
         self.diagonal_attention_mask = diagonal_attention_mask
         self.ORT_weight = ORT_weight
         self.MIT_weight = MIT_weight
         self.customized_loss_func = customized_loss_func
 
         self.encoder = BackboneSAITS(
-            n_layers,
             n_steps,
             n_features,
+            n_layers,
             d_model,
-            d_ffn,
             n_heads,
             d_k,
             d_v,
+            d_ffn,
             dropout,
             attn_dropout,
         )
 
     def forward(
         self,
         inputs: dict,
```

### Comparing `pypots-0.4.1/pypots/imputation/saits/data.py` & `pypots-0.5/pypots/imputation/saits/data.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,48 +1,48 @@
 """
-Dataset class for self-attention models trained with MIT (masked imputation task) task.
+Dataset class for the imputation model SAITS.
 """
 
 # Created by Wenjie Du <wenjay.du@gmail.com>
 # License: BSD-3-Clause
 
 from typing import Union, Iterable
 
 import torch
 from pygrinder import mcar, fill_and_get_mask_torch
 
-from ...data.base import BaseDataset
+from ...data.dataset import BaseDataset
 
 
 class DatasetForSAITS(BaseDataset):
     """Dataset for models that need MIT (masked imputation task) in their training, such as SAITS.
 
     For more information about MIT, please refer to :cite:`du2023SAITS`.
 
     Parameters
     ----------
-    data : dict or str,
+    data :
         The dataset for model input, should be a dictionary including keys as 'X' and 'y',
         or a path string locating a data file.
-        If it is a dict, X should be array-like of shape [n_samples, sequence length (time steps), n_features],
+        If it is a dict, X should be array-like of shape [n_samples, sequence length (n_steps), n_features],
         which is time-series data for input, can contain missing values, and y should be array-like of shape
         [n_samples], which is classification labels of X.
         If it is a path string, the path should point to a data file, e.g. a h5 file, which contains
         key-value pairs like a dict, and it has to include keys as 'X' and 'y'.
 
-    return_labels : bool, default = True,
+    return_y :
         Whether to return labels in function __getitem__() if they exist in the given data. If `True`, for example,
         during training of classification models, the Dataset class will return labels in __getitem__() for model input.
         Otherwise, labels won't be included in the data returned by __getitem__(). This parameter exists because we
         need the defined Dataset class for all training/validating/testing stages. For those big datasets stored in h5
         files, they already have both X and y saved. But we don't read labels from the file for validating and testing
         with function _fetch_data_from_file(), which works for all three stages. Therefore, we need this parameter for
         distinction.
 
-    file_type : str, default = "h5py"
+    file_type :
         The type of the given file if train_set and val_set are path strings.
 
     rate : float, in (0,1),
         Artificially missing rate, rate of the observed values which will be artificially masked as missing.
         Note that, `rate` = (number of artificially missing values) / np.sum(~np.isnan(self.data)),
         not (number of artificially missing values) / np.product(self.data.shape),
         considering that the given data may already contain missing values,
@@ -50,51 +50,57 @@
         the function will do nothing, i.e. it won't play the role it has to be.
     """
 
     def __init__(
         self,
         data: Union[dict, str],
         return_X_ori: bool,
-        return_labels: bool,
-        file_type: str = "h5py",
+        return_y: bool,
+        file_type: str = "hdf5",
         rate: float = 0.2,
     ):
-        super().__init__(data, return_X_ori, return_labels, file_type)
+        super().__init__(
+            data=data,
+            return_X_ori=return_X_ori,
+            return_X_pred=False,
+            return_y=return_y,
+            file_type=file_type,
+        )
         self.rate = rate
 
     def _fetch_data_from_array(self, idx: int) -> Iterable:
         """Fetch data according to index.
 
         Parameters
         ----------
-        idx : int,
+        idx :
             The index to fetch the specified sample.
 
         Returns
         -------
-        sample : list,
+        sample :
             A list contains
 
-            index : int tensor,
+            index :
                 The index of the sample.
 
-            X_ori : tensor,
+            X_ori :
                 Original time-series for calculating mask imputation loss.
 
-            X : tensor,
+            X :
                 Time-series data with artificially missing values for model input.
 
-            missing_mask : tensor,
+            missing_mask :
                 The mask records all missing values in X.
 
-            indicating_mask : tensor.
+            indicating_mask :
                 The mask indicates artificially missing values in X.
         """
 
-        if self.X_ori is not None and self.return_X_ori:
+        if self.return_X_ori:
             X = self.X[idx]
             X_ori = self.X_ori[idx]
             missing_mask = self.missing_mask[idx]
             indicating_mask = self.indicating_mask[idx]
         else:
             X_ori = self.X[idx]
             X = mcar(X_ori, p=self.rate)
@@ -106,38 +112,38 @@
             torch.tensor(idx),
             X,
             missing_mask,
             X_ori,
             indicating_mask,
         ]
 
-        if self.y is not None and self.return_labels:
+        if self.return_y:
             sample.append(self.y[idx].to(torch.long))
 
         return sample
 
     def _fetch_data_from_file(self, idx: int) -> Iterable:
         """Fetch data with the lazy-loading strategy, i.e. only loading data from the file while requesting for samples.
         Here the opened file handle doesn't load the entire dataset into RAM but only load the currently accessed slice.
 
         Parameters
         ----------
-        idx : int,
+        idx :
             The index of the sample to be return.
 
         Returns
         -------
-        sample : list,
+        sample :
             The collated data sample, a list including all necessary sample info.
         """
 
         if self.file_handle is None:
             self.file_handle = self._open_file_handle()
 
-        if "X_ori" in self.file_handle.keys() and self.return_X_ori:
+        if self.return_X_ori:
             X = torch.from_numpy(self.file_handle["X"][idx]).to(torch.float32)
             X_ori = torch.from_numpy(self.file_handle["X_ori"][idx]).to(torch.float32)
             X_ori, X_ori_missing_mask = fill_and_get_mask_torch(X_ori)
             X, missing_mask = fill_and_get_mask_torch(X)
             indicating_mask = (X_ori_missing_mask - missing_mask).to(torch.float32)
         else:
             X_ori = torch.from_numpy(self.file_handle["X"][idx]).to(torch.float32)
@@ -145,11 +151,11 @@
             X_ori, X_ori_missing_mask = fill_and_get_mask_torch(X_ori)
             X, missing_mask = fill_and_get_mask_torch(X)
             indicating_mask = (X_ori_missing_mask - missing_mask).to(torch.float32)
 
         sample = [torch.tensor(idx), X, missing_mask, X_ori, indicating_mask]
 
         # if the dataset has labels and is for training, then fetch it from the file
-        if "y" in self.file_handle.keys() and self.return_labels:
+        if self.return_y:
             sample.append(torch.tensor(self.file_handle["y"][idx], dtype=torch.long))
 
         return sample
```

### Comparing `pypots-0.4.1/pypots/imputation/saits/model.py` & `pypots-0.5/pypots/imputation/saits/model.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,34 +1,26 @@
 """
 The implementation of SAITS for the partially-observed time-series imputation task.
 
-Refer to the paper "Wenjie Du, David Cote, and Yan Liu.
-SAITS: Self-Attention-based Imputation for Time Series.
-Expert Systems with Applications, 219:119619, 2023."
-
-Notes
------
-Partial implementation uses code from https://github.com/WenjieDu/SAITS.
-
 """
 
 # Created by Wenjie Du <wenjay.du@gmail.com>
 # License: BSD-3-Clause
 
 from typing import Union, Optional, Callable
 
 import numpy as np
 import torch
 from torch.utils.data import DataLoader
 
-from .data import DatasetForSAITS
 from .core import _SAITS
+from .data import DatasetForSAITS
 from ..base import BaseNNImputer
-from ...data.base import BaseDataset
-from ...data.checking import check_X_ori_in_val_set
+from ...data.checking import key_in_data_set
+from ...data.dataset import BaseDataset
 from ...optim.adam import Adam
 from ...optim.base import Optimizer
 from ...utils.logging import logger
 from ...utils.metrics import calc_mae
 
 
 class SAITS(BaseNNImputer):
@@ -45,30 +37,30 @@
     n_layers :
         The number of layers in the 1st and 2nd DMSA blocks in the SAITS model.
 
     d_model :
         The dimension of the model's backbone.
         It is the input dimension of the multi-head DMSA layers.
 
-    d_ffn :
-        The dimension of the layer in the Feed-Forward Networks (FFN).
-
     n_heads :
         The number of heads in the multi-head DMSA mechanism.
         ``d_model`` must be divisible by ``n_heads``, and the result should be equal to ``d_k``.
 
     d_k :
         The dimension of the `keys` (K) and the `queries` (Q) in the DMSA mechanism.
         ``d_k`` should be the result of ``d_model`` divided by ``n_heads``. Although ``d_k`` can be directly calculated
         with given ``d_model`` and ``n_heads``, we want it be explicitly given together with ``d_v`` by users to ensure
         users be aware of them and to avoid any potential mistakes.
 
     d_v :
         The dimension of the `values` (V) in the DMSA mechanism.
 
+    d_ffn :
+        The dimension of the layer in the Feed-Forward Networks (FFN).
+
     dropout :
         The dropout rate for all fully-connected layers in the model.
 
     attn_dropout :
         The dropout rate for DMSA.
 
     diagonal_attention_mask :
@@ -128,18 +120,18 @@
 
     def __init__(
         self,
         n_steps: int,
         n_features: int,
         n_layers: int,
         d_model: int,
-        d_ffn: int,
         n_heads: int,
         d_k: int,
         d_v: int,
+        d_ffn: int,
         dropout: float = 0,
         attn_dropout: float = 0,
         diagonal_attention_mask: bool = True,
         ORT_weight: int = 1,
         MIT_weight: int = 1,
         batch_size: int = 32,
         epochs: int = 100,
@@ -188,18 +180,18 @@
 
         # set up the model
         self.model = _SAITS(
             self.n_layers,
             self.n_steps,
             self.n_features,
             self.d_model,
-            self.d_ffn,
             self.n_heads,
             self.d_k,
             self.d_v,
+            self.d_ffn,
             self.dropout,
             self.attn_dropout,
             self.diagonal_attention_mask,
             self.ORT_weight,
             self.MIT_weight,
         )
         self._print_model_size()
@@ -242,32 +234,32 @@
         }
         return inputs
 
     def fit(
         self,
         train_set: Union[dict, str],
         val_set: Optional[Union[dict, str]] = None,
-        file_type: str = "h5py",
+        file_type: str = "hdf5",
     ) -> None:
         # Step 1: wrap the input data with classes Dataset and DataLoader
         training_set = DatasetForSAITS(
-            train_set, return_X_ori=False, return_labels=False, file_type=file_type
+            train_set, return_X_ori=False, return_y=False, file_type=file_type
         )
         training_loader = DataLoader(
             training_set,
             batch_size=self.batch_size,
             shuffle=True,
             num_workers=self.num_workers,
         )
         val_loader = None
         if val_set is not None:
-            if not check_X_ori_in_val_set(val_set):
+            if not key_in_data_set("X_ori", val_set):
                 raise ValueError("val_set must contain 'X_ori' for model validation.")
             val_set = DatasetForSAITS(
-                val_set, return_X_ori=True, return_labels=False, file_type=file_type
+                val_set, return_X_ori=True, return_y=False, file_type=file_type
             )
             val_loader = DataLoader(
                 val_set,
                 batch_size=self.batch_size,
                 shuffle=False,
                 num_workers=self.num_workers,
             )
@@ -279,51 +271,55 @@
 
         # Step 3: save the model if necessary
         self._auto_save_model_if_necessary(confirm_saving=True)
 
     def predict(
         self,
         test_set: Union[dict, str],
-        file_type: str = "h5py",
+        file_type: str = "hdf5",
         diagonal_attention_mask: bool = True,
         return_latent_vars: bool = False,
     ) -> dict:
         """Make predictions for the input data with the trained model.
 
         Parameters
         ----------
-        test_set : dict or str
+        test_set :
             The dataset for model validating, should be a dictionary including keys as 'X',
             or a path string locating a data file supported by PyPOTS (e.g. h5 file).
-            If it is a dict, X should be array-like of shape [n_samples, sequence length (time steps), n_features],
+            If it is a dict, X should be array-like of shape [n_samples, sequence length (n_steps), n_features],
             which is time-series data for validating, can contain missing values, and y should be array-like of shape
             [n_samples], which is classification labels of X.
             If it is a path string, the path should point to a data file, e.g. a h5 file, which contains
             key-value pairs like a dict, and it has to include keys as 'X' and 'y'.
 
-        file_type : str
+        file_type :
             The type of the given file if test_set is a path string.
 
-        diagonal_attention_mask : bool
+        diagonal_attention_mask :
             Whether to apply a diagonal attention mask to the self-attention mechanism in the testing stage.
 
-        return_latent_vars : bool
+        return_latent_vars :
             Whether to return the latent variables in SAITS, e.g. attention weights of two DMSA blocks and
             the weight matrix from the combination block, etc.
 
         Returns
         -------
-        result_dict : dict,
+        file_type :
             The dictionary containing the clustering results and latent variables if necessary.
 
         """
         # Step 1: wrap the input data with classes Dataset and DataLoader
         self.model.eval()  # set the model as eval status to freeze it.
         test_set = BaseDataset(
-            test_set, return_X_ori=False, return_labels=False, file_type=file_type
+            test_set,
+            return_X_ori=False,
+            return_X_pred=False,
+            return_y=False,
+            file_type=file_type,
         )
         test_loader = DataLoader(
             test_set,
             batch_size=self.batch_size,
             shuffle=False,
             num_workers=self.num_workers,
         )
@@ -370,36 +366,29 @@
             }
             result_dict["latent_vars"] = latent_var_collector
 
         return result_dict
 
     def impute(
         self,
-        X: Union[dict, str],
-        file_type="h5py",
+        test_set: Union[dict, str],
+        file_type: str = "hdf5",
     ) -> np.ndarray:
         """Impute missing values in the given data with the trained model.
 
-        Warnings
-        --------
-        The method impute is deprecated. Please use `predict()` instead.
-
         Parameters
         ----------
-        X :
-            The data samples for testing, should be array-like of shape [n_samples, sequence length (time steps),
+        test_set :
+            The data samples for testing, should be array-like of shape [n_samples, sequence length (n_steps),
             n_features], or a path string locating a data file, e.g. h5 file.
 
         file_type :
             The type of the given file if X is a path string.
 
         Returns
         -------
-        array-like, shape [n_samples, sequence length (time steps), n_features],
+        array-like, shape [n_samples, sequence length (n_steps), n_features],
             Imputed data.
         """
-        logger.warning(
-            "🚨DeprecationWarning: The method impute is deprecated. Please use `predict` instead."
-        )
 
-        results_dict = self.predict(X, file_type=file_type)
-        return results_dict["imputation"]
+        result_dict = self.predict(test_set, file_type=file_type)
+        return result_dict["imputation"]
```

### Comparing `pypots-0.4.1/pypots/imputation/timesnet/core.py` & `pypots-0.5/pypots/imputation/timesnet/core.py`

 * *Files identical despite different names*

### Comparing `pypots-0.4.1/pypots/imputation/timesnet/model.py` & `pypots-0.5/pypots/imputation/fedformer/model.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,73 +1,76 @@
 """
-The implementation of TimesNet for the partially-observed time-series imputation task.
-
-Refer to the paper "Haixu Wu, Tengge Hu, Yong Liu, Hang Zhou, Jianmin Wang, and Mingsheng Long.
-TimesNet: Temporal 2D-Variation Modeling for General Time Series Analysis.
-In ICLR, 2023."
-
-Notes
------
-Partial implementation uses code from https://github.com/thuml/Time-Series-Library.
+The implementation of FEDformer for the partially-observed time-series imputation task.
 
 """
 
 # Created by Wenjie Du <wenjay.du@gmail.com>
 # License: BSD-3-Clause
 
 from typing import Union, Optional
 
 import numpy as np
 import torch
 from torch.utils.data import DataLoader
 
-from .core import _TimesNet
-from .data import DatasetForTimesNet
+from .core import _FEDformer
+from .data import DatasetForFEDformer
 from ..base import BaseNNImputer
-from ...data.base import BaseDataset
-from ...data.checking import check_X_ori_in_val_set
+from ...data.checking import key_in_data_set
+from ...data.dataset import BaseDataset
 from ...optim.adam import Adam
 from ...optim.base import Optimizer
-from ...utils.logging import logger
 
 
-class TimesNet(BaseNNImputer):
-    """The PyTorch implementation of the TimesNet model.
-    TimesNet is originally proposed by Wu et al. in :cite:`wu2023timesnet`.
+class FEDformer(BaseNNImputer):
+    """The PyTorch implementation of the FEDformer model.
+    FEDformer is originally proposed by Woo et al. in :cite:`zhou2022fedformer`.
 
     Parameters
     ----------
     n_steps :
         The number of time steps in the time-series data sample.
 
     n_features :
         The number of features in the time-series data sample.
 
     n_layers :
-        The number of layers in the TimesNet model.
+        The number of layers in the FEDformer.
 
-    top_k :
-        The number of top-k amplitude values to be selected to  obtain the most significant frequencies.
+    n_heads :
+        The number of heads in the multi-head attention mechanism.
 
     d_model :
         The dimension of the model.
 
     d_ffn :
         The dimension of the feed-forward network.
 
-    n_kernels :
-        The number of 2D kernels (2D convolutional layers) to use in the submodule InceptionBlockV1.
+    moving_avg_window_size :
+        The window size of moving average.
 
     dropout :
         The dropout rate for the model.
 
-    apply_nonstationary_norm :
-        Whether to apply non-stationary normalization to the input data for TimesNet.
-        Please refer to :cite:`liu2022nonstationary` for details about non-stationary normalization,
-        which is not the idea of the original TimesNet paper. Hence, we make it optional and default not to use here.
+    version :
+        The version of the model. It has to be one of ["Wavelets", "Fourier"].
+        The default value is "Fourier".
+
+    modes :
+        The number of modes to be selected. The default value is 32.
+
+    mode_select :
+        Get modes on frequency domain. It has to "random" or "low". The default value is "random".
+        'random' means sampling randomly; 'low' means sampling the lowest modes;
+
+    ORT_weight :
+        The weight for the ORT loss, the same as SAITS.
+
+    MIT_weight :
+        The weight for the MIT loss, the same as SAITS.
 
     batch_size :
         The batch size for training and evaluating the model.
 
     epochs :
         The number of epochs for training the model.
 
@@ -104,23 +107,27 @@
         better than in previous epochs.
         The "all" strategy will save every model after each epoch training.
 
     """
 
     def __init__(
         self,
-        n_steps: int,
-        n_features: int,
-        n_layers: int,
-        top_k: int,
-        d_model: int,
-        d_ffn: int,
-        n_kernels: int,
+        n_steps,
+        n_features,
+        n_layers,
+        d_model,
+        n_heads,
+        d_ffn,
+        moving_avg_window_size,
         dropout: float = 0,
-        apply_nonstationary_norm: bool = False,
+        version="Fourier",
+        modes=32,
+        mode_select="random",
+        ORT_weight: float = 1,
+        MIT_weight: float = 1,
         batch_size: int = 32,
         epochs: int = 100,
         patience: int = None,
         optimizer: Optional[Optimizer] = Adam(),
         num_workers: int = 0,
         device: Optional[Union[str, torch.device, list]] = None,
         saving_path: str = None,
@@ -136,32 +143,40 @@
             model_saving_strategy,
         )
 
         self.n_steps = n_steps
         self.n_features = n_features
         # model hype-parameters
         self.n_layers = n_layers
-        self.top_k = top_k
+        self.n_heads = n_heads
         self.d_model = d_model
         self.d_ffn = d_ffn
-        self.n_kernels = n_kernels
+        self.moving_avg_window_size = moving_avg_window_size
         self.dropout = dropout
-        self.apply_nonstationary_norm = apply_nonstationary_norm
+        self.version = version
+        self.modes = modes
+        self.mode_select = mode_select
+        self.ORT_weight = ORT_weight
+        self.MIT_weight = MIT_weight
 
         # set up the model
-        self.model = _TimesNet(
-            self.n_layers,
+        self.model = _FEDformer(
             self.n_steps,
             self.n_features,
-            self.top_k,
+            self.n_layers,
             self.d_model,
+            self.n_heads,
             self.d_ffn,
-            self.n_kernels,
+            self.moving_avg_window_size,
             self.dropout,
-            self.apply_nonstationary_norm,
+            self.version,
+            self.modes,
+            self.mode_select,
+            self.ORT_weight,
+            self.MIT_weight,
         )
         self._send_model_to_given_device()
         self._print_model_size()
 
         # set up the optimizer
         self.optimizer = optimizer
         self.optimizer.init_optimizer(self.model.parameters())
@@ -197,32 +212,32 @@
 
         return inputs
 
     def fit(
         self,
         train_set: Union[dict, str],
         val_set: Optional[Union[dict, str]] = None,
-        file_type: str = "h5py",
+        file_type: str = "hdf5",
     ) -> None:
         # Step 1: wrap the input data with classes Dataset and DataLoader
-        training_set = DatasetForTimesNet(
-            train_set, return_X_ori=False, return_labels=False, file_type=file_type
+        training_set = DatasetForFEDformer(
+            train_set, return_X_ori=False, return_y=False, file_type=file_type
         )
         training_loader = DataLoader(
             training_set,
             batch_size=self.batch_size,
             shuffle=True,
             num_workers=self.num_workers,
         )
         val_loader = None
         if val_set is not None:
-            if not check_X_ori_in_val_set(val_set):
+            if not key_in_data_set("X_ori", val_set):
                 raise ValueError("val_set must contain 'X_ori' for model validation.")
-            val_set = DatasetForTimesNet(
-                val_set, return_X_ori=True, return_labels=False, file_type=file_type
+            val_set = DatasetForFEDformer(
+                val_set, return_X_ori=True, return_y=False, file_type=file_type
             )
             val_loader = DataLoader(
                 val_set,
                 batch_size=self.batch_size,
                 shuffle=False,
                 num_workers=self.num_workers,
             )
@@ -234,42 +249,46 @@
 
         # Step 3: save the model if necessary
         self._auto_save_model_if_necessary(confirm_saving=True)
 
     def predict(
         self,
         test_set: Union[dict, str],
-        file_type: str = "h5py",
+        file_type: str = "hdf5",
     ) -> dict:
         """Make predictions for the input data with the trained model.
 
         Parameters
         ----------
         test_set : dict or str
             The dataset for model validating, should be a dictionary including keys as 'X',
             or a path string locating a data file supported by PyPOTS (e.g. h5 file).
-            If it is a dict, X should be array-like of shape [n_samples, sequence length (time steps), n_features],
+            If it is a dict, X should be array-like of shape [n_samples, sequence length (n_steps), n_features],
             which is time-series data for validating, can contain missing values, and y should be array-like of shape
             [n_samples], which is classification labels of X.
             If it is a path string, the path should point to a data file, e.g. a h5 file, which contains
             key-value pairs like a dict, and it has to include keys as 'X' and 'y'.
 
-        file_type : str
+        file_type :
             The type of the given file if test_set is a path string.
 
         Returns
         -------
-        result_dict : dict,
+        file_type :
             The dictionary containing the clustering results and latent variables if necessary.
 
         """
         # Step 1: wrap the input data with classes Dataset and DataLoader
         self.model.eval()  # set the model as eval status to freeze it.
         test_set = BaseDataset(
-            test_set, return_X_ori=False, return_labels=False, file_type=file_type
+            test_set,
+            return_X_ori=False,
+            return_X_pred=False,
+            return_y=False,
+            file_type=file_type,
         )
         test_loader = DataLoader(
             test_set,
             batch_size=self.batch_size,
             shuffle=False,
             num_workers=self.num_workers,
         )
@@ -287,36 +306,29 @@
         result_dict = {
             "imputation": imputation,
         }
         return result_dict
 
     def impute(
         self,
-        X: Union[dict, str],
-        file_type="h5py",
+        test_set: Union[dict, str],
+        file_type: str = "hdf5",
     ) -> np.ndarray:
         """Impute missing values in the given data with the trained model.
 
-        Warnings
-        --------
-        The method impute is deprecated. Please use `predict()` instead.
-
         Parameters
         ----------
-        X :
-            The data samples for testing, should be array-like of shape [n_samples, sequence length (time steps),
+        test_set :
+            The data samples for testing, should be array-like of shape [n_samples, sequence length (n_steps),
             n_features], or a path string locating a data file, e.g. h5 file.
 
         file_type :
             The type of the given file if X is a path string.
 
         Returns
         -------
-        array-like, shape [n_samples, sequence length (time steps), n_features],
+        array-like, shape [n_samples, sequence length (n_steps), n_features],
             Imputed data.
         """
-        logger.warning(
-            "🚨DeprecationWarning: The method impute is deprecated. Please use `predict` instead."
-        )
 
-        results_dict = self.predict(X, file_type=file_type)
-        return results_dict["imputation"]
+        result_dict = self.predict(test_set, file_type=file_type)
+        return result_dict["imputation"]
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pypots-0.4.1/pypots/imputation/transformer/__init__.py` & `pypots-0.5/pypots/imputation/transformer/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,14 +9,17 @@
 <https://proceedings.neurips.cc/paper/2017/file/3f5ee243547dee91fbd053c1c4a845aa-Paper.pdf>`_
 and
 `Wenjie Du, David Cote, and Yan Liu.
 SAITS: Self-Attention-based Imputation for Time Series.
 Expert Systems with Applications, 219:119619, 2023.
 <https://arxiv.org/pdf/2202.08516>`_
 
+Notes
+-----
+This implementation is inspired by https://github.com/WenjieDu/SAITS
 """
 
 # Created by Wenjie Du <wenjay.du@gmail.com>
 # License: BSD-3-Clause
 
 
 from .model import Transformer
```

### Comparing `pypots-0.4.1/pypots/imputation/transformer/core.py` & `pypots-0.5/pypots/imputation/transformer/core.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,77 +1,72 @@
 """
-The implementation of Transformer for the partially-observed time-series imputation task.
-
-Refer to the paper "Du, W., Cote, D., & Liu, Y. (2023). SAITS: Self-Attention-based Imputation for Time Series.
-Expert systems with applications."
-
-Notes
------
-Partial implementation uses code from https://github.com/WenjieDu/SAITS.
+The core wrapper assembles the submodules of Transformer imputation model
+and takes over the forward progress of the algorithm.
 
 """
 
 # Created by Wenjie Du <wenjay.du@gmail.com>
 # License: BSD-3-Clause
 
-import torch
 import torch.nn as nn
 
-from ...nn.modules.saits import SaitsLoss
-from ...nn.modules.transformer import TransformerEncoder, PositionalEncoding
+from ...nn.modules.saits import SaitsLoss, SaitsEmbedding
+from ...nn.modules.transformer import TransformerEncoder
 
 
 class _Transformer(nn.Module):
     def __init__(
         self,
         n_steps: int,
         n_features: int,
         n_layers: int,
         d_model: int,
-        d_ffn: int,
         n_heads: int,
         d_k: int,
         d_v: int,
+        d_ffn: int,
         dropout: float,
         attn_dropout: float,
         ORT_weight: float = 1,
         MIT_weight: float = 1,
     ):
         super().__init__()
         self.n_layers = n_layers
         self.ORT_weight = ORT_weight
         self.MIT_weight = MIT_weight
 
-        self.embedding = nn.Linear(n_features * 2, d_model)
-        self.dropout = nn.Dropout(dropout)
-        self.position_enc = PositionalEncoding(d_model, n_positions=n_steps)
+        self.saits_embedding = SaitsEmbedding(
+            n_features * 2,
+            d_model,
+            with_pos=True,
+            n_max_steps=n_steps,
+            dropout=dropout,
+        )
         self.encoder = TransformerEncoder(
             n_layers,
             d_model,
-            d_ffn,
             n_heads,
             d_k,
             d_v,
+            d_ffn,
             dropout,
             attn_dropout,
         )
         self.output_projection = nn.Linear(d_model, n_features)
 
         # apply SAITS loss function to Transformer on the imputation task
         self.saits_loss_func = SaitsLoss(ORT_weight, MIT_weight)
 
     def forward(self, inputs: dict, training: bool = True) -> dict:
         X, missing_mask = inputs["X"], inputs["missing_mask"]
 
         # apply the SAITS embedding strategy, concatenate X and missing mask for input
-        input_X = torch.cat([X, missing_mask], dim=2)
+        input_X = self.saits_embedding(X, missing_mask)
 
         # Transformer encoder processing
-        input_X = self.embedding(input_X)
-        input_X = self.dropout(self.position_enc(input_X))
         enc_output, _ = self.encoder(input_X)
         # project the representation from the d_model-dimensional space to the original data space for output
         reconstruction = self.output_projection(enc_output)
 
         # replace the observed part with values from X
         imputed_data = missing_mask * X + (1 - missing_mask) * reconstruction
```

### Comparing `pypots-0.4.1/pypots/imputation/transformer/model.py` & `pypots-0.5/pypots/imputation/transformer/model.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,34 +1,26 @@
 """
 The implementation of Transformer for the partially-observed time-series imputation task.
 
-Refer to the paper "Wenjie Du, David Cote, and Yan Liu.
-SAITS: Self-Attention-based Imputation for Time Series.
-Expert Systems with Applications, 219:119619, 2023."
-
-Notes
------
-Partial implementation uses code from https://github.com/WenjieDu/SAITS.
-
 """
 
 # Created by Wenjie Du <wenjay.du@gmail.com>
 # License: BSD-3-Clause
 
 from typing import Union, Optional
 
 import numpy as np
 import torch
 from torch.utils.data import DataLoader
 
 from .core import _Transformer
 from .data import DatasetForTransformer
 from ..base import BaseNNImputer
-from ...data.base import BaseDataset
-from ...data.checking import check_X_ori_in_val_set
+from ...data.dataset import BaseDataset
+from ...data.checking import key_in_data_set
 from ...optim.adam import Adam
 from ...optim.base import Optimizer
 from ...utils.logging import logger
 
 
 class Transformer(BaseNNImputer):
     """The PyTorch implementation of the Transformer model.
@@ -47,30 +39,30 @@
     n_layers :
         The number of layers in the 1st and 2nd DMSA blocks in the SAITS model.
 
     d_model :
         The dimension of the model's backbone.
         It is the input dimension of the multi-head self-attention layers.
 
-    d_ffn :
-        The dimension of the layer in the Feed-Forward Networks (FFN).
-
     n_heads :
         The number of heads in the multi-head self-attention mechanism.
         ``d_model`` must be divisible by ``n_heads``, and the result should be equal to ``d_k``.
 
     d_k :
         The dimension of the `keys` (K) and the `queries` (Q) in the DMSA mechanism.
         ``d_k`` should be the result of ``d_model`` divided by ``n_heads``. Although ``d_k`` can be directly calculated
         with given ``d_model`` and ``n_heads``, we want it be explicitly given together with ``d_v`` by users to ensure
         users be aware of them and to avoid any potential mistakes.
 
     d_v :
         The dimension of the `values` (V) in the DMSA mechanism.
 
+    d_ffn :
+        The dimension of the layer in the Feed-Forward Networks (FFN).
+
     dropout :
         The dropout rate for all fully-connected layers in the model.
 
     attn_dropout :
         The dropout rate for DMSA.
 
     ORT_weight :
@@ -122,18 +114,18 @@
 
     def __init__(
         self,
         n_steps: int,
         n_features: int,
         n_layers: int,
         d_model: int,
-        d_ffn: int,
         n_heads: int,
         d_k: int,
         d_v: int,
+        d_ffn: int,
         dropout: float = 0,
         attn_dropout: float = 0,
         ORT_weight: int = 1,
         MIT_weight: int = 1,
         batch_size: int = 32,
         epochs: int = 100,
         patience: Optional[int] = None,
@@ -179,18 +171,18 @@
 
         # set up the model
         self.model = _Transformer(
             self.n_steps,
             self.n_features,
             self.n_layers,
             self.d_model,
-            self.d_ffn,
             self.n_heads,
             self.d_k,
             self.d_v,
+            self.d_ffn,
             self.dropout,
             self.attn_dropout,
             self.ORT_weight,
             self.MIT_weight,
         )
         self._send_model_to_given_device()
         self._print_model_size()
@@ -230,32 +222,32 @@
 
         return inputs
 
     def fit(
         self,
         train_set: Union[dict, str],
         val_set: Optional[Union[dict, str]] = None,
-        file_type: str = "h5py",
+        file_type: str = "hdf5",
     ) -> None:
         # Step 1: wrap the input data with classes Dataset and DataLoader
         training_set = DatasetForTransformer(
-            train_set, return_X_ori=False, return_labels=False, file_type=file_type
+            train_set, return_X_ori=False, return_y=False, file_type=file_type
         )
         training_loader = DataLoader(
             training_set,
             batch_size=self.batch_size,
             shuffle=True,
             num_workers=self.num_workers,
         )
         val_loader = None
         if val_set is not None:
-            if not check_X_ori_in_val_set(val_set):
+            if not key_in_data_set("X_ori", val_set):
                 raise ValueError("val_set must contain 'X_ori' for model validation.")
             val_set = DatasetForTransformer(
-                val_set, return_X_ori=True, return_labels=False, file_type=file_type
+                val_set, return_X_ori=True, return_y=False, file_type=file_type
             )
             val_loader = DataLoader(
                 val_set,
                 batch_size=self.batch_size,
                 shuffle=False,
                 num_workers=self.num_workers,
             )
@@ -267,19 +259,23 @@
 
         # Step 3: save the model if necessary
         self._auto_save_model_if_necessary(confirm_saving=True)
 
     def predict(
         self,
         test_set: Union[dict, str],
-        file_type: str = "h5py",
+        file_type: str = "hdf5",
     ) -> dict:
         self.model.eval()  # set the model as eval status to freeze it.
         test_set = BaseDataset(
-            test_set, return_X_ori=False, return_labels=False, file_type=file_type
+            test_set,
+            return_X_ori=False,
+            return_X_pred=False,
+            return_y=False,
+            file_type=file_type,
         )
         test_loader = DataLoader(
             test_set,
             batch_size=self.batch_size,
             shuffle=False,
             num_workers=self.num_workers,
         )
@@ -296,35 +292,29 @@
         result_dict = {
             "imputation": imputation,
         }
         return result_dict
 
     def impute(
         self,
-        X: Union[dict, str],
-        file_type="h5py",
+        test_set: Union[dict, str],
+        file_type: str = "hdf5",
     ) -> np.ndarray:
         """Impute missing values in the given data with the trained model.
 
-        Warnings
-        --------
-        The method impute is deprecated. Please use `predict()` instead.
-
         Parameters
         ----------
-        X :
-            The data samples for testing, should be array-like of shape [n_samples, sequence length (time steps),
+        test_set :
+            The data samples for testing, should be array-like of shape [n_samples, sequence length (n_steps),
             n_features], or a path string locating a data file, e.g. h5 file.
 
         file_type :
             The type of the given file if X is a path string.
 
         Returns
         -------
-        array-like, shape [n_samples, sequence length (time steps), n_features],
+        array-like, shape [n_samples, sequence length (n_steps), n_features],
             Imputed data.
         """
-        logger.warning(
-            "🚨DeprecationWarning: The method impute is deprecated. Please use `predict` instead."
-        )
-        results_dict = self.predict(X, file_type=file_type)
-        return results_dict["imputation"]
+
+        result_dict = self.predict(test_set, file_type=file_type)
+        return result_dict["imputation"]
```

### Comparing `pypots-0.4.1/pypots/imputation/usgan/core.py` & `pypots-0.5/pypots/imputation/usgan/core.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,10 @@
 """
-The implementation of USGAN for the partially-observed time-series imputation task.
-
-Refer to the paper "Miao, X., Wu, Y., Wang, J., Gao, Y., Mao, X., & Yin, J. (2021).
-Generative Semi-supervised Learning for Multivariate Time Series Imputation. AAAI 2021."
-
+The core wrapper assembles the submodules of USGAN imputation model
+and takes over the forward progress of the algorithm.
 """
 
 # Created by Jun Wang <jwangfx@connect.ust.hk> and Wenjie Du <wenjay.du@gmail.com>
 # License: BSD-3-Clause
 
 import torch.nn as nn
```

### Comparing `pypots-0.4.1/pypots/imputation/usgan/data.py` & `pypots-0.5/pypots/classification/brits/data.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,47 +1,53 @@
 """
-Dataset class for model USGAN.
+Dataset class for the classification model BRITS.
 """
 
-# Created by Jun Wang <jwangfx@connect.ust.hk> and Wenjie Du <wenjay.du@gmail.com>
+# Created by Wenjie Du <wenjay.du@gmail.com>
 # License: BSD-3-Clause
 
 from typing import Union
 
-from ..brits.data import DatasetForBRITS
+from ...imputation.brits.data import (
+    DatasetForBRITS as DatasetForBRITS_Imputation,
+)
 
 
-class DatasetForUSGAN(DatasetForBRITS):
-    """Dataset class for USGAN, the same with the one for BRITS.
+class DatasetForBRITS(DatasetForBRITS_Imputation):
+    """Dataset class for BRITS.
 
     Parameters
     ----------
-    data : dict or str,
+    data :
         The dataset for model input, should be a dictionary including keys as 'X' and 'y',
         or a path string locating a data file.
-        If it is a dict, X should be array-like of shape [n_samples, sequence length (time steps), n_features],
+        If it is a dict, X should be array-like of shape [n_samples, sequence length (n_steps), n_features],
         which is time-series data for input, can contain missing values, and y should be array-like of shape
         [n_samples], which is classification labels of X.
         If it is a path string, the path should point to a data file, e.g. a h5 file, which contains
         key-value pairs like a dict, and it has to include keys as 'X' and 'y'.
 
-    return_labels : bool, default = True,
+    return_y :
         Whether to return labels in function __getitem__() if they exist in the given data. If `True`, for example,
         during training of classification models, the Dataset class will return labels in __getitem__() for model input.
         Otherwise, labels won't be included in the data returned by __getitem__(). This parameter exists because we
         need the defined Dataset class for all training/validating/testing stages. For those big datasets stored in h5
         files, they already have both X and y saved. But we don't read labels from the file for validating and testing
         with function _fetch_data_from_file(), which works for all three stages. Therefore, we need this parameter for
         distinction.
 
-    file_type : str, default = "h5py"
+    file_type :
         The type of the given file if train_set and val_set are path strings.
     """
 
     def __init__(
         self,
         data: Union[dict, str],
-        return_X_ori: bool,
-        return_labels: bool,
-        file_type: str = "h5py",
+        return_y: bool = True,
+        file_type: str = "hdf5",
     ):
-        super().__init__(data, return_X_ori, return_labels, file_type)
+        super().__init__(
+            data=data,
+            return_X_ori=False,
+            return_y=return_y,
+            file_type=file_type,
+        )
```

### Comparing `pypots-0.4.1/pypots/imputation/usgan/model.py` & `pypots-0.5/pypots/imputation/usgan/model.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,10 @@
 """
 The implementation of USGAN for the partially-observed time-series imputation task.
 
-Refer to the paper "Xiaoye Miao, Yangyang Wu, Jun Wang, Yunjun Gao, Xudong Mao, and Jianwei Yin.
-Generative Semi-supervised Learning for Multivariate Time Series Imputation.
-In AAAI, 35(10):8983–8991, May 2021."
-
 """
 
 # Created by Jun Wang <jwangfx@connect.ust.hk> and Wenjie Du <wenjay.du@gmail.com>
 # License: BSD-3-Clause
 
 import os
 from typing import Union, Optional
@@ -16,15 +12,15 @@
 import numpy as np
 import torch
 from torch.utils.data import DataLoader
 
 from .core import _USGAN
 from .data import DatasetForUSGAN
 from ..base import BaseNNImputer
-from ...data.checking import check_X_ori_in_val_set
+from ...data.checking import key_in_data_set
 from ...optim.adam import Adam
 from ...optim.base import Optimizer
 from ...utils.logging import logger
 from ...utils.metrics import calc_mse
 
 try:
     import nni
@@ -371,32 +367,32 @@
             f"Finished training. The best model is from epoch#{self.best_epoch}."
         )
 
     def fit(
         self,
         train_set: Union[dict, str],
         val_set: Optional[Union[dict, str]] = None,
-        file_type: str = "h5py",
+        file_type: str = "hdf5",
     ) -> None:
         # Step 1: wrap the input data with classes Dataset and DataLoader
         training_set = DatasetForUSGAN(
-            train_set, return_X_ori=False, return_labels=False, file_type=file_type
+            train_set, return_X_ori=False, return_y=False, file_type=file_type
         )
         training_loader = DataLoader(
             training_set,
             batch_size=self.batch_size,
             shuffle=True,
             num_workers=self.num_workers,
         )
         val_loader = None
         if val_set is not None:
-            if not check_X_ori_in_val_set(val_set):
+            if not key_in_data_set("X_ori", val_set):
                 raise ValueError("val_set must contain 'X_ori' for model validation.")
             val_set = DatasetForUSGAN(
-                val_set, return_X_ori=True, return_labels=False, file_type=file_type
+                val_set, return_X_ori=True, return_y=False, file_type=file_type
             )
             val_loader = DataLoader(
                 val_set,
                 batch_size=self.batch_size,
                 shuffle=False,
                 num_workers=self.num_workers,
             )
@@ -408,19 +404,19 @@
 
         # Step 3: save the model if necessary
         self._auto_save_model_if_necessary(confirm_saving=True)
 
     def predict(
         self,
         test_set: Union[dict, str],
-        file_type="h5py",
+        file_type: str = "hdf5",
     ) -> dict:
         self.model.eval()  # set the model as eval status to freeze it.
         test_set = DatasetForUSGAN(
-            test_set, return_X_ori=False, return_labels=False, file_type=file_type
+            test_set, return_X_ori=False, return_y=False, file_type=file_type
         )
         test_loader = DataLoader(
             test_set,
             batch_size=self.batch_size,
             shuffle=False,
             num_workers=self.num_workers,
         )
@@ -437,35 +433,29 @@
         result_dict = {
             "imputation": imputation,
         }
         return result_dict
 
     def impute(
         self,
-        X: Union[dict, str],
-        file_type="h5py",
+        test_set: Union[dict, str],
+        file_type: str = "hdf5",
     ) -> np.ndarray:
         """Impute missing values in the given data with the trained model.
 
-        Warnings
-        --------
-        The method impute is deprecated. Please use `predict()` instead.
-
         Parameters
         ----------
-        X :
-            The data samples for testing, should be array-like of shape [n_samples, sequence length (time steps),
+        test_set :
+            The data samples for testing, should be array-like of shape [n_samples, sequence length (n_steps),
             n_features], or a path string locating a data file, e.g. h5 file.
 
         file_type :
             The type of the given file if X is a path string.
 
         Returns
         -------
-        array-like, shape [n_samples, sequence length (time steps), n_features],
+        array-like, shape [n_samples, sequence length (n_steps), n_features],
             Imputed data.
         """
-        logger.warning(
-            "🚨DeprecationWarning: The method impute is deprecated. Please use `predict` instead."
-        )
-        results_dict = self.predict(X, file_type=file_type)
-        return results_dict["imputation"]
+
+        result_dict = self.predict(test_set, file_type=file_type)
+        return result_dict["imputation"]
```

### Comparing `pypots-0.4.1/pypots/nn/functional/normalization.py` & `pypots-0.5/pypots/nn/functional/normalization.py`

 * *Files identical despite different names*

### Comparing `pypots-0.4.1/pypots/nn/modules/autoformer/auto_encoder.py` & `pypots-0.5/pypots/nn/modules/autoformer/autoencoder.py`

 * *Files 15% similar despite different names*

```diff
@@ -7,42 +7,38 @@
 
 import torch.nn as nn
 
 from .layers import (
     SeasonalLayerNorm,
     AutoformerEncoderLayer,
     AutoCorrelation,
-    AutoCorrelationLayer,
 )
-from ..informer.auto_encoder import InformerEncoder
+from ..informer.autoencoder import InformerEncoder
 
 
 class AutoformerEncoder(nn.Module):
     def __init__(
         self,
         n_layers,
-        n_heads,
         d_model,
+        n_heads,
         d_ffn,
         factor,
         moving_avg_window_size,
         dropout,
         activation="relu",
     ):
         super().__init__()
 
         self.encoder = InformerEncoder(
             [
                 AutoformerEncoderLayer(
-                    AutoCorrelationLayer(
-                        AutoCorrelation(factor, dropout),
-                        d_model,
-                        n_heads,
-                    ),
+                    AutoCorrelation(factor, dropout),
                     d_model,
+                    n_heads,
                     d_ffn,
                     moving_avg_window_size,
                     dropout,
                     activation,
                 )
                 for _ in range(n_layers)
             ],
```

### Comparing `pypots-0.4.1/pypots/nn/modules/autoformer/layers.py` & `pypots-0.5/pypots/nn/modules/autoformer/layers.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,22 +2,25 @@
 
 """
 
 # Created by Wenjie Du <wenjay.du@gmail.com>
 # License: BSD-3-Clause
 
 import math
+from typing import Tuple, Optional
 
 import torch
 import torch.fft
 import torch.nn as nn
 import torch.nn.functional as F
 
+from ..transformer.attention import AttentionOperator, MultiHeadAttention
 
-class AutoCorrelation(nn.Module):
+
+class AutoCorrelation(AttentionOperator):
     """
     AutoCorrelation Mechanism with the following two phases:
         (1) period-based dependencies discovery
         (2) time delay aggregation
 
     This block can replace the self-attention family mechanism seamlessly.
     """
@@ -128,71 +131,54 @@
         delays_agg = torch.zeros_like(values).float()
         for i in range(top_k):
             tmp_delay = init_index + delay[..., i].unsqueeze(-1)
             pattern = torch.gather(tmp_values, dim=-1, index=tmp_delay)
             delays_agg = delays_agg + pattern * (tmp_corr[..., i].unsqueeze(-1))
         return delays_agg
 
-    def forward(self, queries, keys, values, attn_mask):
-        B, L, H, E = queries.shape
-        _, S, _, D = values.shape
+    def forward(
+        self,
+        q: torch.Tensor,
+        k: torch.Tensor,
+        v: torch.Tensor,
+        attn_mask: Optional[torch.Tensor] = None,
+        **kwargs,
+    ) -> Tuple[torch.Tensor, torch.Tensor]:
+        # q, k, v all have 4 dimensions [batch_size, n_steps, n_heads, d_tensor]
+        # d_tensor could be d_q, d_k, d_v
+
+        B, L, H, E = q.shape
+        _, S, _, D = v.shape
         if L > S:
-            zeros = torch.zeros_like(queries[:, : (L - S), :]).float()
-            values = torch.cat([values, zeros], dim=1)
-            keys = torch.cat([keys, zeros], dim=1)
+            zeros = torch.zeros_like(q[:, : (L - S), :]).float()
+            v = torch.cat([v, zeros], dim=1)
+            k = torch.cat([k, zeros], dim=1)
         else:
-            values = values[:, :L, :, :]
-            keys = keys[:, :L, :, :]
+            v = v[:, :L, :, :]
+            k = k[:, :L, :, :]
 
         # period-based dependencies
-        q_fft = torch.fft.rfft(queries.permute(0, 2, 3, 1).contiguous(), dim=-1)
-        k_fft = torch.fft.rfft(keys.permute(0, 2, 3, 1).contiguous(), dim=-1)
+        q_fft = torch.fft.rfft(q.permute(0, 2, 3, 1).contiguous(), dim=-1)
+        k_fft = torch.fft.rfft(k.permute(0, 2, 3, 1).contiguous(), dim=-1)
         res = q_fft * torch.conj(k_fft)
         corr = torch.fft.irfft(res, dim=-1)
 
         # time delay agg
         if self.training:
             V = self.time_delay_agg_training(
-                values.permute(0, 2, 3, 1).contiguous(), corr
+                v.permute(0, 2, 3, 1).contiguous(), corr
             ).permute(0, 3, 1, 2)
         else:
             V = self.time_delay_agg_inference(
-                values.permute(0, 2, 3, 1).contiguous(), corr
+                v.permute(0, 2, 3, 1).contiguous(), corr
             ).permute(0, 3, 1, 2)
 
-        return V.contiguous(), corr.permute(0, 3, 1, 2)
-
-
-class AutoCorrelationLayer(nn.Module):
-    def __init__(self, correlation, d_model, n_heads, d_keys=None, d_values=None):
-        super().__init__()
-
-        d_keys = d_keys or (d_model // n_heads)
-        d_values = d_values or (d_model // n_heads)
-
-        self.inner_correlation = correlation
-        self.query_projection = nn.Linear(d_model, d_keys * n_heads)
-        self.key_projection = nn.Linear(d_model, d_keys * n_heads)
-        self.value_projection = nn.Linear(d_model, d_values * n_heads)
-        self.out_projection = nn.Linear(d_values * n_heads, d_model)
-        self.n_heads = n_heads
-
-    def forward(self, queries, keys, values, attn_mask):
-        B, L, _ = queries.shape
-        _, S, _ = keys.shape
-        H = self.n_heads
-
-        queries = self.query_projection(queries).view(B, L, H, -1)
-        keys = self.key_projection(keys).view(B, S, H, -1)
-        values = self.value_projection(values).view(B, S, H, -1)
-
-        out, attn = self.inner_correlation(queries, keys, values, attn_mask)
-        out = out.view(B, L, -1)
-
-        return self.out_projection(out), attn
+        attn = corr.permute(0, 3, 1, 2)
+        output = V.contiguous()
+        return output, attn
 
 
 class SeasonalLayerNorm(nn.Module):
     """A special designed layer normalization for the seasonal part."""
 
     def __init__(self, n_channels):
         super().__init__()
@@ -240,29 +226,36 @@
 
 
 class AutoformerEncoderLayer(nn.Module):
     """Autoformer encoder layer with the progressive decomposition architecture."""
 
     def __init__(
         self,
-        attention,
-        d_model,
-        d_ff=None,
-        moving_avg=25,
-        dropout=0.1,
+        attn_opt: AttentionOperator,
+        d_model: int,
+        n_heads: int,
+        d_ffn: int,
+        moving_avg: int = 25,
+        dropout: float = 0.1,
         activation="relu",
     ):
         super().__init__()
-        d_ff = d_ff or 4 * d_model
-        self.attention = attention
+        d_ffn = d_ffn or 4 * d_model
+        self.attention = MultiHeadAttention(
+            attn_opt,
+            d_model,
+            n_heads,
+            d_model // n_heads,
+            d_model // n_heads,
+        )
         self.conv1 = nn.Conv1d(
-            in_channels=d_model, out_channels=d_ff, kernel_size=1, bias=False
+            in_channels=d_model, out_channels=d_ffn, kernel_size=1, bias=False
         )
         self.conv2 = nn.Conv1d(
-            in_channels=d_ff, out_channels=d_model, kernel_size=1, bias=False
+            in_channels=d_ffn, out_channels=d_model, kernel_size=1, bias=False
         )
         self.series_decomp1 = SeriesDecompositionBlock(moving_avg)
         self.series_decomp2 = SeriesDecompositionBlock(moving_avg)
         self.dropout = nn.Dropout(dropout)
         self.activation = F.relu if activation == "relu" else F.gelu
 
     def forward(self, x, attn_mask=None):
@@ -279,40 +272,53 @@
 class AutoformerDecoderLayer(nn.Module):
     """
     Autoformer decoder layer with the progressive decomposition architecture
     """
 
     def __init__(
         self,
-        self_attention,
-        cross_attention,
+        self_attn_opt,
+        cross_attn_opt,
         d_model,
-        c_out,
+        n_heads,
+        d_out,
         d_ff=None,
         moving_avg=25,
         dropout=0.1,
         activation="relu",
     ):
         super().__init__()
         d_ff = d_ff or 4 * d_model
-        self.self_attention = self_attention
-        self.cross_attention = cross_attention
+        self.self_attention = MultiHeadAttention(
+            self_attn_opt,
+            d_model,
+            n_heads,
+            d_model // n_heads,
+            d_model // n_heads,
+        )
+        self.cross_attention = MultiHeadAttention(
+            cross_attn_opt,
+            d_model,
+            n_heads,
+            d_model // n_heads,
+            d_model // n_heads,
+        )
         self.conv1 = nn.Conv1d(
             in_channels=d_model, out_channels=d_ff, kernel_size=1, bias=False
         )
         self.conv2 = nn.Conv1d(
             in_channels=d_ff, out_channels=d_model, kernel_size=1, bias=False
         )
         self.series_decomp1 = SeriesDecompositionBlock(moving_avg)
         self.series_decomp2 = SeriesDecompositionBlock(moving_avg)
         self.series_decomp3 = SeriesDecompositionBlock(moving_avg)
         self.dropout = nn.Dropout(dropout)
         self.projection = nn.Conv1d(
             in_channels=d_model,
-            out_channels=c_out,
+            out_channels=d_out,
             kernel_size=3,
             stride=1,
             padding=1,
             padding_mode="circular",
             bias=False,
         )
         self.activation = F.relu if activation == "relu" else F.gelu
```

### Comparing `pypots-0.4.1/pypots/nn/modules/brits/__init__.py` & `pypots-0.5/pypots/nn/modules/brits/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -3,14 +3,19 @@
 
 Refer to the paper
 `Wei Cao, Dong Wang, Jian Li, Hao Zhou, Lei Li, and Yitan Li.
 BRITS: Bidirectional recurrent imputation for time series.
 In Advances in Neural Information Processing Systems, volume 31. Curran Associates, Inc., 2018.
 <https://papers.nips.cc/paper_files/paper/2018/file/734e6bfcd358e25ac1db0a4241b95651-Paper.pdf>`_
 
+Notes
+-----
+This implementation is inspired by the official one https://github.com/caow13/BRITS
+The bugs in the original implementation are fixed here.
+
 """
 
 # Created by Wenjie Du <wenjay.du@gmail.com>
 # License: BSD-3-Clause
 
 from .backbone import BackboneRITS, BackboneBRITS
 from .layers import FeatureRegression
```

### Comparing `pypots-0.4.1/pypots/nn/modules/brits/backbone.py` & `pypots-0.5/pypots/nn/modules/brits/backbone.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,8 @@
 """
-The implementation of BRITS for the partially-observed time-series imputation task.
-
-Refer to the paper "Cao, W., Wang, D., Li, J., Zhou, H., Li, L., & Li, Y. (2018).
-BRITS: Bidirectional Recurrent Imputation for Time Series. NeurIPS 2018."
-
-Notes
------
-Partial implementation uses code from https://github.com/caow13/BRITS. The bugs in the original implementation
-are fixed here.
 
 """
 
 # Created by Wenjie Du <wenjay.du@gmail.com>
 # License: BSD-3-Clause
 
 from typing import Tuple
```

### Comparing `pypots-0.4.1/pypots/nn/modules/brits/layers.py` & `pypots-0.5/pypots/nn/modules/grud/layers.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,78 +1,78 @@
-"""
-The implementation of the modules for BRITS.
-
-Refer to the paper "Cao, W., Wang, D., Li, J., Zhou, H., Li, L., & Li, Y. (2018).
-BRITS: Bidirectional Recurrent Imputation for Time Series. NeurIPS 2018."
-
-Notes
------
-Partial implementation uses code from https://github.com/caow13/BRITS. The bugs in the original implementation
-are fixed here.
-
-"""
-
-# Created by Wenjie Du <wenjay.du@gmail.com>
-# License: BSD-3-Clause
-
 import math
 
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 from torch.autograd import Variable
 from torch.nn.parameter import Parameter
 
 
-class FeatureRegression(nn.Module):
-    """The module used to capture the correlation between features for imputation in BRITS.
+class TemporalDecay(nn.Module):
+    """The module used to generate the temporal decay factor gamma in the GRU-D model.
+    Please refer to the original paper :cite:`che2018GRUD` for more details.
 
     Attributes
     ----------
-    W : tensor
+    W: tensor,
         The weights (parameters) of the module.
-
-    b : tensor
+    b: tensor,
         The bias of the module.
 
-    m (buffer) : tensor
-        The mask matrix, a squire matrix with diagonal entries all zeroes while left parts all ones.
-        It is applied to the weight matrix to mask out the estimation contributions from features themselves.
-        It is used to help enhance the imputation performance of the network.
-
     Parameters
     ----------
-    input_size : the feature dimension of the input
+    input_size : int,
+        the feature dimension of the input
+
+    output_size : int,
+        the feature dimension of the output
+
+    diag : bool,
+        whether to product the weight with an identity matrix before forward processing
+
+    References
+    ----------
+    .. [1] `Che, Zhengping, Sanjay Purushotham, Kyunghyun Cho, David Sontag, and Yan Liu.
+        "Recurrent neural networks for multivariate time series with missing values."
+        Scientific reports 8, no. 1 (2018): 6085.
+        <https://www.nature.com/articles/s41598-018-24271-9.pdf>`_
+
     """
 
-    def __init__(self, input_size: int):
+    def __init__(self, input_size: int, output_size: int, diag: bool = False):
         super().__init__()
-        self.W = Parameter(torch.Tensor(input_size, input_size))
-        self.b = Parameter(torch.Tensor(input_size))
-
-        m = torch.ones(input_size, input_size) - torch.eye(input_size, input_size)
-        self.register_buffer("m", m)
+        self.diag = diag
+        self.W = Parameter(torch.Tensor(output_size, input_size))
+        self.b = Parameter(torch.Tensor(output_size))
+
+        if self.diag:
+            assert input_size == output_size
+            m = torch.eye(input_size, input_size)
+            self.register_buffer("m", m)
 
         self._reset_parameters()
 
     def _reset_parameters(self) -> None:
         std_dev = 1.0 / math.sqrt(self.W.size(0))
         self.W.data.uniform_(-std_dev, std_dev)
         if self.b is not None:
             self.b.data.uniform_(-std_dev, std_dev)
 
-    def forward(self, x: torch.Tensor) -> torch.Tensor:
-        """Forward processing of the NN module.
+    def forward(self, delta: torch.Tensor) -> torch.Tensor:
+        """Forward processing of this NN module.
 
         Parameters
         ----------
-        x : tensor,
-            the input for processing
+        delta : tensor, shape [n_samples, n_steps, n_features]
+            The time gaps.
 
         Returns
         -------
-        output: tensor,
-            the processed result containing imputation from feature regression
-
+        gamma : tensor, of the same shape with parameter `delta`, values in (0,1]
+            The temporal decay factor.
         """
-        output = F.linear(x, self.W * Variable(self.m), self.b)
-        return output
+        if self.diag:
+            gamma = F.relu(F.linear(delta, self.W * Variable(self.m), self.b))
+        else:
+            gamma = F.relu(F.linear(delta, self.W, self.b))
+        gamma = torch.exp(-gamma)
+        return gamma
```

### Comparing `pypots-0.4.1/pypots/nn/modules/crli/backbone.py` & `pypots-0.5/pypots/nn/modules/crli/backbone.py`

 * *Files identical despite different names*

### Comparing `pypots-0.4.1/pypots/nn/modules/crli/layers.py` & `pypots-0.5/pypots/nn/modules/crli/layers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,8 @@
 """
-The implementation of the modules for CRLI (Clustering Representation Learning on Incomplete time-series data).
-
-Refer to the paper "Ma, Q., Chen, C., Li, S., & Cottrell, G. W. (2021).
-Learning Representations for Incomplete Time Series Clustering. AAAI 2021."
 
 """
 
 # Created by Wenjie Du <wenjay.du@gmail.com>
 # License: BSD-3-Clause
 
 from typing import Tuple
```

### Comparing `pypots-0.4.1/pypots/nn/modules/crossformer/auto_encoder.py` & `pypots-0.5/pypots/nn/modules/crossformer/autoencoder.py`

 * *Files identical despite different names*

### Comparing `pypots-0.4.1/pypots/nn/modules/crossformer/layers.py` & `pypots-0.5/pypots/nn/modules/crossformer/layers.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -29,33 +29,33 @@
         d_ff=None,
         dropout=0.1,
         attn_dropout=0.1,
     ):
         super().__init__()
         d_ff = 4 * d_model if d_ff is None else d_ff
         self.time_attention = MultiHeadAttention(
-            n_heads,
+            ScaledDotProductAttention(d_k**0.5, attn_dropout),
             d_model,
+            n_heads,
             d_k,
             d_v,
-            ScaledDotProductAttention(d_k**0.5, attn_dropout),
         )
         self.dim_sender = MultiHeadAttention(
-            n_heads,
+            ScaledDotProductAttention(d_k**0.5, attn_dropout),
             d_model,
+            n_heads,
             d_k,
             d_v,
-            ScaledDotProductAttention(d_k**0.5, attn_dropout),
         )
         self.dim_receiver = MultiHeadAttention(
-            n_heads,
+            ScaledDotProductAttention(d_k**0.5, attn_dropout),
             d_model,
+            n_heads,
             d_k,
             d_v,
-            ScaledDotProductAttention(d_k**0.5, attn_dropout),
         )
         self.router = nn.Parameter(torch.randn(seg_num, factor, d_model))
 
         self.dropout = nn.Dropout(dropout)
 
         self.norm1 = nn.LayerNorm(d_model)
         self.norm2 = nn.LayerNorm(d_model)
```

### Comparing `pypots-0.4.1/pypots/nn/modules/csdi/layers.py` & `pypots-0.5/pypots/nn/modules/csdi/layers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Modules for CSDI model.
+
 """
 
 # Created by Wenjie Du <wenjay.du@gmail.com>
 # License: BSD-3-Clause
 
 import math
```

### Comparing `pypots-0.4.1/pypots/nn/modules/dlinear/backbone.py` & `pypots-0.5/pypots/nn/modules/dlinear/backbone.py`

 * *Files identical despite different names*

### Comparing `pypots-0.4.1/pypots/nn/modules/etsformer/__init__.py` & `pypots-0.5/pypots/nn/modules/etsformer/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,21 +3,25 @@
 
 Refer to the paper
 `Gerald Woo, Chenghao Liu, Doyen Sahoo, Akshat Kumar, and Steven Hoi.
 ETSformer: Exponential smoothing transformers for time-series forecasting.
 In ICLR, 2023.
 <https://openreview.net/pdf?id=5m_3whfo483>`_
 
+Notes
+-----
+This implementation is inspired by the official one https://github.com/salesforce/ETSformer
+
 """
 
 # Created by Wenjie Du <wenjay.du@gmail.com>
 # License: BSD-3-Clause
 
 
-from .auto_encoder import ETSformerEncoder, ETSformerDecoder
+from .autoencoder import ETSformerEncoder, ETSformerDecoder
 from .layers import ETSformerEncoderLayer, ETSformerDecoderLayer, Transform
 
 __all__ = [
     "ETSformerEncoder",
     "ETSformerEncoderLayer",
     "ETSformerDecoder",
     "ETSformerDecoderLayer",
```

### Comparing `pypots-0.4.1/pypots/nn/modules/etsformer/auto_encoder.py` & `pypots-0.5/pypots/nn/modules/etsformer/autoencoder.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,20 +24,20 @@
         return level, growths, seasons
 
 
 class ETSformerDecoder(nn.Module):
     def __init__(self, layers):
         super().__init__()
         self.d_model = layers[0].d_model
-        self.c_out = layers[0].c_out
+        self.d_out = layers[0].d_out
         self.pred_len = layers[0].pred_len
-        self.nhead = layers[0].nhead
+        self.n_head = layers[0].n_heads
 
         self.layers = nn.ModuleList(layers)
-        self.pred = nn.Linear(self.d_model, self.c_out)
+        self.pred = nn.Linear(self.d_model, self.d_out)
 
     def forward(self, growths, seasons):
         growth_repr = []
         season_repr = []
 
         for idx, layer in enumerate(self.layers):
             growth_horizon, season_horizon = layer(growths[idx], seasons[idx])
```

### Comparing `pypots-0.4.1/pypots/nn/modules/etsformer/layers.py` & `pypots-0.5/pypots/nn/modules/etsformer/layers.py`

 * *Files 8% similar despite different names*

```diff
@@ -105,36 +105,36 @@
 
     def forward(self, x):
         x = self.linear2(self.dropout1(self.activation(self.linear1(x))))
         return self.dropout2(x)
 
 
 class GrowthLayer(nn.Module):
-    def __init__(self, d_model, nhead, d_head=None, dropout=0.1):
+    def __init__(self, d_model, n_heads, d_head=None, dropout=0.1):
         super().__init__()
-        self.d_head = d_head or (d_model // nhead)
+        self.d_head = d_head or (d_model // n_heads)
         self.d_model = d_model
-        self.nhead = nhead
+        self.n_heads = n_heads
 
-        self.z0 = nn.Parameter(torch.randn(self.nhead, self.d_head))
-        self.in_proj = nn.Linear(self.d_model, self.d_head * self.nhead)
-        self.es = ExponentialSmoothing(self.d_head, self.nhead, dropout=dropout)
-        self.out_proj = nn.Linear(self.d_head * self.nhead, self.d_model)
+        self.z0 = nn.Parameter(torch.randn(self.n_heads, self.d_head))
+        self.in_proj = nn.Linear(self.d_model, self.d_head * self.n_heads)
+        self.es = ExponentialSmoothing(self.d_head, self.n_heads, dropout=dropout)
+        self.out_proj = nn.Linear(self.d_head * self.n_heads, self.d_model)
 
         assert (
-            self.d_head * self.nhead == self.d_model
-        ), "d_model must be divisible by nhead"
+            self.d_head * self.n_heads == self.d_model
+        ), "d_model must be divisible by n_heads"
 
     def forward(self, inputs):
         """
         :param inputs: shape: (batch, seq_len, dim)
         :return: shape: (batch, seq_len, dim)
         """
         b, t, d = inputs.shape
-        values = self.in_proj(inputs).view(b, t, self.nhead, -1)
+        values = self.in_proj(inputs).view(b, t, self.n_heads, -1)
         values = torch.cat([repeat(self.z0, "h d -> b 1 h d", b=b), values], dim=1)
         values = values[:, 1:] - values[:, :-1]
         out = self.es(values)
         out = torch.cat([repeat(self.es.v0, "1 1 h d -> b 1 h d", b=b), out], dim=1)
         out = rearrange(out, "b t h d -> b t (h d)")
         return self.out_proj(out)
 
@@ -215,40 +215,38 @@
 
 
 class ETSformerEncoderLayer(nn.Module):
     def __init__(
         self,
         d_model,
         n_heads,
-        c_out,
+        d_out,
         seq_len,
         pred_len,
         k,
-        dim_feedforward=None,
+        d_ffn=None,
         dropout=0.1,
         activation="sigmoid",
         layer_norm_eps=1e-5,
     ):
         super().__init__()
         self.d_model = d_model
-        self.nhead = n_heads
-        self.c_out = c_out
+        self.n_heads = n_heads
+        self.d_out = d_out
         self.seq_len = seq_len
         self.pred_len = pred_len
-        dim_feedforward = dim_feedforward or 4 * d_model
-        self.dim_feedforward = dim_feedforward
+        d_ffn = d_ffn or 4 * d_model
+        self.d_ffn = d_ffn
 
         self.growth_layer = GrowthLayer(d_model, n_heads, dropout=dropout)
         self.seasonal_layer = FourierLayer(d_model, pred_len, k=k)
-        self.level_layer = LevelLayer(d_model, c_out, dropout=dropout)
+        self.level_layer = LevelLayer(d_model, d_out, dropout=dropout)
 
         # Implementation of Feedforward model
-        self.ff = Feedforward(
-            d_model, dim_feedforward, dropout=dropout, activation=activation
-        )
+        self.ff = Feedforward(d_model, d_ffn, dropout=dropout, activation=activation)
         self.norm1 = nn.LayerNorm(d_model, eps=layer_norm_eps)
         self.norm2 = nn.LayerNorm(d_model, eps=layer_norm_eps)
 
         self.dropout1 = nn.Dropout(dropout)
         self.dropout2 = nn.Dropout(dropout)
 
     def forward(self, res, level, attn_mask=None):
@@ -267,47 +265,47 @@
 
     def _season_block(self, x):
         x = self.seasonal_layer(x)
         return self.dropout2(x)
 
 
 class DampingLayer(nn.Module):
-    def __init__(self, pred_len, nhead, dropout=0.1):
+    def __init__(self, pred_len, n_heads, dropout=0.1):
         super().__init__()
         self.pred_len = pred_len
-        self.nhead = nhead
-        self._damping_factor = nn.Parameter(torch.randn(1, nhead))
+        self.n_heads = n_heads
+        self._damping_factor = nn.Parameter(torch.randn(1, n_heads))
         self.dropout = nn.Dropout(dropout)
 
     def forward(self, x):
         x = repeat(x, "b 1 d -> b t d", t=self.pred_len)
         b, t, d = x.shape
 
         powers = torch.arange(self.pred_len).to(self._damping_factor.device) + 1
         powers = powers.view(self.pred_len, 1)
         damping_factors = self.damping_factor**powers
         damping_factors = damping_factors.cumsum(dim=0)
-        x = x.view(b, t, self.nhead, -1)
+        x = x.view(b, t, self.n_heads, -1)
         x = self.dropout(x) * damping_factors.unsqueeze(-1)
         return x.view(b, t, d)
 
     @property
     def damping_factor(self):
         return torch.sigmoid(self._damping_factor)
 
 
 class ETSformerDecoderLayer(nn.Module):
-    def __init__(self, d_model, nhead, c_out, pred_len, dropout=0.1):
+    def __init__(self, d_model, n_heads, d_out, pred_len, dropout=0.1):
         super().__init__()
         self.d_model = d_model
-        self.nhead = nhead
-        self.c_out = c_out
+        self.n_heads = n_heads
+        self.d_out = d_out
         self.pred_len = pred_len
 
-        self.growth_damping = DampingLayer(pred_len, nhead, dropout=dropout)
+        self.growth_damping = DampingLayer(pred_len, n_heads, dropout=dropout)
         self.dropout1 = nn.Dropout(dropout)
 
     def forward(self, growth, season):
         growth_horizon = self.growth_damping(growth[:, -1:])
         growth_horizon = self.dropout1(growth_horizon)
 
         seasonal_horizon = season[:, -self.pred_len :]
```

### Comparing `pypots-0.4.1/pypots/nn/modules/fedformer/__init__.py` & `pypots-0.5/pypots/nn/modules/fedformer/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -3,14 +3,18 @@
 
 Refer to the paper
 `Tian Zhou, Ziqing Ma, Qingsong Wen, Xue Wang, Liang Sun, and Rong Jin.
 FEDformer: Frequency enhanced decomposed transformer for long-term series forecasting.
 In ICML, volume 162 of Proceedings of Machine Learning Research, pages 27268–27286. PMLR, 17–23 Jul 2022.
 <https://proceedings.mlr.press/v162/zhou22g/zhou22g.pdf>`_
 
+Notes
+-----
+This implementation is inspired by the official one https://github.com/MAZiqing/FEDformer
+
 """
 
 # Created by Wenjie Du <wenjay.du@gmail.com>
 # License: BSD-3-Clause
 
 
 from .autoencoder import FEDformerEncoder, FEDformerDecoder
```

### Comparing `pypots-0.4.1/pypots/nn/modules/fedformer/autoencoder.py` & `pypots-0.5/pypots/nn/modules/fedformer/autoencoder.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,27 +12,26 @@
     MultiWaveletCross,
     FourierBlock,
     FourierCrossAttention,
 )
 from ....nn.modules.autoformer import (
     AutoformerEncoderLayer,
     AutoformerDecoderLayer,
-    AutoCorrelationLayer,
     SeasonalLayerNorm,
 )
 from ....nn.modules.informer import InformerEncoder, InformerDecoder
 
 
 class FEDformerEncoder(nn.Module):
     def __init__(
         self,
         n_steps,
         n_layers,
-        n_heads,
         d_model,
+        n_heads,
         d_ffn,
         moving_avg_window_size,
         dropout,
         version="Fourier",
         modes=32,
         mode_select="random",
         activation="relu",
@@ -53,20 +52,17 @@
             raise ValueError(
                 f"Unsupported version: {version}. Please choose from ['Wavelets', 'Fourier']."
             )
 
         self.encoder = InformerEncoder(
             [
                 AutoformerEncoderLayer(
-                    AutoCorrelationLayer(
-                        encoder_self_att,  # instead of multi-head attention in transformer
-                        d_model,
-                        n_heads,
-                    ),
+                    encoder_self_att,  # instead of multi-head attention in transformer
                     d_model,
+                    n_heads,
                     d_ffn,
                     moving_avg_window_size,
                     dropout,
                     activation,
                 )
                 for _ in range(n_layers)
             ],
@@ -130,17 +126,18 @@
             raise ValueError(
                 f"Unsupported version: {version}. Please choose from ['Wavelets', 'Fourier']."
             )
 
         self.decoder = InformerDecoder(
             [
                 AutoformerDecoderLayer(
-                    AutoCorrelationLayer(decoder_self_att, d_model, n_heads),
-                    AutoCorrelationLayer(decoder_cross_att, d_model, n_heads),
+                    decoder_self_att,
+                    decoder_cross_att,
                     d_model,
+                    n_heads,
                     d_output,
                     d_ffn,
                     moving_avg=moving_avg_window_size,
                     dropout=dropout,
                     activation=activation,
                 )
                 for _ in range(n_layers)
```

### Comparing `pypots-0.4.1/pypots/nn/modules/fedformer/layers.py` & `pypots-0.5/pypots/nn/modules/fedformer/layers.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,24 +3,26 @@
 """
 
 # Created by Wenjie Du <wenjay.du@gmail.com>
 # License: BSD-3-Clause
 
 import math
 from functools import partial
-from typing import List, Tuple
+from typing import List, Tuple, Optional
 
 import numpy as np
 import torch
 import torch.nn.functional as F
 from scipy.special import eval_legendre
 from sympy import Poly, legendre, Symbol, chebyshevt
 from torch import Tensor
 from torch import nn
 
+from ..transformer.attention import AttentionOperator
+
 
 def legendreDer(k, x):
     def _legendre(k, x):
         return (2 * k + 1) * eval_legendre(k, x)
 
     out = 0
     for i in np.arange(k - 1, -1, -2):
@@ -391,15 +393,15 @@
 
         x = torch.zeros(B, N * 2, c, self.k, device=x.device)
         x[..., ::2, :, :] = x_e
         x[..., 1::2, :, :] = x_o
         return x
 
 
-class MultiWaveletTransform(nn.Module):
+class MultiWaveletTransform(AttentionOperator):
     """
     1D multiwavelet block.
     """
 
     def __init__(
         self,
         ich=1,
@@ -418,35 +420,45 @@
         self.L = L
         self.nCZ = nCZ
         self.Lk0 = nn.Linear(ich, c * k)
         self.Lk1 = nn.Linear(c * k, ich)
         self.ich = ich
         self.MWT_CZ = nn.ModuleList(MWT_CZ1d(k, alpha, L, c, base) for i in range(nCZ))
 
-    def forward(self, queries, keys, values, attn_mask):
-        B, L, H, E = queries.shape
-        _, S, _, D = values.shape
+    def forward(
+        self,
+        q: torch.Tensor,
+        k: torch.Tensor,
+        v: torch.Tensor,
+        attn_mask: Optional[torch.Tensor] = None,
+        **kwargs,
+    ) -> Tuple[torch.Tensor, None]:
+        # q, k, v all have 4 dimensions [batch_size, n_steps, n_heads, d_tensor]
+        # d_tensor could be d_q, d_k, d_v
+
+        B, L, H, E = q.shape
+        _, S, _, D = v.shape
         if L > S:
-            zeros = torch.zeros_like(queries[:, : (L - S), :]).float()
-            values = torch.cat([values, zeros], dim=1)
-            keys = torch.cat([keys, zeros], dim=1)
+            zeros = torch.zeros_like(q[:, : (L - S), :]).float()
+            v = torch.cat([v, zeros], dim=1)
+            # k = torch.cat([k, zeros], dim=1)
         else:
-            values = values[:, :L, :, :]
-            keys = keys[:, :L, :, :]
-        values = values.view(B, L, -1)
+            v = v[:, :L, :, :]
+            # k = k[:, :L, :, :]
+        v = v.reshape(B, L, -1)
 
-        V = self.Lk0(values).view(B, L, self.c, -1)
+        V = self.Lk0(v).view(B, L, self.c, -1)
         for i in range(self.nCZ):
             V = self.MWT_CZ[i](V)
             if i < self.nCZ - 1:
                 V = F.relu(V)
 
         V = self.Lk1(V.view(B, L, -1))
         V = V.view(B, L, -1, D)
-        return (V.contiguous(), None)
+        return V.contiguous(), None
 
 
 class FourierCrossAttentionW(nn.Module):
     def __init__(
         self,
         in_channels,
         out_channels,
@@ -527,15 +539,15 @@
         out = torch.fft.irfft(
             out_ft / self.in_channels / self.out_channels, n=xq.size(-1)
         ).permute(0, 3, 2, 1)
         # size = [B, L, H, E]
         return (out, None)
 
 
-class MultiWaveletCross(nn.Module):
+class MultiWaveletCross(AttentionOperator):
     """
     1D Multiwavelet Cross Attention layer.
     """
 
     def __init__(
         self,
         in_channels,
@@ -550,15 +562,14 @@
         base="legendre",
         mode_select_method="random",
         initializer=None,
         activation="tanh",
         **kwargs,
     ):
         super().__init__()
-        # print("base", base)
 
         self.c = c
         self.k = k
         self.L = L
         H0, H1, G0, G1, PHI0, PHI1 = get_filter(base, k)
         H0r = H0 @ PHI0
         G0r = G0 @ PHI0
@@ -616,15 +627,25 @@
 
         self.Lk = nn.Linear(ich, c * k)
         self.Lq = nn.Linear(ich, c * k)
         self.Lv = nn.Linear(ich, c * k)
         self.out = nn.Linear(c * k, ich)
         self.modes1 = modes
 
-    def forward(self, q, k, v, mask=None):
+    def forward(
+        self,
+        q: torch.Tensor,
+        k: torch.Tensor,
+        v: torch.Tensor,
+        attn_mask: Optional[torch.Tensor] = None,
+        **kwargs,
+    ) -> Tuple[torch.Tensor, None]:
+        # q, k, v all have 4 dimensions [batch_size, n_steps, n_heads, d_tensor]
+        # d_tensor could be d_q, d_k, d_v
+
         B, N, H, E = q.shape  # (B, N, H, E) torch.Size([3, 768, 8, 2])
         _, S, _, _ = k.shape  # (B, S, H, E) torch.Size([3, 96, 8, 2])
 
         q = q.view(q.shape[0], q.shape[1], -1)
         k = k.view(k.shape[0], k.shape[1], -1)
         v = v.view(v.shape[0], v.shape[1], -1)
         q = self.Lq(q)
@@ -676,27 +697,27 @@
             Ud_v += [tuple([d, v])]
             Us_v += [d]
         for i in range(ns - self.L):
             dk, sk = Ud_k[i], Us_k[i]
             dq, sq = Ud_q[i], Us_q[i]
             dv, sv = Ud_v[i], Us_v[i]
             Ud += [
-                self.attn1(dq[0], dk[0], dv[0], mask)[0]
-                + self.attn2(dq[1], dk[1], dv[1], mask)[0]
+                self.attn1(dq[0], dk[0], dv[0], attn_mask)[0]
+                + self.attn2(dq[1], dk[1], dv[1], attn_mask)[0]
             ]
-            Us += [self.attn3(sq, sk, sv, mask)[0]]
-        v = self.attn4(q, k, v, mask)[0]
+            Us += [self.attn3(sq, sk, sv, attn_mask)[0]]
+        v = self.attn4(q, k, v, attn_mask)[0]
 
         # reconstruct
         for i in range(ns - 1 - self.L, -1, -1):
             v = v + Us[i]
             v = torch.cat((v, Ud[i]), -1)
             v = self.evenOdd(v)
         v = self.out(v[:, :N, :, :].contiguous().view(B, N, -1))
-        return (v.contiguous(), None)
+        return v.contiguous(), None
 
     def wavelet_transform(self, x):
         xa = torch.cat(
             [
                 x[:, ::2, :, :],
                 x[:, 1::2, :, :],
             ],
@@ -732,15 +753,15 @@
     else:
         index = list(range(0, modes))
     index.sort()
     return index
 
 
 # ########## fourier layer #############
-class FourierBlock(nn.Module):
+class FourierBlock(AttentionOperator):
     def __init__(
         self, in_channels, out_channels, seq_len, modes=0, mode_select_method="random"
     ):
         super().__init__()
         # print("fourier enhanced block used!")
         """
         1D Fourier block. It performs representation learning on frequency domain,
@@ -765,33 +786,42 @@
         )
 
     # Complex multiplication
     def compl_mul1d(self, input, weights):
         # (batch, in_channel, x ), (in_channel, out_channel, x) -> (batch, out_channel, x)
         return torch.einsum("bhi,hio->bho", input, weights)
 
-    def forward(self, q, k, v, mask):
-        # size = [B, L, H, E]
+    def forward(
+        self,
+        q: torch.Tensor,
+        k: torch.Tensor,
+        v: torch.Tensor,
+        attn_mask: Optional[torch.Tensor] = None,
+        **kwargs,
+    ) -> Tuple[torch.Tensor, None]:
+        # q, k, v all have 4 dimensions [batch_size, n_steps, n_heads, d_tensor]
+        # d_tensor could be d_q, d_k, d_v
+
         B, L, H, E = q.shape
         x = q.permute(0, 2, 3, 1)
         # Compute Fourier coefficients
         x_ft = torch.fft.rfft(x, dim=-1)
         # Perform Fourier neural operations
         out_ft = torch.zeros(B, H, E, L // 2 + 1, device=x.device, dtype=torch.cfloat)
         for wi, i in enumerate(self.index):
             out_ft[:, :, :, wi] = self.compl_mul1d(
                 x_ft[:, :, :, i], self.weights1[:, :, :, wi]
             )
         # Return to time domain
         x = torch.fft.irfft(out_ft, n=x.size(-1))
-        return (x, None)
+        return x, None
 
 
 # ########## Fourier Cross Former ####################
-class FourierCrossAttention(nn.Module):
+class FourierCrossAttention(AttentionOperator):
     def __init__(
         self,
         in_channels,
         out_channels,
         seq_len_q,
         seq_len_kv,
         modes=64,
@@ -859,16 +889,25 @@
                 - torch.einsum(order, x.imag, weights.imag),
                 torch.einsum(order, x.real, weights.imag)
                 + torch.einsum(order, x.imag, weights.real),
             )
         else:
             return torch.einsum(order, x.real, weights.real)
 
-    def forward(self, q, k, v, mask):
-        # size = [B, L, H, E]
+    def forward(
+        self,
+        q: torch.Tensor,
+        k: torch.Tensor,
+        v: torch.Tensor,
+        attn_mask: Optional[torch.Tensor] = None,
+        **kwargs,
+    ) -> Tuple[torch.Tensor, None]:
+        # q, k, v all have 4 dimensions [batch_size, n_steps, n_heads, d_tensor]
+        # d_tensor could be d_q, d_k, d_v
+
         B, L, H, E = q.shape
         xq = q.permute(0, 2, 3, 1)  # size = [B, H, E, L]
         xk = k.permute(0, 2, 3, 1)
         # xv = v.permute(0, 2, 3, 1)
 
         # Compute Fourier coefficients
         xq_ft_ = torch.zeros(
@@ -908,8 +947,8 @@
             if i >= xqkvw.shape[3] or j >= out_ft.shape[3]:
                 continue
             out_ft[:, :, :, j] = xqkvw[:, :, :, i]
         # Return to time domain
         out = torch.fft.irfft(
             out_ft / self.in_channels / self.out_channels, n=xq.size(-1)
         )
-        return (out, None)
+        return out, None
```

### Comparing `pypots-0.4.1/pypots/nn/modules/gpvae/__init__.py` & `pypots-0.5/pypots/nn/modules/gpvae/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -3,14 +3,18 @@
 
 Refer to the paper
 `Vincent Fortuin, Dmitry Baranchuk, Gunnar Rätsch, and Stephan Mandt.
 GP-VAE: Deep probabilistic time series imputation.
 In International conference on artificial intelligence and statistics, pages 1651–1661. PMLR, 2020.
 <http://proceedings.mlr.press/v108/fortuin20a/fortuin20a.pdf>`_
 
+Notes
+-----
+This implementation is inspired by the official one https://github.com/ratschlab/GP-VAE
+
 """
 
 # Created by Jun Wang <jwangfx@connect.ust.hk> and Wenjie Du <wenjay.du@gmail.com>
 # License: BSD-3-Clause
 
 from .backbone import BackboneGPVAE
```

### Comparing `pypots-0.4.1/pypots/nn/modules/gpvae/backbone.py` & `pypots-0.5/pypots/nn/modules/gpvae/backbone.py`

 * *Files identical despite different names*

### Comparing `pypots-0.4.1/pypots/nn/modules/gpvae/layers.py` & `pypots-0.5/pypots/nn/modules/gpvae/layers.py`

 * *Files identical despite different names*

### Comparing `pypots-0.4.1/pypots/nn/modules/grud/backbone.py` & `pypots-0.5/pypots/nn/modules/grud/backbone.py`

 * *Files identical despite different names*

### Comparing `pypots-0.4.1/pypots/nn/modules/informer/__init__.py` & `pypots-0.5/pypots/nn/modules/informer/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,21 +3,25 @@
 
 Refer to the paper
 `Haoyi Zhou, Shanghang Zhang, Jieqi Peng, Shuai Zhang, Jianxin Li, Hui Xiong, and Wancai Zhang.
 Informer: Beyond efficient transformer for long sequence time-series forecasting.
 In Proceedings of the AAAI conference on artificial intelligence, volume 35, pages 11106–11115, 2021.
 <https://ojs.aaai.org/index.php/AAAI/article/download/17325/17132>`_
 
+Notes
+-----
+This implementation is inspired by the official one https://github.com/zhouhaoyi/Informer2020
+
 """
 
 # Created by Wenjie Du <wenjay.du@gmail.com>
 # License: BSD-3-Clause
 
 
-from .auto_encoder import InformerEncoder, InformerDecoder
+from .autoencoder import InformerEncoder, InformerDecoder
 from .layers import ProbAttention, ConvLayer, InformerEncoderLayer, InformerDecoderLayer
 
 __all__ = [
     "ProbAttention",
     "ConvLayer",
     "InformerEncoderLayer",
     "InformerDecoderLayer",
```

### Comparing `pypots-0.4.1/pypots/nn/modules/informer/auto_encoder.py` & `pypots-0.5/pypots/nn/modules/informer/autoencoder.py`

 * *Files identical despite different names*

### Comparing `pypots-0.4.1/pypots/nn/modules/informer/layers.py` & `pypots-0.5/pypots/nn/modules/informer/layers.py`

 * *Files 1% similar despite different names*

```diff
@@ -130,14 +130,16 @@
         self,
         q: torch.Tensor,
         k: torch.Tensor,
         v: torch.Tensor,
         attn_mask: Optional[torch.Tensor] = None,
         **kwargs,
     ):
+        # q, k, v all have 4 dimensions [batch_size, n_steps, n_heads, d_tensor]
+        # d_tensor could be d_q, d_k, d_v
 
         B, L_Q, H, D = q.shape
         _, L_K, _, _ = k.shape
 
         q = q.transpose(2, 1)
         k = k.transpose(2, 1)
         v = v.transpose(2, 1)
```

### Comparing `pypots-0.4.1/pypots/nn/modules/mrnn/__init__.py` & `pypots-0.5/pypots/nn/modules/mrnn/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,14 +3,19 @@
 
 Refer to the paper
 `Jinsung Yoon, William R. Zame, and Mihaela van der Schaar.
 Estimating missing data in temporal data streams using multi-directional recurrent neural networks.
 IEEE Transactions on Biomedical Engineering, 66(5):14771490, 2019.
 <https://arxiv.org/pdf/1711.08742>`_
 
+Notes
+-----
+This implementation is inspired by the official one
+https://github.com/jsyoon0823/MRNN and https://github.com/WenjieDu/SAITS
+
 """
 
 # Created by Wenjie Du <wenjay.du@gmail.com>
 # License: BSD-3-Clause
 
 from .backbone import BackboneMRNN
 from .layers import MrnnFcnRegression
```

### Comparing `pypots-0.4.1/pypots/nn/modules/mrnn/backbone.py` & `pypots-0.5/pypots/nn/modules/mrnn/backbone.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 """
-PyTorch MRNN model for the time-series imputation task.
-This implementation is inspired by the official one https://github.com/jsyoon0823/MRNN.
-Some part of the code is from https://github.com/WenjieDu/SAITS.
+
 """
 
 # Created by Wenjie Du <wenjay.du@gmail.com>
 # License: BSD-3-Clause
 
 from typing import Tuple
```

### Comparing `pypots-0.4.1/pypots/nn/modules/mrnn/layers.py` & `pypots-0.5/pypots/nn/modules/mrnn/layers.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-The layers of the M-RNN model.
+
 """
 
 # Created by Wenjie Du <wenjay.du@gmail.com>
 # License: BSD-3-Clause
 
 
 import math
```

### Comparing `pypots-0.4.1/pypots/nn/modules/patchtst/__init__.py` & `pypots-0.5/pypots/nn/modules/patchtst/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,21 +3,25 @@
 
 Refer to the paper
 `Yuqi Nie, Nam H Nguyen, Phanwadee Sinthong, and Jayant Kalagnanam.
 A time series is worth 64 words: Long-term forecasting with transformers.
 In ICLR, 2023.
 <https://openreview.net/pdf?id=Jbdc0vTOcol>`_
 
+Notes
+-----
+This implementation is inspired by the official one https://github.com/yuqinie98/PatchTST
+
 """
 
 # Created by Wenjie Du <wenjay.du@gmail.com>
 # License: BSD-3-Clause
 
 
-from .auto_encoder import PatchtstEncoder
+from .autoencoder import PatchtstEncoder
 from .layers import PatchEmbedding, RegressionHead, ClassificationHead, PredictionHead
 
 __all__ = [
     "PatchtstEncoder",
     "PatchEmbedding",
     "RegressionHead",
     "ClassificationHead",
```

### Comparing `pypots-0.4.1/pypots/nn/modules/patchtst/auto_encoder.py` & `pypots-0.5/pypots/nn/modules/patchtst/autoencoder.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -10,34 +10,34 @@
 from ....nn.modules.transformer import TransformerEncoder
 
 
 class PatchtstEncoder(nn.Module):
     def __init__(
         self,
         n_layers: int,
-        n_heads: int,
         d_model: int,
-        d_ffn: int,
+        n_heads: int,
         d_k: int,
         d_v: int,
+        d_ffn: int,
         dropout: float,
         attn_dropout: float,
     ):
         super().__init__()
 
         self.n_layers = n_layers
         self.d_model = d_model
 
         self.encoder = TransformerEncoder(
             n_layers,
             d_model,
-            d_ffn,
             n_heads,
             d_k,
             d_v,
+            d_ffn,
             dropout,
             attn_dropout,
         )
 
     def forward(self, x, attn_mask=None):
 
         enc_out, attns = self.encoder(x, attn_mask)
```

### Comparing `pypots-0.4.1/pypots/nn/modules/patchtst/layers.py` & `pypots-0.5/pypots/nn/modules/patchtst/layers.py`

 * *Files identical despite different names*

### Comparing `pypots-0.4.1/pypots/nn/modules/raindrop/backbone.py` & `pypots-0.5/pypots/nn/modules/raindrop/backbone.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,67 +1,53 @@
 """
-The implementation of Raindrop for the partially-observed time-series classification task.
-
-Refer to the paper "Zhang, X., Zeman, M., Tsiligkaridis, T., & Zitnik, M. (2022).
-Graph-Guided Network for Irregularly Sampled Multivariate Time Series. ICLR 2022."
 
 """
 
 
 # Created by Wenjie Du <wenjay.du@gmail.com>
 # License: BSD-3-Clause
 
 
 from typing import Tuple
 
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 from torch.nn import TransformerEncoderLayer, TransformerEncoder
-from torch.nn.parameter import Parameter
-
-from ....utils.logging import logger
-
-try:
-    from .layers import PositionalEncoding, ObservationPropagation
-    from torch_geometric.nn.inits import glorot
-except ImportError as e:
-    logger.error(
-        f"❌ {e}\n"
-        "Note torch_geometric is missing, please install it with "
-        "'pip install torch_geometric torch_scatter torch_sparse' or "
-        "'conda install -c pyg pyg pytorch-scatter pytorch-sparse'"
-    )
-except NameError as e:
-    logger.error(
-        f"❌ {e}\n"
-        "Note torch_geometric is missing, please install it with "
-        "'pip install torch_geometric torch_scatter torch_sparse' or "
-        "'conda install -c pyg pyg pytorch-scatter pytorch-sparse'"
-    )
 
 
 class BackboneRaindrop(nn.Module):
     def __init__(
         self,
         n_features,
         n_layers,
         d_model,
-        d_ffn,
         n_heads,
+        d_ffn,
         n_classes,
         dropout=0.3,
         max_len=215,
         d_static=9,
         d_pe=16,
         aggregation="mean",
         sensor_wise_mask=False,
         static=False,
     ):
+
+        try:
+            from .layers import PositionalEncoding, ObservationPropagation
+        except (ImportError, NameError) as e:
+            raise ImportError(
+                f"❌ {e}. Note that torch_geometric is missing, please install it with "
+                "'pip install torch_geometric torch_scatter torch_sparse' or "
+                "'conda install -c pyg pyg pytorch-scatter pytorch-sparse'"
+            )
+
         super().__init__()
+
         self.n_layers = n_layers
         self.n_features = n_features
         self.d_model = d_model
         self.d_ffn = d_ffn
         self.n_heads = n_heads
         self.n_classes = n_classes
         self.dropout = dropout
@@ -91,15 +77,15 @@
             dim_check = d_model + d_pe
             assert dim_check % n_heads == 0, "dim_check must be divisible by n_heads"
             encoder_layers = TransformerEncoderLayer(
                 d_model + d_pe, n_heads, d_ffn, dropout
             )
         self.transformer_encoder = TransformerEncoder(encoder_layers, n_layers)
 
-        self.R_u = Parameter(torch.Tensor(1, self.n_features * self.d_ob))
+        self.R_u = nn.Parameter(torch.Tensor(1, self.n_features * self.d_ob))
 
         self.ob_propagation = ObservationPropagation(
             in_channels=max_len * self.d_ob,
             out_channels=max_len * self.d_ob,
             heads=1,
             n_nodes=n_features,
             ob_dim=self.d_ob,
@@ -126,23 +112,23 @@
         self.init_weights()
 
     def init_weights(self):
         init_range = 1e-10
         self.encoder.weight.data.uniform_(-init_range, init_range)
         if self.static:
             self.static_emb.weight.data.uniform_(-init_range, init_range)
-        glorot(self.R_u)
+        nn.init.xavier_uniform(self.R_u)  # xavier_uniform also known as glorot
 
     def forward(
         self,
         X: torch.Tensor,
         timestamps: torch.Tensor,
         lengths: torch.Tensor,
     ) -> Tuple[torch.Tensor, ...]:
-        """Forward processing of BRITS.
+        """Forward processing of Raindrop.
 
         Parameters
         ----------
         X :
             The input tensor of shape (batch_size, n_features, max_len).
 
         timestamps :
```

### Comparing `pypots-0.4.1/pypots/nn/modules/raindrop/layers.py` & `pypots-0.5/pypots/nn/modules/raindrop/layers.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,8 @@
 """
-The implementation of the modules for Raindrop.
-
-Refer to the paper "Zhang, X., Zeman, M., Tsiligkaridis, T., & Zitnik, M. (2022).
-Graph-Guided Network for Irregularly Sampled Multivariate Time Series. ICLR 2022."
 
 """
 
 # Created by Wenjie Du <wenjay.du@gmail.com>
 # License: BSD-3-Clause
 
 
@@ -18,30 +14,25 @@
 import torch.nn as nn
 import torch.nn.functional as F
 from torch import Tensor
 from torch.nn import Linear
 from torch.nn import init
 from torch.nn.parameter import Parameter
 
-from ....utils.logging import logger
-
 try:
     from torch_geometric.nn.conv import MessagePassing
     from torch_geometric.nn.inits import glorot
     from torch_geometric.typing import PairTensor, Adj, OptTensor
     from torch_geometric.utils import softmax
     from torch_scatter import scatter
     from torch_sparse import SparseTensor
-except ImportError as e:
-    logger.error(
-        f"❌ {e}\n"
-        "Note torch_geometric is missing, please install it with "
-        "'pip install torch_geometric torch_scatter torch_sparse' or "
-        "'conda install -c pyg pyg pytorch-scatter pytorch-sparse'"
-    )
+except ImportError:
+    # Modules here only for Raindrop model, and torch_geometric import errors are caught in BackboneRaindrop.
+    # Hence, we can pass them here.
+    pass
 
 
 class PositionalEncoding(nn.Module):
     """Generate positional encoding according to time information."""
 
     def __init__(self, d_pe: int, max_len: int = 500):
         super().__init__()
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pypots-0.4.1/pypots/nn/modules/saits/backbone.py` & `pypots-0.5/pypots/nn/modules/saits/backbone.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,120 +1,120 @@
 """
-Refer to the paper "Du, W., Cote, D., & Liu, Y. (2023). SAITS: Self-Attention-based Imputation for Time Series.
-Expert systems with applications."
-
-Notes
------
-Partial implementation uses code from https://github.com/WenjieDu/SAITS.
 
 """
 
 # Created by Wenjie Du <wenjay.du@gmail.com>
 # License: BSD-3-Clause
 
 from typing import Optional, Tuple
 
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 
+from .embedding import SaitsEmbedding
 from ..transformer import (
-    PositionalEncoding,
     TransformerEncoderLayer,
     ScaledDotProductAttention,
 )
 
 
 class BackboneSAITS(nn.Module):
     def __init__(
         self,
-        n_layers: int,
         n_steps: int,
         n_features: int,
+        n_layers: int,
         d_model: int,
-        d_ffn: int,
         n_heads: int,
         d_k: int,
         d_v: int,
+        d_ffn: int,
         dropout: float,
         attn_dropout: float,
     ):
         super().__init__()
 
         # concatenate the feature vector and missing mask, hence double the number of features
         actual_n_features = n_features * 2
 
+        # for the 1st block
+        self.embedding_1 = SaitsEmbedding(
+            actual_n_features,
+            d_model,
+            with_pos=True,
+            n_max_steps=n_steps,
+            dropout=dropout,
+        )
         self.layer_stack_for_first_block = nn.ModuleList(
             [
                 TransformerEncoderLayer(
+                    ScaledDotProductAttention(d_k**0.5, attn_dropout),
                     d_model,
-                    d_ffn,
                     n_heads,
                     d_k,
                     d_v,
-                    ScaledDotProductAttention(d_k**0.5, attn_dropout),
+                    d_ffn,
                     dropout,
                 )
                 for _ in range(n_layers)
             ]
         )
+        self.reduce_dim_z = nn.Linear(d_model, n_features)
+
+        # for the 2nd block
+        self.embedding_2 = SaitsEmbedding(
+            actual_n_features,
+            d_model,
+            with_pos=True,
+            n_max_steps=n_steps,
+            dropout=dropout,
+        )
         self.layer_stack_for_second_block = nn.ModuleList(
             [
                 TransformerEncoderLayer(
+                    ScaledDotProductAttention(d_k**0.5, attn_dropout),
                     d_model,
-                    d_ffn,
                     n_heads,
                     d_k,
                     d_v,
-                    ScaledDotProductAttention(d_k**0.5, attn_dropout),
+                    d_ffn,
                     dropout,
                 )
                 for _ in range(n_layers)
             ]
         )
 
-        self.dropout = nn.Dropout(p=dropout)
-        self.position_enc = PositionalEncoding(d_model, n_positions=n_steps)
-        # for the 1st block
-        self.embedding_1 = nn.Linear(actual_n_features, d_model)
-        self.reduce_dim_z = nn.Linear(d_model, n_features)
-        # for the 2nd block
-        self.embedding_2 = nn.Linear(actual_n_features, d_model)
         self.reduce_dim_beta = nn.Linear(d_model, n_features)
         self.reduce_dim_gamma = nn.Linear(n_features, n_features)
+
         # for delta decay factor
         self.weight_combine = nn.Linear(n_features + n_steps, n_features)
 
     def forward(
         self, X, missing_mask, attn_mask: Optional = None
     ) -> Tuple[torch.Tensor, ...]:
 
         # first DMSA block
-        input_X_for_first = torch.cat([X, missing_mask], dim=2)
-        input_X_for_first = self.embedding_1(input_X_for_first)
-        enc_output = self.dropout(
-            self.position_enc(input_X_for_first)
+        enc_output = self.embedding_1(
+            X, missing_mask
         )  # namely, term e in the math equation
         first_DMSA_attn_weights = None
         for encoder_layer in self.layer_stack_for_first_block:
             enc_output, first_DMSA_attn_weights = encoder_layer(enc_output, attn_mask)
-
         X_tilde_1 = self.reduce_dim_z(enc_output)
         X_prime = missing_mask * X + (1 - missing_mask) * X_tilde_1
 
         # second DMSA block
-        input_X_for_second = torch.cat([X_prime, missing_mask], dim=2)
-        input_X_for_second = self.embedding_2(input_X_for_second)
-        enc_output = self.position_enc(
-            input_X_for_second
+        enc_output = self.embedding_2(
+            X_prime, missing_mask
         )  # namely term alpha in math algo
         second_DMSA_attn_weights = None
         for encoder_layer in self.layer_stack_for_second_block:
             enc_output, second_DMSA_attn_weights = encoder_layer(enc_output, attn_mask)
-
         X_tilde_2 = self.reduce_dim_gamma(F.relu(self.reduce_dim_beta(enc_output)))
 
         # attention-weighted combine
         copy_second_DMSA_weights = second_DMSA_attn_weights.clone()
         copy_second_DMSA_weights = copy_second_DMSA_weights.squeeze(
             dim=1
         )  # namely term A_hat in Eq.
```

### Comparing `pypots-0.4.1/pypots/nn/modules/saits/loss.py` & `pypots-0.5/pypots/nn/modules/saits/loss.py`

 * *Files identical despite different names*

### Comparing `pypots-0.4.1/pypots/nn/modules/timesnet/backbone.py` & `pypots-0.5/pypots/nn/modules/timesnet/backbone.py`

 * *Files identical despite different names*

### Comparing `pypots-0.4.1/pypots/nn/modules/timesnet/layers.py` & `pypots-0.5/pypots/nn/modules/timesnet/layers.py`

 * *Files identical despite different names*

### Comparing `pypots-0.4.1/pypots/nn/modules/transformer/__init__.py` & `pypots-0.5/pypots/nn/modules/transformer/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,21 +9,26 @@
 <https://proceedings.neurips.cc/paper/2017/file/3f5ee243547dee91fbd053c1c4a845aa-Paper.pdf>`_
 and
 `Wenjie Du, David Cote, and Yan Liu.
 SAITS: Self-Attention-based Imputation for Time Series.
 Expert Systems with Applications, 219:119619, 2023.
 <https://arxiv.org/pdf/2202.08516>`_
 
+
+Notes
+-----
+This implementation is inspired by https://github.com/WenjieDu/SAITS
+
 """
 
 # Created by Wenjie Du <wenjay.du@gmail.com>
 # License: BSD-3-Clause
 
 from .attention import ScaledDotProductAttention, MultiHeadAttention
-from .auto_encoder import TransformerEncoder, TransformerDecoder
+from .autoencoder import TransformerEncoder, TransformerDecoder
 from .embedding import PositionalEncoding
 from .layers import (
     TransformerEncoderLayer,
     TransformerDecoderLayer,
     PositionWiseFeedForward,
 )
```

### Comparing `pypots-0.4.1/pypots/nn/modules/transformer/attention.py` & `pypots-0.5/pypots/nn/modules/transformer/attention.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 The implementation of the modules for Transformer :cite:`vaswani2017Transformer`
 
 Notes
 -----
-Partial implementation uses code from https://github.com/WenjieDu/SAITS,
+This implementation is inspired by the official one https://github.com/WenjieDu/SAITS,
 and https://github.com/jadore801120/attention-is-all-you-need-pytorch.
 
 """
 
 # Created by Wenjie Du <wenjay.du@gmail.com>
 # License: BSD-3-Clause
 
@@ -89,17 +89,20 @@
         output:
             The result of Value multiplied with the scaled dot-product attention map.
 
         attn:
             The scaled dot-product attention map.
 
         """
-        # q, k, v all have 4 dimensions [batch_size, n_heads, n_steps, d_tensor]
+        # q, k, v all have 4 dimensions [batch_size, n_steps, n_heads, d_tensor]
         # d_tensor could be d_q, d_k, d_v
 
+        # transpose for attention dot product: [batch_size, n_heads, n_steps, d_k or d_v]
+        q, k, v = q.transpose(1, 2), k.transpose(1, 2), v.transpose(1, 2)
+
         # dot product q with k.T to obtain similarity
         attn = torch.matmul(q / self.temperature, k.transpose(2, 3))
 
         # apply masking on the attention map, this is optional
         if attn_mask is not None:
             attn = attn.masked_fill(attn_mask == 0, -1e9)
 
@@ -114,50 +117,50 @@
 
 
 class MultiHeadAttention(nn.Module):
     """Transformer multi-head attention module.
 
     Parameters
     ----------
-    n_heads:
-        The number of heads in multi-head attention.
+    attn_opt:
+        The attention operator, e.g. the self-attention proposed in Transformer.
 
     d_model:
         The dimension of the input tensor.
 
+    n_heads:
+        The number of heads in multi-head attention.
+
     d_k:
         The dimension of the key and query tensor.
 
     d_v:
         The dimension of the value tensor.
 
-    attention_operator:
-        The attention operator, e.g. the self-attention proposed in Transformer.
-
     """
 
     def __init__(
         self,
-        n_heads: int,
+        attn_opt: AttentionOperator,
         d_model: int,
+        n_heads: int,
         d_k: int,
         d_v: int,
-        attention_operator: AttentionOperator,
     ):
         super().__init__()
 
         self.n_heads = n_heads
         self.d_k = d_k
         self.d_v = d_v
 
         self.w_qs = nn.Linear(d_model, n_heads * d_k, bias=False)
         self.w_ks = nn.Linear(d_model, n_heads * d_k, bias=False)
         self.w_vs = nn.Linear(d_model, n_heads * d_v, bias=False)
 
-        self.attention_operator = attention_operator
+        self.attention_operator = attn_opt
         self.fc = nn.Linear(n_heads * d_v, d_model, bias=False)
 
     def forward(
         self,
         q: torch.Tensor,
         k: torch.Tensor,
         v: torch.Tensor,
@@ -186,29 +189,25 @@
         v:
             The output of the multi-head attention layer.
 
         attn_weights:
             The attention map.
 
         """
-        # the input q, k, v currently have 3 dimensions [batch_size, n_steps, d_tensor]
-        # d_tensor could be n_heads*d_k, n_heads*d_v
+        # the shapes of q, k, v are the same [batch_size, n_steps, d_model]
 
-        # keep useful variables
         batch_size, q_len = q.size(0), q.size(1)
         k_len = k.size(1)
         v_len = v.size(1)
 
         # now separate the last dimension of q, k, v into different heads -> [batch_size, n_steps, n_heads, d_k or d_v]
         q = self.w_qs(q).view(batch_size, q_len, self.n_heads, self.d_k)
         k = self.w_ks(k).view(batch_size, k_len, self.n_heads, self.d_k)
         v = self.w_vs(v).view(batch_size, v_len, self.n_heads, self.d_v)
-
-        # transpose for self-attention calculation -> [batch_size, n_steps, d_k or d_v, n_heads]
-        q, k, v = q.transpose(1, 2), k.transpose(1, 2), v.transpose(1, 2)
+        # for generalization, we don't do transposing here but leave it for the attention operator if necessary
 
         if attn_mask is not None:
             # broadcasting on the head axis
             attn_mask = attn_mask.unsqueeze(1)
 
         v, attn_weights = self.attention_operator(q, k, v, attn_mask, **kwargs)
```

### Comparing `pypots-0.4.1/pypots/nn/modules/transformer/auto_encoder.py` & `pypots-0.5/pypots/nn/modules/transformer/autoencoder.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -23,56 +23,56 @@
     n_layers:
         The number of layers in the encoder.
 
     d_model:
         The dimension of the module manipulation space.
         The input tensor will be projected to a space with d_model dimensions.
 
-    d_ffn:
-        The dimension of the hidden layer in the feed-forward network.
-
     n_heads:
         The number of heads in multi-head attention.
 
     d_k:
         The dimension of the key and query tensor.
 
     d_v:
         The dimension of the value tensor.
 
+    d_ffn:
+        The dimension of the hidden layer in the feed-forward network.
+
     dropout:
         The dropout rate.
 
     attn_dropout:
         The dropout rate for the attention map.
 
     """
 
     def __init__(
         self,
         n_layers: int,
         d_model: int,
-        d_ffn: int,
         n_heads: int,
         d_k: int,
         d_v: int,
+        d_ffn: int,
         dropout: float,
         attn_dropout: float,
     ):
         super().__init__()
 
         self.enc_layer_stack = nn.ModuleList(
             [
                 TransformerEncoderLayer(
+                    ScaledDotProductAttention(d_k**0.5, attn_dropout),
                     d_model,
-                    d_ffn,
                     n_heads,
                     d_k,
                     d_v,
-                    ScaledDotProductAttention(d_k**0.5, attn_dropout),
+                    d_ffn,
                     dropout,
                 )
                 for _ in range(n_layers)
             ]
         )
 
     def forward(
@@ -110,74 +110,74 @@
 
 
 class TransformerDecoder(nn.Module):
     """Transformer decoder.
 
     Parameters
     ----------
-    n_layers:
-        The number of layers in the decoder.
-
     n_steps:
         The number of time steps in the input tensor.
 
     n_features:
         The number of features in the input tensor.
 
+    n_layers:
+        The number of layers in the decoder.
+
     d_model:
         The dimension of the module manipulation space.
         The input tensor will be projected to a space with d_model dimensions.
 
-    d_ffn:
-        The dimension of the hidden layer in the feed-forward network.
-
     n_heads:
         The number of heads in multi-head attention.
 
     d_k:
         The dimension of the key and query tensor.
 
     d_v:
         The dimension of the value tensor.
 
+    d_ffn:
+        The dimension of the hidden layer in the feed-forward network.
+
     dropout:
         The dropout rate.
 
     attn_dropout:
         The dropout rate for the attention map.
 
     """
 
     def __init__(
         self,
-        n_layers: int,
         n_steps: int,
         n_features: int,
+        n_layers: int,
         d_model: int,
-        d_ffn: int,
         n_heads: int,
         d_k: int,
         d_v: int,
+        d_ffn: int,
         dropout: float,
         attn_dropout: float,
     ):
         super().__init__()
         self.embedding = nn.Linear(n_features, d_model)
         self.dropout = nn.Dropout(dropout)
         self.position_enc = PositionalEncoding(d_model, n_positions=n_steps)
         self.layer_stack = nn.ModuleList(
             [
                 TransformerDecoderLayer(
+                    ScaledDotProductAttention(d_k**0.5, attn_dropout),
+                    ScaledDotProductAttention(d_k**0.5, attn_dropout),
                     d_model,
-                    d_ffn,
                     n_heads,
                     d_k,
                     d_v,
-                    ScaledDotProductAttention(d_k**0.5, attn_dropout),
-                    ScaledDotProductAttention(d_k**0.5, attn_dropout),
+                    d_ffn,
                     dropout,
                 )
                 for _ in range(n_layers)
             ]
         )
 
     def forward(
```

### Comparing `pypots-0.4.1/pypots/nn/modules/transformer/embedding.py` & `pypots-0.5/pypots/nn/modules/transformer/embedding.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 Embedding methods for Transformer models are put here.
 
 
-Partial implementation uses code from https://github.com/zhouhaoyi/Informer2020/blob/main/models/embed.py
+This implementation is inspired by the official one https://github.com/zhouhaoyi/Informer2020/blob/main/models/embed.py
 """
 
 # Created by Wenjie Du <wenjay.du@gmail.com>
 # License: BSD-3-Clause
 
 
 import math
```

### Comparing `pypots-0.4.1/pypots/nn/modules/transformer/layers.py` & `pypots-0.5/pypots/nn/modules/transformer/layers.py`

 * *Files 7% similar despite different names*

```diff
@@ -66,49 +66,55 @@
 
 
 class TransformerEncoderLayer(nn.Module):
     """Transformer encoder layer.
 
     Parameters
     ----------
+    attn_opt:
+        The attention operator for the multi-head attention module in the encoder layer.
+
     d_model:
         The dimension of the input tensor.
 
-    d_ffn:
-        The dimension of the hidden layer.
-
     n_heads:
         The number of heads in multi-head attention.
 
     d_k:
         The dimension of the key and query tensor.
 
     d_v:
         The dimension of the value tensor.
 
-    slf_attn_opt:
-        The attention operator for the self multi-head attention module in the encoder layer.
+    d_ffn:
+        The dimension of the hidden layer.
 
     dropout:
         The dropout rate.
 
     """
 
     def __init__(
         self,
+        attn_opt: AttentionOperator,
         d_model: int,
-        d_ffn: int,
         n_heads: int,
         d_k: int,
         d_v: int,
-        slf_attn_opt: AttentionOperator,
+        d_ffn: int,
         dropout: float = 0.1,
     ):
         super().__init__()
-        self.slf_attn = MultiHeadAttention(n_heads, d_model, d_k, d_v, slf_attn_opt)
+        self.slf_attn = MultiHeadAttention(
+            attn_opt,
+            d_model,
+            n_heads,
+            d_k,
+            d_v,
+        )
         self.dropout = nn.Dropout(dropout)
         self.layer_norm = nn.LayerNorm(d_model, eps=1e-6)
         self.pos_ffn = PositionWiseFeedForward(d_model, d_ffn, dropout)
 
     def forward(
         self,
         enc_input: torch.Tensor,
@@ -154,54 +160,66 @@
 
 
 class TransformerDecoderLayer(nn.Module):
     """Transformer decoder layer.
 
     Parameters
     ----------
+    slf_attn_opt:
+        The attention operator for the multi-head attention module in the decoder layer.
+
+    enc_attn_opt:
+        The attention operator for the encoding multi-head attention module in the decoder layer.
+
     d_model:
         The dimension of the input tensor.
 
-    d_ffn:
-        The dimension of the hidden layer.
-
     n_heads:
         The number of heads in multi-head attention.
 
     d_k:
         The dimension of the key and query tensor.
 
     d_v:
         The dimension of the value tensor.
 
-    slf_attn_opt:
-        The attention operator for the self multi-head attention module in the decoder layer.
-
-    enc_attn_opt:
-        The attention operator for the encoding multi-head attention module in the decoder layer.
+    d_ffn:
+        The dimension of the hidden layer.
 
     dropout:
         The dropout rate.
 
     """
 
     def __init__(
         self,
+        slf_attn_opt: AttentionOperator,
+        enc_attn_opt: AttentionOperator,
         d_model: int,
-        d_ffn: int,
         n_heads: int,
         d_k: int,
         d_v: int,
-        slf_attn_opt: AttentionOperator,
-        enc_attn_opt: AttentionOperator,
+        d_ffn: int,
         dropout: float = 0.1,
     ):
         super().__init__()
-        self.slf_attn = MultiHeadAttention(n_heads, d_model, d_k, d_v, slf_attn_opt)
-        self.enc_attn = MultiHeadAttention(n_heads, d_model, d_k, d_v, enc_attn_opt)
+        self.slf_attn = MultiHeadAttention(
+            slf_attn_opt,
+            d_model,
+            n_heads,
+            d_k,
+            d_v,
+        )
+        self.enc_attn = MultiHeadAttention(
+            enc_attn_opt,
+            d_model,
+            n_heads,
+            d_k,
+            d_v,
+        )
         self.pos_ffn = PositionWiseFeedForward(d_model, d_ffn, dropout)
 
     def forward(
         self,
         dec_input: torch.Tensor,
         enc_output: torch.Tensor,
         slf_attn_mask: Optional[torch.Tensor] = None,
```

### Comparing `pypots-0.4.1/pypots/nn/modules/usgan/__init__.py` & `pypots-0.5/pypots/nn/modules/usgan/__init__.py`

 * *Files identical despite different names*

### Comparing `pypots-0.4.1/pypots/nn/modules/usgan/backbone.py` & `pypots-0.5/pypots/nn/modules/usgan/backbone.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,8 @@
 """
-The implementation of USGAN for the partially-observed time-series imputation task.
-
-Refer to the paper "Miao, X., Wu, Y., Wang, J., Gao, Y., Mao, X., & Yin, J. (2021).
-Generative Semi-supervised Learning for Multivariate Time Series Imputation. AAAI 2021."
 
 """
 
 # Created by Jun Wang <jwangfx@connect.ust.hk> and Wenjie Du <wenjay.du@gmail.com>
 # License: BSD-3-Clause
 
 from typing import Tuple
```

### Comparing `pypots-0.4.1/pypots/nn/modules/usgan/layers.py` & `pypots-0.5/pypots/nn/modules/usgan/layers.py`

 * *Files identical despite different names*

### Comparing `pypots-0.4.1/pypots/nn/modules/vader/__init__.py` & `pypots-0.5/pypots/nn/modules/vader/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,14 +4,18 @@
 Refer to the paper
 `Johann de Jong, Mohammad Asif Emon, Ping Wu, Reagon Karki, Meemansa Sood, Patrice Godard, Ashar Ahmad, Henri Vrooman,
 Martin Hofmann-Apitius, and Holger Fröhlich.
 Deep learning for clustering of multivariate clinical patient trajectories with missing values.
 GigaScience, 8(11):giz134, November 2019.
 <https://academic.oup.com/gigascience/article-pdf/8/11/giz134/30797160/giz134.pdf>`_
 
+Notes
+-----
+This implementation is inspired by the official one https://github.com/johanndejong/VaDER
+
 """
 
 # Created by Wenjie Du <wenjay.du@gmail.com>
 # License: BSD-3-Clause
 
 from .backbone import BackboneVaDER
 from .layers import PeepholeLSTMCell, ImplicitImputation, GMMLayer
```

### Comparing `pypots-0.4.1/pypots/nn/modules/vader/backbone.py` & `pypots-0.5/pypots/nn/modules/vader/backbone.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,8 @@
 """
-The implementation of VaDER for the partially-observed time-series clustering task.
-
-Refer to the paper "Jong, J.D., Emon, M.A., Wu, P., Karki, R., Sood, M., Godard, P., Ahmad, A., Vrooman, H.A.,
-Hofmann-Apitius, M., & Fröhlich, H. (2019).
-Deep learning for clustering of multivariate clinical patient trajectories with missing values. GigaScience."
 
 """
 
 # Created by Wenjie Du <wenjay.du@gmail.com>
 # License: BSD-3-Clause
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pypots-0.4.1/pypots/nn/modules/vader/layers.py` & `pypots-0.5/pypots/nn/modules/vader/layers.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,8 @@
 """
-The implementation of the modules for VaDER.
-
-Refer to the paper "Jong, J.D., Emon, M.A., Wu, P., Karki, R., Sood, M., Godard, P., Ahmad, A., Vrooman, H.A.,
-Hofmann-Apitius, M., & Fröhlich, H. (2019).
-Deep learning for clustering of multivariate clinical patient trajectories with missing values. GigaScience."
 
 """
 
 # Created by Wenjie Du <wenjay.du@gmail.com>
 # License: BSD-3-Clause
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pypots-0.4.1/pypots/optim/adadelta.py` & `pypots-0.5/pypots/optim/adadelta.py`

 * *Files identical despite different names*

### Comparing `pypots-0.4.1/pypots/optim/adagrad.py` & `pypots-0.5/pypots/optim/adagrad.py`

 * *Files identical despite different names*

### Comparing `pypots-0.4.1/pypots/optim/adam.py` & `pypots-0.5/pypots/optim/adam.py`

 * *Files identical despite different names*

### Comparing `pypots-0.4.1/pypots/optim/adamw.py` & `pypots-0.5/pypots/optim/adamw.py`

 * *Files identical despite different names*

### Comparing `pypots-0.4.1/pypots/optim/base.py` & `pypots-0.5/pypots/optim/base.py`

 * *Files identical despite different names*

### Comparing `pypots-0.4.1/pypots/optim/lr_scheduler/__init__.py` & `pypots-0.5/pypots/optim/lr_scheduler/__init__.py`

 * *Files identical despite different names*

### Comparing `pypots-0.4.1/pypots/optim/lr_scheduler/base.py` & `pypots-0.5/pypots/optim/lr_scheduler/base.py`

 * *Files identical despite different names*

### Comparing `pypots-0.4.1/pypots/optim/lr_scheduler/constant_lrs.py` & `pypots-0.5/pypots/optim/lr_scheduler/constant_lrs.py`

 * *Files identical despite different names*

### Comparing `pypots-0.4.1/pypots/optim/lr_scheduler/exponential_lrs.py` & `pypots-0.5/pypots/optim/lr_scheduler/exponential_lrs.py`

 * *Files identical despite different names*

### Comparing `pypots-0.4.1/pypots/optim/lr_scheduler/lambda_lrs.py` & `pypots-0.5/pypots/optim/lr_scheduler/lambda_lrs.py`

 * *Files identical despite different names*

### Comparing `pypots-0.4.1/pypots/optim/lr_scheduler/linear_lrs.py` & `pypots-0.5/pypots/optim/lr_scheduler/linear_lrs.py`

 * *Files identical despite different names*

### Comparing `pypots-0.4.1/pypots/optim/lr_scheduler/multiplicative_lrs.py` & `pypots-0.5/pypots/optim/lr_scheduler/multiplicative_lrs.py`

 * *Files identical despite different names*

### Comparing `pypots-0.4.1/pypots/optim/lr_scheduler/multistep_lrs.py` & `pypots-0.5/pypots/optim/lr_scheduler/multistep_lrs.py`

 * *Files identical despite different names*

### Comparing `pypots-0.4.1/pypots/optim/lr_scheduler/step_lrs.py` & `pypots-0.5/pypots/optim/lr_scheduler/step_lrs.py`

 * *Files identical despite different names*

### Comparing `pypots-0.4.1/pypots/optim/rmsprop.py` & `pypots-0.5/pypots/optim/rmsprop.py`

 * *Files identical despite different names*

### Comparing `pypots-0.4.1/pypots/optim/sgd.py` & `pypots-0.5/pypots/optim/sgd.py`

 * *Files identical despite different names*

### Comparing `pypots-0.4.1/pypots/utils/file.py` & `pypots-0.5/pypots/utils/file.py`

 * *Files identical despite different names*

### Comparing `pypots-0.4.1/pypots/utils/metrics/__init__.py` & `pypots-0.5/pypots/utils/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `pypots-0.4.1/pypots/utils/metrics/classification.py` & `pypots-0.5/pypots/utils/metrics/classification.py`

 * *Files identical despite different names*

### Comparing `pypots-0.4.1/pypots/utils/metrics/clustering.py` & `pypots-0.5/pypots/utils/metrics/clustering.py`

 * *Files identical despite different names*

### Comparing `pypots-0.4.1/pypots/utils/metrics/error.py` & `pypots-0.5/pypots/utils/metrics/error.py`

 * *Files identical despite different names*

### Comparing `pypots-0.4.1/pypots/utils/random.py` & `pypots-0.5/pypots/utils/random.py`

 * *Files identical despite different names*

### Comparing `pypots-0.4.1/pypots/utils/visual/clustering.py` & `pypots-0.5/pypots/utils/visual/clustering.py`

 * *Files identical despite different names*

### Comparing `pypots-0.4.1/pypots/utils/visual/data.py` & `pypots-0.5/pypots/utils/visual/data.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,34 +25,34 @@
 ):
     """Plot the imputed values, the observed values, and the evaluated values of one multivariate timeseries.
     The observed values are marked with red 'x',  the evaluated values are marked with blue 'o',
     and the imputed values are marked with solid green line.
 
     Parameters
     ----------
-    X : ndarray,
+    X :
         The observed values
 
-    X_ori : ndarray,
+    X_ori :
         The evaluated values
 
-    X_imputed : ndarray,
+    X_imputed :
         The imputed values
 
-    sample_idx : int,
+    sample_idx :
         The index of the sample to be plotted.
         If None, a randomly-selected sample will be plotted for visualization.
 
-    n_rows : int,
+    n_rows :
         The number of rows in the plot
 
-    n_cols : int,
+    n_cols :
         The number of columns in the plot
 
-    fig_size : list,
+    fig_size :
         The size of the figure
     """
 
     vals_shape = X.shape
     assert (
         len(vals_shape) == 3
     ), "vals_obs should be a 3D array of shape (n_samples, n_steps, n_features)"
@@ -91,35 +91,35 @@
 
     logger.info(
         "Plotting finished. Please invoke matplotlib.pyplot.show() to display the plot."
     )
 
 
 def plot_missingness(
-    missing_mask,
-    min_step=0,
-    max_step=1,
+    missing_mask: int,
+    min_step: int = 0,
+    max_step: int = 1,
     sample_idx: Optional[int] = None,
 ):
     """Plot the missingness pattern of one multivariate timeseries. For each feature,
     the observed timestamp is marked with blue '|'. The distribution of sequence lengths is also plotted.
     Hereby, the sequence length is defined as the number of observed timestamps in one feature.
 
     Parameters
     ----------
-    missing_mask : ndarray,
+    missing_mask :
         The missing mask of multivariate time series.
 
-    min_step : int,
+    min_step :
         The minimum time step for visualization.
 
-    max_step : int,
+    max_step :
         The maximum time step for visualization.
 
-    sample_idx : int,
+    sample_idx :
         The index of the sample to be plotted, if None, a randomly-selected sample will be plotted for visualization.
     """
     mask_shape = missing_mask.shape
     if len(mask_shape) == 3:
         n_samples, n_steps, n_features = missing_mask.shape
         if sample_idx is None:
             sample_idx = np.random.randint(low=0, high=n_samples)
```

### Comparing `pypots-0.4.1/pypots.egg-info/PKG-INFO` & `pypots-0.5/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,45 +1,7 @@
-Metadata-Version: 2.1
-Name: pypots
-Version: 0.4.1
-Summary: A Python Toolbox for Data Mining on Partially-Observed Time Series
-Home-page: https://pypots.com/
-Author: Wenjie Du
-Author-email: wenjay.du@gmail.com
-License: BSD-3-Clause
-Project-URL: Documentation, https://docs.pypots.com/
-Project-URL: Source, https://github.com/WenjieDu/PyPOTS/
-Project-URL: Tracker, https://github.com/WenjieDu/PyPOTS/issues/
-Project-URL: Download, https://github.com/WenjieDu/PyPOTS/archive/main.zip
-Keywords: data science,data mining,neural networks,machine learning,deep learning,artificial intelligence,time-series analysis,time series,imputation,interpolation,classification,clustering,forecasting,partially observed,irregular sampled,partially-observed time series,incomplete time series,missing data,missing values
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Education
-Classifier: Intended Audience :: Science/Research
-Classifier: Intended Audience :: Healthcare Industry
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
-Requires-Python: >=3.7.0
-Description-Content-Type: text/markdown
-Provides-Extra: basic
-Provides-Extra: optional
-Provides-Extra: full
-Provides-Extra: test
-Provides-Extra: doc
-Provides-Extra: dev
-License-File: LICENSE
-
 <a href="https://github.com/WenjieDu/PyPOTS">
     <img src="https://pypots.com/figs/pypots_logos/PyPOTS/logo_FFBG.svg" width="200" align="right">
 </a>
 
 <h3 align="center">Welcome to PyPOTS</h3>
 
 <p align="center"><i>a Python toolbox for machine learning on Partially-Observed Time Series</i></p>
@@ -86,14 +48,17 @@
     </a>
     <a href="https://pepy.tech/project/pypots">
         <img alt="PyPI downloads" src="https://img.shields.io/endpoint?url=https://pypots.com/figs/downloads_badges/pypi_pypots_downloads.json">
     </a>
     <a href="https://arxiv.org/abs/2305.18811">
         <img alt="arXiv DOI" src="https://img.shields.io/badge/DOI-10.48550/arXiv.2305.18811-F8F7F0">
     </a>
+    <a href="https://github.com/WenjieDu/PyPOTS/blob/main/README_zh.md">
+        <img alt="README in Chinese" src="https://img.shields.io/badge/README-🇨🇳中文版-FCEFE8">
+    </a>
 </p>
 
 ⦿ `Motivation`: Due to all kinds of reasons like failure of collection sensors, communication error,
 and unexpected malfunction, missing values are common to see in time series from the real-world environment.
 This makes partially-observed time series (POTS) a pervasive problem in open-world modeling and prevents advanced
 data analysis. Although this problem is important, the area of machine learning on POTS still lacks a dedicated toolkit.
 PyPOTS is created to fill in this blank.
@@ -105,36 +70,90 @@
 have unified APIs together with detailed documentation and interactive examples across algorithms as tutorials.
 
 🤗 **Please** star this repo to help others notice PyPOTS if you think it is a useful toolkit.
 **Please** properly [cite PyPOTS](https://github.com/WenjieDu/PyPOTS#-citing-pypots) in your publications
 if it helps with your research. This really means a lot to our open-source research. Thank you!
 
 The rest of this readme file is organized as follows:
+[**❖ Available Algorithms**](#-available-algorithms),
 [**❖ PyPOTS Ecosystem**](#-pypots-ecosystem),
 [**❖ Installation**](#-installation),
 [**❖ Usage**](#-usage),
-[**❖ Available Algorithms**](#-available-algorithms),
 [**❖ Citing PyPOTS**](#-citing-pypots),
 [**❖ Contribution**](#-contribution),
 [**❖ Community**](#-community).
 
 
+## ❖ Available Algorithms
+PyPOTS supports imputation, classification, clustering, forecasting, and anomaly detection tasks on multivariate partially-observed
+time series with missing values. The table below shows the availability of each algorithm (sorted by Year) in PyPOTS for different tasks.
+The symbol ✅ indicates the algorithm is available for the corresponding task (note that models will be continuously updated
+in the future to handle tasks that are not currently supported. Stay tuned❗️).
+
+🌟 Since **v0.2**, all neural-network models in PyPOTS has got hyperparameter-optimization support.
+This functionality is implemented with the [Microsoft NNI](https://github.com/microsoft/nni) framework. You may want to refer to our time-series
+imputation survey repo [Awesome_Imputation](https://github.com/WenjieDu/Awesome_Imputation) to see how to config and
+tune the hyperparameters.
+
+🔥 Note that Transformer, iTransformer, FreTS, Crossformer, PatchTST, DLinear, ETSformer, FiLM, FEDformer, Informer, Autoformer
+are not proposed as imputation methods in their original papers, and they cannot accept POTS as input.
+**To make them applicable on POTS data, we apply the embedding strategy and training approach (ORT+MIT)
+the same as we did in [SAITS paper](https://arxiv.org/pdf/2202.08516).**
+
+The task types are abbreviated as follows:
+**`IMPU`**: Imputation;
+**`FORE`**: Forecasting;
+**`CLAS`**: Classification;
+**`CLUS`**: Clustering;
+**`ANOD`**: Anomaly Detection.
+The paper references and links are all listed at the bottom of this file.
+
+| **Type**      | **Algo**                           | **IMPU** | **FORE** | **CLAS** | **CLUS** | **ANOD** | **Year - Venue** |
+|:--------------|:-----------------------------------|:--------:|:--------:|:--------:|:--------:|:--------:|:-----------------|
+| Neural Net    | iTransformer[^24]                  |    ✅     |          |          |          |          | 2024 - ICLR      |
+| Neural Net    | FreTS[^23]                         |    ✅     |          |          |          |          | 2024 - NeurIPS   |
+| Neural Net    | SAITS[^1]                          |    ✅     |          |          |          |          | 2023 - ESWA      |
+| Neural Net    | Crossformer[^16]                   |    ✅     |          |          |          |          | 2023 - ICLR      |
+| Neural Net    | TimesNet[^14]                      |    ✅     |          |          |          |          | 2023 - ICLR      |
+| Neural Net    | PatchTST[^18]                      |    ✅     |          |          |          |          | 2023 - ICLR      |
+| Neural Net    | ETSformer[^19]                     |    ✅     |          |          |          |          | 2023 - ICLR      |
+| Neural Net    | DLinear[^17]                       |    ✅     |          |          |          |          | 2023 - AAAI      |
+| Neural Net    | FiLM[^22]                          |    ✅     |          |          |          |          | 2022 - NeurIPS   |
+| Neural Net    | Raindrop[^5]                       |          |          |    ✅     |          |          | 2022 - ICLR      |
+| Neural Net    | FEDformer[^20]                     |    ✅     |          |          |          |          | 2022 - ICML      |
+| Neural Net    | Autoformer[^15]                    |    ✅     |          |          |          |          | 2021 - NeurIPS   |
+| Neural Net    | CSDI[^12]                          |    ✅     |    ✅     |          |          |          | 2021 - NeurIPS   |
+| Neural Net    | Informer[^21]                      |    ✅     |          |          |          |          | 2021 - AAAI      |
+| Neural Net    | US-GAN[^10]                        |    ✅     |          |          |          |          | 2021 - AAAI      |
+| Neural Net    | CRLI[^6]                           |          |          |          |    ✅     |          | 2021 - AAAI      |
+| Probabilistic | BTTF[^8]                           |          |    ✅     |          |          |          | 2021 - TPAMI     |
+| Neural Net    | GP-VAE[^11]                        |    ✅     |          |          |          |          | 2020 - AISTATS   |
+| Neural Net    | VaDER[^7]                          |          |          |          |    ✅     |          | 2019 - GigaSci.  |
+| Neural Net    | M-RNN[^9]                          |    ✅     |          |          |          |          | 2019 - TBME      |
+| Neural Net    | BRITS[^3]                          |    ✅     |          |    ✅     |          |          | 2018 - NeurIPS   |
+| Neural Net    | GRU-D[^4]                          |    ✅     |          |    ✅     |          |          | 2018 - Sci. Rep. |
+| Neural Net    | Transformer[^2]                    |    ✅     |          |          |          |          | 2017 - NeurIPS   |
+| Naive         | LOCF/NOCB                          |    ✅     |          |          |          |          |                  |
+| Naive         | Mean                               |    ✅     |          |          |          |          |                  |
+| Naive         | Median                             |    ✅     |          |          |          |          |                  |
+
+
 ## ❖ PyPOTS Ecosystem
 At PyPOTS, things are related to coffee, which we're familiar with. Yes, this is a coffee universe!
 As you can see, there is a coffee pot in the PyPOTS logo.
 And what else? Please read on ;-)
 
 <a href="https://github.com/WenjieDu/TSDB">
     <img src="https://pypots.com/figs/pypots_logos/TSDB/logo_FFBG.svg" align="left" width="140" alt="TSDB logo"/>
 </a>
 
 👈 Time series datasets are taken as coffee beans at PyPOTS, and POTS datasets are incomplete coffee beans with missing parts that have their own meanings.
 To make various public time-series datasets readily available to users,
 <i>Time Series Data Beans (TSDB)</i> is created to make loading time-series datasets super easy!
-Visit [TSDB](https://github.com/WenjieDu/TSDB) right now to know more about this handy tool 🛠, and it now supports a total of 168 open-source datasets!
+Visit [TSDB](https://github.com/WenjieDu/TSDB) right now to know more about this handy tool 🛠, and it now supports a total of 169 open-source datasets!
 
 <a href="https://github.com/WenjieDu/PyGrinder">
     <img src="https://pypots.com/figs/pypots_logos/PyGrinder/logo_FFBG.svg" align="right" width="140" alt="PyGrinder logo"/>
 </a>
 
 👉 To simulate the real-world data beans with missingness, the ecosystem library [PyGrinder](https://github.com/WenjieDu/PyGrinder),
 a toolkit helping grind your coffee beans into incomplete ones, is created. Missing patterns fall into three categories according to Robin's theory[^13]:
@@ -160,15 +179,15 @@
 </p>
 
 
 ## ❖ Installation
 You can refer to [the installation instruction](https://docs.pypots.com/en/latest/install.html) in PyPOTS documentation for a guideline with more details.
 
 PyPOTS is available on both [PyPI](https://pypi.python.org/pypi/pypots) and [Anaconda](https://anaconda.org/conda-forge/pypots).
-You can install PyPOTS as shown below:
+You can install PyPOTS like below as well as TSDB and PyGrinder:
 
 ``` bash
 # via pip
 pip install pypots            # the first time installation
 pip install pypots --upgrade  # update pypots to the latest version
 # install from the latest source code with the latest features but may be not officially released yet
 pip install https://github.com/WenjieDu/PyPOTS/archive/main.zip
@@ -188,91 +207,45 @@
 
 We present you a usage example of imputing missing values in time series with PyPOTS below, you can click it to view.
 
 <details open>
 <summary><b>Click here to see an example applying SAITS on PhysioNet2012 for imputation:</b></summary>
 
 ``` python
+# Data preprocessing. Tedious, but PyPOTS can help.
 import numpy as np
 from sklearn.preprocessing import StandardScaler
 from pygrinder import mcar
 from pypots.data import load_specific_dataset
-from pypots.imputation import SAITS
-from pypots.utils.metrics import calc_mae
-
-# Data preprocessing. Tedious, but PyPOTS can help.
 data = load_specific_dataset('physionet_2012')  # PyPOTS will automatically download and extract it.
 X = data['X']
 num_samples = len(X['RecordID'].unique())
 X = X.drop(['RecordID', 'Time'], axis = 1)
 X = StandardScaler().fit_transform(X.to_numpy())
 X = X.reshape(num_samples, 48, -1)
 X_ori = X  # keep X_ori for validation
 X = mcar(X, 0.1)  # randomly hold out 10% observed values as ground truth
 dataset = {"X": X}  # X for model input
 print(X.shape)  # (11988, 48, 37), 11988 samples and each sample has 48 time steps, 37 features
 
 # Model training. This is PyPOTS showtime.
-saits = SAITS(n_steps=48, n_features=37, n_layers=2, d_model=256, d_ffn=128, n_heads=4, d_k=64, d_v=64, dropout=0.1, epochs=10)
+from pypots.imputation import SAITS
+from pypots.utils.metrics import calc_mae
+saits = SAITS(n_steps=48, n_features=37, n_layers=2, d_model=256, n_heads=4, d_k=64, d_v=64, d_ffn=128, dropout=0.1, epochs=10)
 # Here I use the whole dataset as the training set because ground truth is not visible to the model, you can also split it into train/val/test sets
-saits.fit(dataset)
+saits.fit(dataset)  # train the model on the dataset
 imputation = saits.impute(dataset)  # impute the originally-missing values and artificially-missing values
 indicating_mask = np.isnan(X) ^ np.isnan(X_ori)  # indicating mask for imputation error calculation
 mae = calc_mae(imputation, np.nan_to_num(X_ori), indicating_mask)  # calculate mean absolute error on the ground truth (artificially-missing values)
+saits.save("save_it_here/saits_physionet2012.pypots")  # save the model for future use
+saits.load("save_it_here/saits_physionet2012.pypots")  # reload the serialized model file for following imputation or training
 ```
 </details>
 
 
-## ❖ Available Algorithms
-PyPOTS supports imputation, classification, clustering, and forecasting tasks on multivariate time series with missing values.
-The currently available algorithms of four tasks are cataloged in the following table with four partitions.
-The paper references are all listed at the bottom of this readme file.
-
-🌟 Since **v0.2**, all neural-network models in PyPOTS has got hyperparameter-optimization support.
-This functionality is implemented with the [Microsoft NNI](https://github.com/microsoft/nni) framework.
-
-🔥 Note that Transformer, Crossformer, PatchTST, DLinear, ETSformer, FEDformer, Informer, Autoformer are not proposed as imputation methods in their original papers,
-and they cannot accept POTS as input. **To make them applicable on POTS data, we apply the embedding strategy and training approach (ORT+MIT)
-the same as we did in [SAITS paper](https://arxiv.org/pdf/2202.08516).**
-
-|   ***`Imputation`***   |     🚥      |                                               🚥                                                |    🚥    |
-|:----------------------:|:-----------:|:-----------------------------------------------------------------------------------------------:|:--------:|
-|        **Type**        |  **Abbr.**  |                              **Full name of the algorithm/model**                               | **Year** |
-|       Neural Net       |    SAITS    |                      Self-Attention-based Imputation for Time Series [^1]                       |   2023   |
-|       Neural Net       | Transformer |                                 Attention is All you Need [^2]                                  |   2017   |
-|       Neural Net       | Crossformer | Transformer Utilizing Cross-Dimension Dependency for Multivariate Time Series Forecasting [^16] |   2023   |
-|       Neural Net       |  TimesNet   |              Temporal 2D-Variation Modeling for General Time Series Analysis [^14]              |   2023   |
-|       Neural Net       |  PatchTST   |         A Time Series is Worth 64 Words: Long-Term Forecasting with Transformers [^18]          |   2023   |
-|       Neural Net       |   DLinear   |                  Are Transformers Effective for Time Series Forecasting? [^17]                  |   2023   |
-|       Neural Net       |  ETSformer  |              Exponential Smoothing Transformers for Time-series Forecasting [^19]               |   2023   |
-|       Neural Net       |  FEDformer  |        Frequency Enhanced Decomposed Transformer for Long-term Series Forecasting [^20]         |   2022   |
-|       Neural Net       |  Informer   |          Beyond Efficient Transformer for Long Sequence Time-Series Forecasting [^21]           |   2021   |
-|       Neural Net       | Autoformer  |     Decomposition Transformers with Auto-Correlation for Long-Term Series Forecasting [^15]     |   2021   |
-|       Neural Net       |    CSDI     |     Conditional Score-based Diffusion Models for Probabilistic Time Series Imputation [^12]     |   2021   |
-|       Neural Net       |   US-GAN    |                 Unsupervised GAN for Multivariate Time Series Imputation [^10]                  |   2021   |
-|       Neural Net       |   GP-VAE    |                         Gaussian Process Variational Autoencoder [^11]                          |   2020   |
-|       Neural Net       |    BRITS    |                     Bidirectional Recurrent Imputation for Time Series [^3]                     |   2018   |
-|       Neural Net       |    M-RNN    |                         Multi-directional Recurrent Neural Network [^9]                         |   2019   |
-|         Naive          |  LOCF/NOCB  |              Last Observation Carried Forward / Next Observation Carried Backward               |    -     |
-|         Naive          |   Median    |                                     Median Value Imputation                                     |    -     |
-|         Naive          |    Mean     |                                      Mean Value Imputation                                      |    -     |
-| ***`Classification`*** |     🚥      |                                               🚥                                                |    🚥    |
-|        **Type**        |  **Abbr.**  |                           **Full name of the algorithm/model/paper**                            | **Year** |
-|       Neural Net       |    BRITS    |                     Bidirectional Recurrent Imputation for Time Series [^3]                     |   2018   |
-|       Neural Net       |    GRU-D    |         Recurrent Neural Networks for Multivariate Time Series with Missing Values [^4]         |   2018   |
-|       Neural Net       |  Raindrop   |           Graph-Guided Network for Irregularly Sampled Multivariate Time Series [^5]            |   2022   |
-|   ***`Clustering`***   |     🚥      |                                               🚥                                                |    🚥    |
-|        **Type**        |  **Abbr.**  |                           **Full name of the algorithm/model/paper**                            | **Year** |
-|       Neural Net       |    CRLI     |             Clustering Representation Learning on Incomplete time-series data [^6]              |   2021   |
-|       Neural Net       |    VaDER    |                         Variational Deep Embedding with Recurrence [^7]                         |   2019   |
-|  ***`Forecasting`***   |     🚥      |                                               🚥                                                |    🚥    |
-|        **Type**        |  **Abbr.**  |                           **Full name of the algorithm/model/paper**                            | **Year** |
-|     Probabilistic      |    BTTF     |                           Bayesian Temporal Tensor Factorization [^8]                           |   2021   |
-
-
 ## ❖ Citing PyPOTS
 > [!TIP]
 > **[Updates in Feb 2024]** 😎 Our survey paper [Deep Learning for Multivariate Time Series Imputation: A Survey](https://arxiv.org/abs/2402.04059) has been released on arXiv.
 The code is open source in the GitHub repo [Awesome_Imputation](https://github.com/WenjieDu/Awesome_Imputation).
 We comprehensively review the literature of the state-of-the-art deep-learning imputation methods for time series,
 provide a taxonomy for them, and discuss the challenges and future directions in this field.
 >
@@ -372,14 +345,17 @@
 [^15]: Wu, H., Xu, J., Wang, J., & Long, M. (2021). [Autoformer: Decomposition transformers with auto-correlation for long-term series forecasting](https://proceedings.neurips.cc/paper/2021/hash/bcc0d400288793e8bdcd7c19a8ac0c2b-Abstract.html). *NeurIPS 2021*.
 [^16]: Zhang, Y., & Yan, J. (2023). [Crossformer: Transformer utilizing cross-dimension dependency for multivariate time series forecasting](https://openreview.net/forum?id=vSVLM2j9eie). *ICLR 2023*.
 [^17]: Zeng, A., Chen, M., Zhang, L., & Xu, Q. (2023). [Are transformers effective for time series forecasting?](https://ojs.aaai.org/index.php/AAAI/article/view/26317). *AAAI 2023*
 [^18]: Nie, Y., Nguyen, N. H., Sinthong, P., & Kalagnanam, J. (2023). [A time series is worth 64 words: Long-term forecasting with transformers](https://openreview.net/forum?id=Jbdc0vTOcol). *ICLR 2023*
 [^19]: Woo, G., Liu, C., Sahoo, D., Kumar, A., & Hoi, S. (2023). [ETSformer: Exponential Smoothing Transformers for Time-series Forecasting](https://openreview.net/forum?id=5m_3whfo483).  *ICLR 2023*
 [^20]: Zhou, T., Ma, Z., Wen, Q., Wang, X., Sun, L., & Jin, R. (2022). [FEDformer: Frequency enhanced decomposed transformer for long-term series forecasting](https://proceedings.mlr.press/v162/zhou22g.html). *ICML 2022*.
 [^21]: Zhou, H., Zhang, S., Peng, J., Zhang, S., Li, J., Xiong, H., & Zhang, W. (2021). [Informer: Beyond efficient transformer for long sequence time-series forecasting](https://ojs.aaai.org/index.php/AAAI/article/view/17325). *AAAI 2021*.
+[^22]: Zhou, T., Ma, Z., Wen, Q., Sun, L., Yao, T., Yin, W., & Jin, R. (2022). [FiLM: Frequency improved Legendre Memory Model for Long-term Time Series Forecasting](https://proceedings.neurips.cc/paper_files/paper/2022/hash/524ef58c2bd075775861234266e5e020-Abstract-Conference.html). *NeurIPS 2022*.
+[^23]: Yi, K., Zhang, Q., Fan, W., Wang, S., Wang, P., He, H., An, N., Lian, D., Cao, L., & Niu, Z. (2024). [Frequency-domain MLPs are More Effective Learners in Time Series Forecasting](https://proceedings.neurips.cc/paper_files/paper/2023/hash/f1d16af76939f476b5f040fd1398c0a3-Abstract-Conference.html). *NeurIPS 2024*.
+[^24]: Liu, Y., Hu, T., Zhang, H., Wu, H., Wang, S., Ma, L., & Long, M. (2024). [iTransformer: Inverted Transformers Are Effective for Time Series Forecasting](https://openreview.net/forum?id=JePfAI8fah). *ICLR 2024*.
 
 
 
 <details>
 <summary>🏠 Visits</summary>
 <a href="https://github.com/WenjieDu/PyPOTS">
     <img alt="PyPOTS visits" align="left" src="https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fgithub.com%2FPyPOTS%2FPyPOTS&count_bg=%23009A0A&title_bg=%23555555&icon=&icon_color=%23E7E7E7&title=Visits%20since%20May%202022&edge_flat=false">
```

#### html2text {}

```diff
@@ -1,39 +1,14 @@
-Metadata-Version: 2.1 Name: pypots Version: 0.4.1 Summary: A Python Toolbox for
-Data Mining on Partially-Observed Time Series Home-page: https://pypots.com/
-Author: Wenjie Du Author-email: wenjay.du@gmail.com License: BSD-3-Clause
-Project-URL: Documentation, https://docs.pypots.com/ Project-URL: Source,
-https://github.com/WenjieDu/PyPOTS/ Project-URL: Tracker, https://github.com/
-WenjieDu/PyPOTS/issues/ Project-URL: Download, https://github.com/WenjieDu/
-PyPOTS/archive/main.zip Keywords: data science,data mining,neural
-networks,machine learning,deep learning,artificial intelligence,time-series
-analysis,time
-series,imputation,interpolation,classification,clustering,forecasting,partially
-observed,irregular sampled,partially-observed time series,incomplete time
-series,missing data,missing values Classifier: Development Status :: 5 -
-Production/Stable Classifier: Intended Audience :: Developers Classifier:
-Intended Audience :: Education Classifier: Intended Audience :: Science/
-Research Classifier: Intended Audience :: Healthcare Industry Classifier:
-License :: OSI Approved :: BSD License Classifier: Operating System :: OS
-Independent Classifier: Programming Language :: Python :: 3 Classifier:
-Programming Language :: Python :: 3.7 Classifier: Programming Language ::
-Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
-Programming Language :: Python :: 3.10 Classifier: Programming Language ::
-Python :: 3.11 Classifier: Topic :: Scientific/Engineering :: Artificial
-Intelligence Classifier: Topic :: Software Development :: Libraries ::
-Application Frameworks Requires-Python: >=3.7.0 Description-Content-Type: text/
-markdown Provides-Extra: basic Provides-Extra: optional Provides-Extra: full
-Provides-Extra: test Provides-Extra: doc Provides-Extra: dev License-File:
-LICENSE_[_h_t_t_p_s_:_/_/_p_y_p_o_t_s_._c_o_m_/_f_i_g_s_/_p_y_p_o_t_s___l_o_g_o_s_/_P_y_P_O_T_S_/_l_o_g_o___F_F_B_G_._s_v_g_]
+_[_h_t_t_p_s_:_/_/_p_y_p_o_t_s_._c_o_m_/_f_i_g_s_/_p_y_p_o_t_s___l_o_g_o_s_/_P_y_P_O_T_S_/_l_o_g_o___F_F_B_G_._s_v_g_]
                           ******** WWeellccoommee ttoo PPyyPPOOTTSS ********
     a Python toolbox for machine learning on Partially-Observed Time Series
 _[_P_y_t_h_o_n_ _v_e_r_s_i_o_n_]_[_p_o_w_e_r_e_d_ _b_y_ _P_y_t_o_r_c_h_]_[_t_h_e_ _l_a_t_e_s_t_ _r_e_l_e_a_s_e_ _v_e_r_s_i_o_n_]_[_B_S_D_-_3_ _l_i_c_e_n_s_e_]
   _[_C_o_m_m_u_n_i_t_y_]_[_G_i_t_H_u_b_ _c_o_n_t_r_i_b_u_t_o_r_s_]_[_G_i_t_H_u_b_ _R_e_p_o_ _s_t_a_r_s_]_[_G_i_t_H_u_b_ _R_e_p_o_ _f_o_r_k_s_]_[_C_o_d_e
   _C_l_i_m_a_t_e_ _m_a_i_n_t_a_i_n_a_b_i_l_i_t_y_]_[_C_o_v_e_r_a_l_l_s_ _c_o_v_e_r_a_g_e_]_[_G_i_t_H_u_b_ _T_e_s_t_i_n_g_]_[_D_o_c_s_ _b_u_i_l_d_i_n_g_]
-                 _[_C_o_n_d_a_ _d_o_w_n_l_o_a_d_s_]_[_P_y_P_I_ _d_o_w_n_l_o_a_d_s_]_[_a_r_X_i_v_ _D_O_I_]
+        _[_C_o_n_d_a_ _d_o_w_n_l_o_a_d_s_]_[_P_y_P_I_ _d_o_w_n_l_o_a_d_s_]_[_a_r_X_i_v_ _D_O_I_]_[_R_E_A_D_M_E_ _i_n_ _C_h_i_n_e_s_e_]
 â¦¿ `Motivation`: Due to all kinds of reasons like failure of collection
 sensors, communication error, and unexpected malfunction, missing values are
 common to see in time series from the real-world environment. This makes
 partially-observed time series (POTS) a pervasive problem in open-world
 modeling and prevents advanced data analysis. Although this problem is
 important, the area of machine learning on POTS still lacks a dedicated
 toolkit. PyPOTS is created to fill in this blank. â¦¿ `Mission`: PyPOTS
@@ -45,150 +20,144 @@
 partially-observed multivariate time series. For sure, besides various
 algorithms, PyPOTS is going to have unified APIs together with detailed
 documentation and interactive examples across algorithms as tutorials. ð¤
 **Please** star this repo to help others notice PyPOTS if you think it is a
 useful toolkit. **Please** properly [cite PyPOTS](https://github.com/WenjieDu/
 PyPOTS#-citing-pypots) in your publications if it helps with your research.
 This really means a lot to our open-source research. Thank you! The rest of
-this readme file is organized as follows: [**â PyPOTS Ecosystem**](#-pypots-
-ecosystem), [**â Installation**](#-installation), [**â Usage**](#-usage),
-[**â Available Algorithms**](#-available-algorithms), [**â Citing PyPOTS**]
-(#-citing-pypots), [**â Contribution**](#-contribution), [**â Community**]
-(#-community). ## â PyPOTS Ecosystem At PyPOTS, things are related to coffee,
-which we're familiar with. Yes, this is a coffee universe! As you can see,
-there is a coffee pot in the PyPOTS logo. And what else? Please read on ;-)
-_[_T_S_D_B_ _l_o_g_o_]ð Time series datasets are taken as coffee beans at PyPOTS, and
-POTS datasets are incomplete coffee beans with missing parts that have their
-own meanings. To make various public time-series datasets readily available to
-users, Time Series Data Beans (TSDB) is created to make loading time-series
-datasets super easy! Visit [TSDB](https://github.com/WenjieDu/TSDB) right now
-to know more about this handy tool ð , and it now supports a total of 168
-open-source datasets! _[_P_y_G_r_i_n_d_e_r_ _l_o_g_o_]ð To simulate the real-world data
-beans with missingness, the ecosystem library [PyGrinder](https://github.com/
-WenjieDu/PyGrinder), a toolkit helping grind your coffee beans into incomplete
-ones, is created. Missing patterns fall into three categories according to
-Robin's theory[^13]: MCAR (missing completely at random), MAR (missing at
-random), and MNAR (missing not at random). PyGrinder supports all of them and
-additional functionalities related to missingness. With PyGrinder, you can
-introduce synthetic missing values into your datasets with a single line of
-code. _[_B_r_e_w_P_O_T_S_ _l_o_g_o_]ð Now we have the beans, the grinder, and the pot, how
-to brew us a cup of coffee? Tutorials are necessary! Considering the future
-workload, PyPOTS tutorials are released in a single repo, and you can find them
-in [BrewPOTS](https://github.com/WenjieDu/BrewPOTS). Take a look at it now, and
-learn how to brew your POTS datasets!
+this readme file is organized as follows: [**â Available Algorithms**](#-
+available-algorithms), [**â PyPOTS Ecosystem**](#-pypots-ecosystem), [**â
+Installation**](#-installation), [**â Usage**](#-usage), [**â Citing
+PyPOTS**](#-citing-pypots), [**â Contribution**](#-contribution), [**â
+Community**](#-community). ## â Available Algorithms PyPOTS supports
+imputation, classification, clustering, forecasting, and anomaly detection
+tasks on multivariate partially-observed time series with missing values. The
+table below shows the availability of each algorithm (sorted by Year) in PyPOTS
+for different tasks. The symbol â indicates the algorithm is available for
+the corresponding task (note that models will be continuously updated in the
+future to handle tasks that are not currently supported. Stay tunedâï¸).
+ð Since **v0.2**, all neural-network models in PyPOTS has got
+hyperparameter-optimization support. This functionality is implemented with the
+[Microsoft NNI](https://github.com/microsoft/nni) framework. You may want to
+refer to our time-series imputation survey repo [Awesome_Imputation](https://
+github.com/WenjieDu/Awesome_Imputation) to see how to config and tune the
+hyperparameters. ð¥ Note that Transformer, iTransformer, FreTS, Crossformer,
+PatchTST, DLinear, ETSformer, FiLM, FEDformer, Informer, Autoformer are not
+proposed as imputation methods in their original papers, and they cannot accept
+POTS as input. **To make them applicable on POTS data, we apply the embedding
+strategy and training approach (ORT+MIT) the same as we did in [SAITS paper]
+(https://arxiv.org/pdf/2202.08516).** The task types are abbreviated as
+follows: **`IMPU`**: Imputation; **`FORE`**: Forecasting; **`CLAS`**:
+Classification; **`CLUS`**: Clustering; **`ANOD`**: Anomaly Detection. The
+paper references and links are all listed at the bottom of this file. |
+**Type** | **Algo** | **IMPU** | **FORE** | **CLAS** | **CLUS** | **ANOD** |
+**Year - Venue** | |:--------------|:-----------------------------------|:-----
+---:|:--------:|:--------:|:--------:|:--------:|:-----------------| | Neural
+Net | iTransformer[^24] | â | | | | | 2024 - ICLR | | Neural Net | FreTS[^23]
+| â | | | | | 2024 - NeurIPS | | Neural Net | SAITS[^1] | â | | | | | 2023
+- ESWA | | Neural Net | Crossformer[^16] | â | | | | | 2023 - ICLR | | Neural
+Net | TimesNet[^14] | â | | | | | 2023 - ICLR | | Neural Net | PatchTST[^18]
+| â | | | | | 2023 - ICLR | | Neural Net | ETSformer[^19] | â | | | | |
+2023 - ICLR | | Neural Net | DLinear[^17] | â | | | | | 2023 - AAAI | |
+Neural Net | FiLM[^22] | â | | | | | 2022 - NeurIPS | | Neural Net | Raindrop
+[^5] | | | â | | | 2022 - ICLR | | Neural Net | FEDformer[^20] | â | | | |
+| 2022 - ICML | | Neural Net | Autoformer[^15] | â | | | | | 2021 - NeurIPS |
+| Neural Net | CSDI[^12] | â | â | | | | 2021 - NeurIPS | | Neural Net |
+Informer[^21] | â | | | | | 2021 - AAAI | | Neural Net | US-GAN[^10] | â |
+| | | | 2021 - AAAI | | Neural Net | CRLI[^6] | | | | â | | 2021 - AAAI | |
+Probabilistic | BTTF[^8] | | â | | | | 2021 - TPAMI | | Neural Net | GP-VAE
+[^11] | â | | | | | 2020 - AISTATS | | Neural Net | VaDER[^7] | | | | â | |
+2019 - GigaSci. | | Neural Net | M-RNN[^9] | â | | | | | 2019 - TBME | |
+Neural Net | BRITS[^3] | â | | â | | | 2018 - NeurIPS | | Neural Net | GRU-
+D[^4] | â | | â | | | 2018 - Sci. Rep. | | Neural Net | Transformer[^2] |
+â | | | | | 2017 - NeurIPS | | Naive | LOCF/NOCB | â | | | | | | | Naive |
+Mean | â | | | | | | | Naive | Median | â | | | | | | ## â PyPOTS
+Ecosystem At PyPOTS, things are related to coffee, which we're familiar with.
+Yes, this is a coffee universe! As you can see, there is a coffee pot in the
+PyPOTS logo. And what else? Please read on ;-) _[_T_S_D_B_ _l_o_g_o_]ð Time series
+datasets are taken as coffee beans at PyPOTS, and POTS datasets are incomplete
+coffee beans with missing parts that have their own meanings. To make various
+public time-series datasets readily available to users, Time Series Data Beans
+(TSDB) is created to make loading time-series datasets super easy! Visit [TSDB]
+(https://github.com/WenjieDu/TSDB) right now to know more about this handy tool
+ð , and it now supports a total of 169 open-source datasets! _[_P_y_G_r_i_n_d_e_r
+_l_o_g_o_]ð To simulate the real-world data beans with missingness, the ecosystem
+library [PyGrinder](https://github.com/WenjieDu/PyGrinder), a toolkit helping
+grind your coffee beans into incomplete ones, is created. Missing patterns fall
+into three categories according to Robin's theory[^13]: MCAR (missing
+completely at random), MAR (missing at random), and MNAR (missing not at
+random). PyGrinder supports all of them and additional functionalities related
+to missingness. With PyGrinder, you can introduce synthetic missing values into
+your datasets with a single line of code. _[_B_r_e_w_P_O_T_S_ _l_o_g_o_]ð Now we have the
+beans, the grinder, and the pot, how to brew us a cup of coffee? Tutorials are
+necessary! Considering the future workload, PyPOTS tutorials are released in a
+single repo, and you can find them in [BrewPOTS](https://github.com/WenjieDu/
+BrewPOTS). Take a look at it now, and learn how to brew your POTS datasets!
 _[_h_t_t_p_s_:_/_/_p_y_p_o_t_s_._c_o_m_/_f_i_g_s_/_p_y_p_o_t_s___l_o_g_o_s_/_E_c_o_s_y_s_t_e_m_/_P_y_P_O_T_S___E_c_o_s_y_s_t_e_m___P_i_p_e_l_i_n_e_._p_n_g_]
        ?â???ï?¸? WWeellccoommee ttoo tthhee uunniivveerrssee ooff PPyyPPOOTTSS.. EEnnjjooyy iitt aanndd hhaavvee ffuunn!!
 ## â Installation You can refer to [the installation instruction](https://
 docs.pypots.com/en/latest/install.html) in PyPOTS documentation for a guideline
 with more details. PyPOTS is available on both [PyPI](https://pypi.python.org/
 pypi/pypots) and [Anaconda](https://anaconda.org/conda-forge/pypots). You can
-install PyPOTS as shown below: ``` bash # via pip pip install pypots # the
-first time installation pip install pypots --upgrade # update pypots to the
-latest version # install from the latest source code with the latest features
-but may be not officially released yet pip install https://github.com/WenjieDu/
-PyPOTS/archive/main.zip # via conda conda install -c conda-forge pypots # the
-first time installation conda update -c conda-forge pypots # update pypots to
-the latest version ``` ## â Usage Besides [BrewPOTS](https://github.com/
-WenjieDu/BrewPOTS), you can also find a simple and quick-start tutorial
-notebook on Google Colab _[_C_o_l_a_b_ _t_u_t_o_r_i_a_l_s_]. If you have further questions,
-please refer to PyPOTS documentation [docs.pypots.com](https://
+install PyPOTS like below as well as TSDB and PyGrinder: ``` bash # via pip pip
+install pypots # the first time installation pip install pypots --upgrade #
+update pypots to the latest version # install from the latest source code with
+the latest features but may be not officially released yet pip install https://
+github.com/WenjieDu/PyPOTS/archive/main.zip # via conda conda install -c conda-
+forge pypots # the first time installation conda update -c conda-forge pypots #
+update pypots to the latest version ``` ## â Usage Besides [BrewPOTS](https:/
+/github.com/WenjieDu/BrewPOTS), you can also find a simple and quick-start
+tutorial notebook on Google Colab _[_C_o_l_a_b_ _t_u_t_o_r_i_a_l_s_]. If you have further
+questions, please refer to PyPOTS documentation [docs.pypots.com](https://
 docs.pypots.com). You can also [raise an issue](https://github.com/WenjieDu/
 PyPOTS/issues) or [ask in our community](#-community). We present you a usage
 example of imputing missing values in time series with PyPOTS below, you can
 click it to view. CClliicckk hheerree ttoo sseeee aann eexxaammppllee aappppllyyiinngg SSAAIITTSS oonn PPhhyyssiiooNNeett22001122
-ffoorr iimmppuuttaattiioonn:: ``` python import numpy as np from sklearn.preprocessing import
-StandardScaler from pygrinder import mcar from pypots.data import
-load_specific_dataset from pypots.imputation import SAITS from
-pypots.utils.metrics import calc_mae # Data preprocessing. Tedious, but PyPOTS
-can help. data = load_specific_dataset('physionet_2012') # PyPOTS will
-automatically download and extract it. X = data['X'] num_samples = len(X
-['RecordID'].unique()) X = X.drop(['RecordID', 'Time'], axis = 1) X =
-StandardScaler().fit_transform(X.to_numpy()) X = X.reshape(num_samples, 48, -1)
-X_ori = X # keep X_ori for validation X = mcar(X, 0.1) # randomly hold out 10%
-observed values as ground truth dataset = {"X": X} # X for model input print
-(X.shape) # (11988, 48, 37), 11988 samples and each sample has 48 time steps,
-37 features # Model training. This is PyPOTS showtime. saits = SAITS
-(n_steps=48, n_features=37, n_layers=2, d_model=256, d_ffn=128, n_heads=4,
-d_k=64, d_v=64, dropout=0.1, epochs=10) # Here I use the whole dataset as the
-training set because ground truth is not visible to the model, you can also
-split it into train/val/test sets saits.fit(dataset) imputation = saits.impute
-(dataset) # impute the originally-missing values and artificially-missing
-values indicating_mask = np.isnan(X) ^ np.isnan(X_ori) # indicating mask for
-imputation error calculation mae = calc_mae(imputation, np.nan_to_num(X_ori),
-indicating_mask) # calculate mean absolute error on the ground truth
-(artificially-missing values) ``` ## â Available Algorithms PyPOTS supports
-imputation, classification, clustering, and forecasting tasks on multivariate
-time series with missing values. The currently available algorithms of four
-tasks are cataloged in the following table with four partitions. The paper
-references are all listed at the bottom of this readme file. ð Since
-**v0.2**, all neural-network models in PyPOTS has got hyperparameter-
-optimization support. This functionality is implemented with the [Microsoft
-NNI](https://github.com/microsoft/nni) framework. ð¥ Note that Transformer,
-Crossformer, PatchTST, DLinear, ETSformer, FEDformer, Informer, Autoformer are
-not proposed as imputation methods in their original papers, and they cannot
-accept POTS as input. **To make them applicable on POTS data, we apply the
-embedding strategy and training approach (ORT+MIT) the same as we did in [SAITS
-paper](https://arxiv.org/pdf/2202.08516).** | ***`Imputation`*** | ð¥ | ð¥
-| ð¥ | |:----------------------:|:-----------:|:-----------------------------
-------------------------------------------------------------------:|:--------:
-| | **Type** | **Abbr.** | **Full name of the algorithm/model** | **Year** | |
-Neural Net | SAITS | Self-Attention-based Imputation for Time Series [^1] |
-2023 | | Neural Net | Transformer | Attention is All you Need [^2] | 2017 | |
-Neural Net | Crossformer | Transformer Utilizing Cross-Dimension Dependency for
-Multivariate Time Series Forecasting [^16] | 2023 | | Neural Net | TimesNet |
-Temporal 2D-Variation Modeling for General Time Series Analysis [^14] | 2023 |
-| Neural Net | PatchTST | A Time Series is Worth 64 Words: Long-Term
-Forecasting with Transformers [^18] | 2023 | | Neural Net | DLinear | Are
-Transformers Effective for Time Series Forecasting? [^17] | 2023 | | Neural Net
-| ETSformer | Exponential Smoothing Transformers for Time-series Forecasting
-[^19] | 2023 | | Neural Net | FEDformer | Frequency Enhanced Decomposed
-Transformer for Long-term Series Forecasting [^20] | 2022 | | Neural Net |
-Informer | Beyond Efficient Transformer for Long Sequence Time-Series
-Forecasting [^21] | 2021 | | Neural Net | Autoformer | Decomposition
-Transformers with Auto-Correlation for Long-Term Series Forecasting [^15] |
-2021 | | Neural Net | CSDI | Conditional Score-based Diffusion Models for
-Probabilistic Time Series Imputation [^12] | 2021 | | Neural Net | US-GAN |
-Unsupervised GAN for Multivariate Time Series Imputation [^10] | 2021 | |
-Neural Net | GP-VAE | Gaussian Process Variational Autoencoder [^11] | 2020 | |
-Neural Net | BRITS | Bidirectional Recurrent Imputation for Time Series [^3] |
-2018 | | Neural Net | M-RNN | Multi-directional Recurrent Neural Network [^9] |
-2019 | | Naive | LOCF/NOCB | Last Observation Carried Forward / Next
-Observation Carried Backward | - | | Naive | Median | Median Value Imputation |
-- | | Naive | Mean | Mean Value Imputation | - | | ***`Classification`*** |
-ð¥ | ð¥ | ð¥ | | **Type** | **Abbr.** | **Full name of the algorithm/
-model/paper** | **Year** | | Neural Net | BRITS | Bidirectional Recurrent
-Imputation for Time Series [^3] | 2018 | | Neural Net | GRU-D | Recurrent
-Neural Networks for Multivariate Time Series with Missing Values [^4] | 2018 |
-| Neural Net | Raindrop | Graph-Guided Network for Irregularly Sampled
-Multivariate Time Series [^5] | 2022 | | ***`Clustering`*** | ð¥ | ð¥ |
-ð¥ | | **Type** | **Abbr.** | **Full name of the algorithm/model/paper** |
-**Year** | | Neural Net | CRLI | Clustering Representation Learning on
-Incomplete time-series data [^6] | 2021 | | Neural Net | VaDER | Variational
-Deep Embedding with Recurrence [^7] | 2019 | | ***`Forecasting`*** | ð¥ |
-ð¥ | ð¥ | | **Type** | **Abbr.** | **Full name of the algorithm/model/
-paper** | **Year** | | Probabilistic | BTTF | Bayesian Temporal Tensor
-Factorization [^8] | 2021 | ## â Citing PyPOTS > [!TIP] > **[Updates in Feb
-2024]** ð Our survey paper [Deep Learning for Multivariate Time Series
-Imputation: A Survey](https://arxiv.org/abs/2402.04059) has been released on
-arXiv. The code is open source in the GitHub repo [Awesome_Imputation](https://
-github.com/WenjieDu/Awesome_Imputation). We comprehensively review the
-literature of the state-of-the-art deep-learning imputation methods for time
-series, provide a taxonomy for them, and discuss the challenges and future
-directions in this field. > > **[Updates in Jun 2023]** ð A short version of
-the PyPOTS paper is accepted by the 9th SIGKDD international workshop on Mining
-and Learning from Time Series ([MiLeTS'23](https://kdd-milets.github.io/
-milets2023/))). **Additionally**, PyPOTS has been included as a [PyTorch
-Ecosystem](https://pytorch.org/ecosystem/) project. The paper introducing
-PyPOTS is available on arXiv at [this URL](https://arxiv.org/abs/2305.18811),
-and we are pursuing to publish it in prestigious academic venues, e.g. JMLR
-(track for [Machine Learning Open Source Software](https://www.jmlr.org/mloss/
-)). If you use PyPOTS in your work, please cite it as below and ðstar this
-repository to make others notice this library. ð¤ There are scientific
-research projects using PyPOTS and referencing in their papers. Here is [an
-incomplete list of them](https://scholar.google.com/
+ffoorr iimmppuuttaattiioonn:: ``` python # Data preprocessing. Tedious, but PyPOTS can help.
+import numpy as np from sklearn.preprocessing import StandardScaler from
+pygrinder import mcar from pypots.data import load_specific_dataset data =
+load_specific_dataset('physionet_2012') # PyPOTS will automatically download
+and extract it. X = data['X'] num_samples = len(X['RecordID'].unique()) X =
+X.drop(['RecordID', 'Time'], axis = 1) X = StandardScaler().fit_transform
+(X.to_numpy()) X = X.reshape(num_samples, 48, -1) X_ori = X # keep X_ori for
+validation X = mcar(X, 0.1) # randomly hold out 10% observed values as ground
+truth dataset = {"X": X} # X for model input print(X.shape) # (11988, 48, 37),
+11988 samples and each sample has 48 time steps, 37 features # Model training.
+This is PyPOTS showtime. from pypots.imputation import SAITS from
+pypots.utils.metrics import calc_mae saits = SAITS(n_steps=48, n_features=37,
+n_layers=2, d_model=256, n_heads=4, d_k=64, d_v=64, d_ffn=128, dropout=0.1,
+epochs=10) # Here I use the whole dataset as the training set because ground
+truth is not visible to the model, you can also split it into train/val/test
+sets saits.fit(dataset) # train the model on the dataset imputation =
+saits.impute(dataset) # impute the originally-missing values and artificially-
+missing values indicating_mask = np.isnan(X) ^ np.isnan(X_ori) # indicating
+mask for imputation error calculation mae = calc_mae(imputation, np.nan_to_num
+(X_ori), indicating_mask) # calculate mean absolute error on the ground truth
+(artificially-missing values) saits.save("save_it_here/
+saits_physionet2012.pypots") # save the model for future use saits.load
+("save_it_here/saits_physionet2012.pypots") # reload the serialized model file
+for following imputation or training ``` ## â Citing PyPOTS > [!TIP] > **
+[Updates in Feb 2024]** ð Our survey paper [Deep Learning for Multivariate
+Time Series Imputation: A Survey](https://arxiv.org/abs/2402.04059) has been
+released on arXiv. The code is open source in the GitHub repo
+[Awesome_Imputation](https://github.com/WenjieDu/Awesome_Imputation). We
+comprehensively review the literature of the state-of-the-art deep-learning
+imputation methods for time series, provide a taxonomy for them, and discuss
+the challenges and future directions in this field. > > **[Updates in Jun
+2023]** ð A short version of the PyPOTS paper is accepted by the 9th SIGKDD
+international workshop on Mining and Learning from Time Series ([MiLeTS'23]
+(https://kdd-milets.github.io/milets2023/))). **Additionally**, PyPOTS has been
+included as a [PyTorch Ecosystem](https://pytorch.org/ecosystem/) project. The
+paper introducing PyPOTS is available on arXiv at [this URL](https://arxiv.org/
+abs/2305.18811), and we are pursuing to publish it in prestigious academic
+venues, e.g. JMLR (track for [Machine Learning Open Source Software](https://
+www.jmlr.org/mloss/)). If you use PyPOTS in your work, please cite it as below
+and ðstar this repository to make others notice this library. ð¤ There are
+scientific research projects using PyPOTS and referencing in their papers. Here
+is [an incomplete list of them](https://scholar.google.com/
 scholar?as_ylo=2022&q=%E2%80%9CPyPOTS%E2%80%9D&hl=en>). ``` bibtex @article
 {du2023pypots, title={{PyPOTS: a Python toolbox for data mining on Partially-
 Observed Time Series}}, author={Wenjie Du}, year={2023}, eprint={2305.18811},
 archivePrefix={arXiv}, primaryClass={cs.LG}, url={https://arxiv.org/abs/
 2305.18811}, doi={10.48550/arXiv.2305.18811}, } ``` or > Wenjie Du. (2023). >
 PyPOTS: a Python toolbox for data mining on Partially-Observed Time Series. >
 arXiv, abs/2305.18811.https://arxiv.org/abs/2305.18811 ## â Contribution
@@ -276,9 +245,20 @@
 Exponential Smoothing Transformers for Time-series Forecasting](https://
 openreview.net/forum?id=5m_3whfo483). *ICLR 2023* [^20]: Zhou, T., Ma, Z., Wen,
 Q., Wang, X., Sun, L., & Jin, R. (2022). [FEDformer: Frequency enhanced
 decomposed transformer for long-term series forecasting](https://
 proceedings.mlr.press/v162/zhou22g.html). *ICML 2022*. [^21]: Zhou, H., Zhang,
 S., Peng, J., Zhang, S., Li, J., Xiong, H., & Zhang, W. (2021). [Informer:
 Beyond efficient transformer for long sequence time-series forecasting](https:/
-/ojs.aaai.org/index.php/AAAI/article/view/17325). *AAAI 2021*. ð  Visits
-_[_P_y_P_O_T_S_ _v_i_s_i_t_s_]
+/ojs.aaai.org/index.php/AAAI/article/view/17325). *AAAI 2021*. [^22]: Zhou, T.,
+Ma, Z., Wen, Q., Sun, L., Yao, T., Yin, W., & Jin, R. (2022). [FiLM: Frequency
+improved Legendre Memory Model for Long-term Time Series Forecasting](https://
+proceedings.neurips.cc/paper_files/paper/2022/hash/
+524ef58c2bd075775861234266e5e020-Abstract-Conference.html). *NeurIPS 2022*.
+[^23]: Yi, K., Zhang, Q., Fan, W., Wang, S., Wang, P., He, H., An, N., Lian,
+D., Cao, L., & Niu, Z. (2024). [Frequency-domain MLPs are More Effective
+Learners in Time Series Forecasting](https://proceedings.neurips.cc/
+paper_files/paper/2023/hash/f1d16af76939f476b5f040fd1398c0a3-Abstract-
+Conference.html). *NeurIPS 2024*. [^24]: Liu, Y., Hu, T., Zhang, H., Wu, H.,
+Wang, S., Ma, L., & Long, M. (2024). [iTransformer: Inverted Transformers Are
+Effective for Time Series Forecasting](https://openreview.net/
+forum?id=JePfAI8fah). *ICLR 2024*. ð  Visits_[_P_y_P_O_T_S_ _v_i_s_i_t_s_]
```

### Comparing `pypots-0.4.1/pypots.egg-info/SOURCES.txt` & `pypots-0.5/pypots.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -40,29 +40,35 @@
 pypots/clustering/crli/data.py
 pypots/clustering/crli/model.py
 pypots/clustering/vader/__init__.py
 pypots/clustering/vader/core.py
 pypots/clustering/vader/data.py
 pypots/clustering/vader/model.py
 pypots/data/__init__.py
-pypots/data/base.py
 pypots/data/checking.py
 pypots/data/generating.py
 pypots/data/load_preprocessing.py
 pypots/data/load_specific_datasets.py
 pypots/data/utils.py
+pypots/data/dataset/__init__.py
+pypots/data/dataset/base.py
+pypots/data/dataset/config.py
 pypots/data/saving/__init__.py
 pypots/data/saving/h5.py
 pypots/data/saving/pickle.py
 pypots/forecasting/__init__.py
 pypots/forecasting/base.py
 pypots/forecasting/bttf/__init__.py
 pypots/forecasting/bttf/core.py
 pypots/forecasting/bttf/model.py
 pypots/forecasting/bttf/submodules.py
+pypots/forecasting/csdi/__init__.py
+pypots/forecasting/csdi/core.py
+pypots/forecasting/csdi/data.py
+pypots/forecasting/csdi/model.py
 pypots/imputation/__init__.py
 pypots/imputation/base.py
 pypots/imputation/autoformer/__init__.py
 pypots/imputation/autoformer/core.py
 pypots/imputation/autoformer/data.py
 pypots/imputation/autoformer/model.py
 pypots/imputation/brits/__init__.py
@@ -85,22 +91,34 @@
 pypots/imputation/etsformer/core.py
 pypots/imputation/etsformer/data.py
 pypots/imputation/etsformer/model.py
 pypots/imputation/fedformer/__init__.py
 pypots/imputation/fedformer/core.py
 pypots/imputation/fedformer/data.py
 pypots/imputation/fedformer/model.py
+pypots/imputation/film/__init__.py
+pypots/imputation/film/core.py
+pypots/imputation/film/data.py
+pypots/imputation/film/model.py
+pypots/imputation/frets/__init__.py
+pypots/imputation/frets/core.py
+pypots/imputation/frets/data.py
+pypots/imputation/frets/model.py
 pypots/imputation/gpvae/__init__.py
 pypots/imputation/gpvae/core.py
 pypots/imputation/gpvae/data.py
 pypots/imputation/gpvae/model.py
 pypots/imputation/informer/__init__.py
 pypots/imputation/informer/core.py
 pypots/imputation/informer/data.py
 pypots/imputation/informer/model.py
+pypots/imputation/itransformer/__init__.py
+pypots/imputation/itransformer/core.py
+pypots/imputation/itransformer/data.py
+pypots/imputation/itransformer/model.py
 pypots/imputation/locf/__init__.py
 pypots/imputation/locf/core.py
 pypots/imputation/locf/model.py
 pypots/imputation/mean/__init__.py
 pypots/imputation/mean/model.py
 pypots/imputation/median/__init__.py
 pypots/imputation/median/model.py
@@ -129,63 +147,69 @@
 pypots/imputation/usgan/data.py
 pypots/imputation/usgan/model.py
 pypots/nn/__init__.py
 pypots/nn/functional/__init__.py
 pypots/nn/functional/normalization.py
 pypots/nn/modules/__init__.py
 pypots/nn/modules/autoformer/__init__.py
-pypots/nn/modules/autoformer/auto_encoder.py
+pypots/nn/modules/autoformer/autoencoder.py
 pypots/nn/modules/autoformer/layers.py
 pypots/nn/modules/brits/__init__.py
 pypots/nn/modules/brits/backbone.py
 pypots/nn/modules/brits/layers.py
 pypots/nn/modules/crli/__init__.py
 pypots/nn/modules/crli/backbone.py
 pypots/nn/modules/crli/layers.py
 pypots/nn/modules/crossformer/__init__.py
-pypots/nn/modules/crossformer/auto_encoder.py
+pypots/nn/modules/crossformer/autoencoder.py
 pypots/nn/modules/crossformer/layers.py
 pypots/nn/modules/csdi/__init__.py
 pypots/nn/modules/csdi/backbone.py
 pypots/nn/modules/csdi/layers.py
 pypots/nn/modules/dlinear/__init__.py
 pypots/nn/modules/dlinear/backbone.py
 pypots/nn/modules/etsformer/__init__.py
-pypots/nn/modules/etsformer/auto_encoder.py
+pypots/nn/modules/etsformer/autoencoder.py
 pypots/nn/modules/etsformer/layers.py
 pypots/nn/modules/fedformer/__init__.py
 pypots/nn/modules/fedformer/autoencoder.py
 pypots/nn/modules/fedformer/layers.py
+pypots/nn/modules/film/__init__.py
+pypots/nn/modules/film/backbone.py
+pypots/nn/modules/film/layers.py
+pypots/nn/modules/frets/__init__.py
+pypots/nn/modules/frets/backbone.py
 pypots/nn/modules/gpvae/__init__.py
 pypots/nn/modules/gpvae/backbone.py
 pypots/nn/modules/gpvae/layers.py
 pypots/nn/modules/grud/__init__.py
 pypots/nn/modules/grud/backbone.py
 pypots/nn/modules/grud/layers.py
 pypots/nn/modules/informer/__init__.py
-pypots/nn/modules/informer/auto_encoder.py
+pypots/nn/modules/informer/autoencoder.py
 pypots/nn/modules/informer/layers.py
 pypots/nn/modules/mrnn/__init__.py
 pypots/nn/modules/mrnn/backbone.py
 pypots/nn/modules/mrnn/layers.py
 pypots/nn/modules/patchtst/__init__.py
-pypots/nn/modules/patchtst/auto_encoder.py
+pypots/nn/modules/patchtst/autoencoder.py
 pypots/nn/modules/patchtst/layers.py
 pypots/nn/modules/raindrop/__init__.py
 pypots/nn/modules/raindrop/backbone.py
 pypots/nn/modules/raindrop/layers.py
 pypots/nn/modules/saits/__init__.py
 pypots/nn/modules/saits/backbone.py
+pypots/nn/modules/saits/embedding.py
 pypots/nn/modules/saits/loss.py
 pypots/nn/modules/timesnet/__init__.py
 pypots/nn/modules/timesnet/backbone.py
 pypots/nn/modules/timesnet/layers.py
 pypots/nn/modules/transformer/__init__.py
 pypots/nn/modules/transformer/attention.py
-pypots/nn/modules/transformer/auto_encoder.py
+pypots/nn/modules/transformer/autoencoder.py
 pypots/nn/modules/transformer/embedding.py
 pypots/nn/modules/transformer/layers.py
 pypots/nn/modules/usgan/__init__.py
 pypots/nn/modules/usgan/backbone.py
 pypots/nn/modules/usgan/layers.py
 pypots/nn/modules/vader/__init__.py
 pypots/nn/modules/vader/backbone.py
```

### Comparing `pypots-0.4.1/pypots.egg-info/requires.txt` & `pypots-0.5/pypots.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `pypots-0.4.1/setup.cfg` & `pypots-0.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `pypots-0.4.1/setup.py` & `pypots-0.5/setup.py`

 * *Files identical despite different names*

