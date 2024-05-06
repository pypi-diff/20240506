# Comparing `tmp/zeus-ml-0.8.2.tar.gz` & `tmp/zeus_ml-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zeus-ml-0.8.2.tar", last modified: Mon Feb 26 23:58:43 2024, max compression
+gzip compressed data, was "zeus_ml-0.9.0.tar", last modified: Mon May  6 15:51:24 2024, max compression
```

## Comparing `zeus-ml-0.8.2.tar` & `zeus_ml-0.9.0.tar`

### file list

```diff
@@ -1,111 +1,128 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 23:58:43.526227 zeus-ml-0.8.2/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-02-26 23:58:35.000000 zeus-ml-0.8.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     9722 2024-02-26 23:58:43.526227 zeus-ml-0.8.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8133 2024-02-26 23:58:35.000000 zeus-ml-0.8.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 23:58:43.506227 zeus-ml-0.8.2/capriccio/
--rw-r--r--   0 runner    (1001) docker     (127)     3637 2024-02-26 23:58:35.000000 zeus-ml-0.8.2/capriccio/generate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 23:58:43.506227 zeus-ml-0.8.2/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     1741 2024-02-26 23:58:35.000000 zeus-ml-0.8.2/docs/gen_ref_pages.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 23:58:43.506227 zeus-ml-0.8.2/examples/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 23:58:43.506227 zeus-ml-0.8.2/examples/ZeusDataLoader/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 23:58:43.506227 zeus-ml-0.8.2/examples/ZeusDataLoader/capriccio/
--rw-r--r--   0 runner    (1001) docker     (127)     7844 2024-02-26 23:58:35.000000 zeus-ml-0.8.2/examples/ZeusDataLoader/capriccio/run_zeus.py
--rw-r--r--   0 runner    (1001) docker     (127)    12571 2024-02-26 23:58:35.000000 zeus-ml-0.8.2/examples/ZeusDataLoader/capriccio/train.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 23:58:43.510227 zeus-ml-0.8.2/examples/ZeusDataLoader/cifar100/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 23:58:43.514227 zeus-ml-0.8.2/examples/ZeusDataLoader/cifar100/models/
--rw-r--r--   0 runner    (1001) docker     (127)     6602 2024-02-26 23:58:35.000000 zeus-ml-0.8.2/examples/ZeusDataLoader/cifar100/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11757 2024-02-26 23:58:35.000000 zeus-ml-0.8.2/examples/ZeusDataLoader/cifar100/models/attention.py
--rw-r--r--   0 runner    (1001) docker     (127)     5086 2024-02-26 23:58:35.000000 zeus-ml-0.8.2/examples/ZeusDataLoader/cifar100/models/densenet.py
--rw-r--r--   0 runner    (1001) docker     (127)     4493 2024-02-26 23:58:35.000000 zeus-ml-0.8.2/examples/ZeusDataLoader/cifar100/models/googlenet.py
--rw-r--r--   0 runner    (1001) docker     (127)    10880 2024-02-26 23:58:35.000000 zeus-ml-0.8.2/examples/ZeusDataLoader/cifar100/models/inceptionv3.py
--rw-r--r--   0 runner    (1001) docker     (127)    18107 2024-02-26 23:58:35.000000 zeus-ml-0.8.2/examples/ZeusDataLoader/cifar100/models/inceptionv4.py
--rw-r--r--   0 runner    (1001) docker     (127)     5318 2024-02-26 23:58:35.000000 zeus-ml-0.8.2/examples/ZeusDataLoader/cifar100/models/mobilenet.py
--rw-r--r--   0 runner    (1001) docker     (127)     2817 2024-02-26 23:58:35.000000 zeus-ml-0.8.2/examples/ZeusDataLoader/cifar100/models/mobilenetv2.py
--rw-r--r--   0 runner    (1001) docker     (127)     9594 2024-02-26 23:58:35.000000 zeus-ml-0.8.2/examples/ZeusDataLoader/cifar100/models/nasnet.py
--rw-r--r--   0 runner    (1001) docker     (127)     3897 2024-02-26 23:58:35.000000 zeus-ml-0.8.2/examples/ZeusDataLoader/cifar100/models/preactresnet.py
--rw-r--r--   0 runner    (1001) docker     (127)     5479 2024-02-26 23:58:35.000000 zeus-ml-0.8.2/examples/ZeusDataLoader/cifar100/models/resnet.py
--rw-r--r--   0 runner    (1001) docker     (127)     4199 2024-02-26 23:58:35.000000 zeus-ml-0.8.2/examples/ZeusDataLoader/cifar100/models/resnext.py
--rw-r--r--   0 runner    (1001) docker     (127)     7042 2024-02-26 23:58:35.000000 zeus-ml-0.8.2/examples/ZeusDataLoader/cifar100/models/rir.py
--rw-r--r--   0 runner    (1001) docker     (127)     5231 2024-02-26 23:58:35.000000 zeus-ml-0.8.2/examples/ZeusDataLoader/cifar100/models/senet.py
--rw-r--r--   0 runner    (1001) docker     (127)     7439 2024-02-26 23:58:35.000000 zeus-ml-0.8.2/examples/ZeusDataLoader/cifar100/models/shufflenet.py
--rw-r--r--   0 runner    (1001) docker     (127)     4794 2024-02-26 23:58:35.000000 zeus-ml-0.8.2/examples/ZeusDataLoader/cifar100/models/shufflenetv2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2447 2024-02-26 23:58:35.000000 zeus-ml-0.8.2/examples/ZeusDataLoader/cifar100/models/squeezenet.py
--rw-r--r--   0 runner    (1001) docker     (127)     7516 2024-02-26 23:58:35.000000 zeus-ml-0.8.2/examples/ZeusDataLoader/cifar100/models/stochasticdepth.py
--rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-02-26 23:58:35.000000 zeus-ml-0.8.2/examples/ZeusDataLoader/cifar100/models/vgg.py
--rw-r--r--   0 runner    (1001) docker     (127)     3255 2024-02-26 23:58:35.000000 zeus-ml-0.8.2/examples/ZeusDataLoader/cifar100/models/wideresidual.py
--rw-r--r--   0 runner    (1001) docker     (127)     6112 2024-02-26 23:58:35.000000 zeus-ml-0.8.2/examples/ZeusDataLoader/cifar100/models/xception.py
--rw-r--r--   0 runner    (1001) docker     (127)     7730 2024-02-26 23:58:35.000000 zeus-ml-0.8.2/examples/ZeusDataLoader/cifar100/run_zeus.py
--rw-r--r--   0 runner    (1001) docker     (127)     6588 2024-02-26 23:58:35.000000 zeus-ml-0.8.2/examples/ZeusDataLoader/cifar100/train.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 23:58:43.514227 zeus-ml-0.8.2/examples/ZeusDataLoader/imagenet/
--rw-r--r--   0 runner    (1001) docker     (127)     6810 2024-02-26 23:58:35.000000 zeus-ml-0.8.2/examples/ZeusDataLoader/imagenet/run_zeus.py
--rw-r--r--   0 runner    (1001) docker     (127)    28066 2024-02-26 23:58:35.000000 zeus-ml-0.8.2/examples/ZeusDataLoader/imagenet/train.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 23:58:43.514227 zeus-ml-0.8.2/examples/huggingface/
--rw-r--r--   0 runner    (1001) docker     (127)    30274 2024-02-26 23:58:35.000000 zeus-ml-0.8.2/examples/huggingface/run_clm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 23:58:43.514227 zeus-ml-0.8.2/examples/imagenet/
--rw-r--r--   0 runner    (1001) docker     (127)    12578 2024-02-26 23:58:35.000000 zeus-ml-0.8.2/examples/imagenet/train_dp.py
--rw-r--r--   0 runner    (1001) docker     (127)    11646 2024-02-26 23:58:35.000000 zeus-ml-0.8.2/examples/imagenet/train_single.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 23:58:43.514227 zeus-ml-0.8.2/examples/perseus/
--rw-r--r--   0 runner    (1001) docker     (127)     2202 2024-02-26 23:58:35.000000 zeus-ml-0.8.2/examples/perseus/profile_p2p.py
--rw-r--r--   0 runner    (1001) docker     (127)     8634 2024-02-26 23:58:35.000000 zeus-ml-0.8.2/examples/perseus/run_optimization.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 23:58:43.514227 zeus-ml-0.8.2/examples/trace_driven/
--rw-r--r--   0 runner    (1001) docker     (127)     5259 2024-02-26 23:58:35.000000 zeus-ml-0.8.2/examples/trace_driven/run_alibaba.py
--rw-r--r--   0 runner    (1001) docker     (127)     3888 2024-02-26 23:58:35.000000 zeus-ml-0.8.2/examples/trace_driven/run_single.py
--rw-r--r--   0 runner    (1001) docker     (127)     2571 2024-02-26 23:58:35.000000 zeus-ml-0.8.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-26 23:58:43.526227 zeus-ml-0.8.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 23:58:43.514227 zeus-ml-0.8.2/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 23:58:43.514227 zeus-ml-0.8.2/tests/optimizer/
--rw-r--r--   0 runner    (1001) docker     (127)    10776 2024-02-26 23:58:35.000000 zeus-ml-0.8.2/tests/optimizer/test_power_limit_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4091 2024-02-26 23:58:35.000000 zeus-ml-0.8.2/tests/test_batch_size_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)    16819 2024-02-26 23:58:35.000000 zeus-ml-0.8.2/tests/test_monitor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 23:58:43.514227 zeus-ml-0.8.2/tests/util/
--rw-r--r--   0 runner    (1001) docker     (127)     2714 2024-02-26 23:58:35.000000 zeus-ml-0.8.2/tests/util/test_env.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 23:58:43.518227 zeus-ml-0.8.2/zeus/
--rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-02-26 23:58:35.000000 zeus-ml-0.8.2/zeus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4215 2024-02-26 23:58:35.000000 zeus-ml-0.8.2/zeus/analyze.py
--rw-r--r--   0 runner    (1001) docker     (127)     3455 2024-02-26 23:58:35.000000 zeus-ml-0.8.2/zeus/callback.py
--rw-r--r--   0 runner    (1001) docker     (127)     6779 2024-02-26 23:58:35.000000 zeus-ml-0.8.2/zeus/controller.py
--rw-r--r--   0 runner    (1001) docker     (127)     5012 2024-02-26 23:58:35.000000 zeus-ml-0.8.2/zeus/job.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 23:58:43.518227 zeus-ml-0.8.2/zeus/monitor/
--rw-r--r--   0 runner    (1001) docker     (127)      910 2024-02-26 23:58:35.000000 zeus-ml-0.8.2/zeus/monitor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4257 2024-02-26 23:58:35.000000 zeus-ml-0.8.2/zeus/monitor/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13588 2024-02-26 23:58:35.000000 zeus-ml-0.8.2/zeus/monitor/energy.py
--rw-r--r--   0 runner    (1001) docker     (127)     9719 2024-02-26 23:58:35.000000 zeus-ml-0.8.2/zeus/monitor/power.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 23:58:43.518227 zeus-ml-0.8.2/zeus/optimizer/
--rw-r--r--   0 runner    (1001) docker     (127)      763 2024-02-26 23:58:35.000000 zeus-ml-0.8.2/zeus/optimizer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 23:58:43.518227 zeus-ml-0.8.2/zeus/optimizer/perseus/
--rw-r--r--   0 runner    (1001) docker     (127)      778 2024-02-26 23:58:35.000000 zeus-ml-0.8.2/zeus/optimizer/perseus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11661 2024-02-26 23:58:35.000000 zeus-ml-0.8.2/zeus/optimizer/perseus/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     3257 2024-02-26 23:58:35.000000 zeus-ml-0.8.2/zeus/optimizer/perseus/frequency_controller.py
--rw-r--r--   0 runner    (1001) docker     (127)     9068 2024-02-26 23:58:35.000000 zeus-ml-0.8.2/zeus/optimizer/perseus/optimizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 23:58:43.518227 zeus-ml-0.8.2/zeus/optimizer/perseus/server/
--rw-r--r--   0 runner    (1001) docker     (127)      997 2024-02-26 23:58:35.000000 zeus-ml-0.8.2/zeus/optimizer/perseus/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9492 2024-02-26 23:58:35.000000 zeus-ml-0.8.2/zeus/optimizer/perseus/server/job_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     3767 2024-02-26 23:58:35.000000 zeus-ml-0.8.2/zeus/optimizer/perseus/server/router.py
--rw-r--r--   0 runner    (1001) docker     (127)    12182 2024-02-26 23:58:35.000000 zeus-ml-0.8.2/zeus/optimizer/perseus/server/scheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)    22804 2024-02-26 23:58:35.000000 zeus-ml-0.8.2/zeus/optimizer/power_limit.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 23:58:43.522227 zeus-ml-0.8.2/zeus/policy/
--rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-02-26 23:58:35.000000 zeus-ml-0.8.2/zeus/policy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3888 2024-02-26 23:58:35.000000 zeus-ml-0.8.2/zeus/policy/interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     6664 2024-02-26 23:58:35.000000 zeus-ml-0.8.2/zeus/policy/mab.py
--rw-r--r--   0 runner    (1001) docker     (127)    19915 2024-02-26 23:58:35.000000 zeus-ml-0.8.2/zeus/policy/optimizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 23:58:43.522227 zeus-ml-0.8.2/zeus/run/
--rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-02-26 23:58:35.000000 zeus-ml-0.8.2/zeus/run/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    48989 2024-02-26 23:58:35.000000 zeus-ml-0.8.2/zeus/run/dataloader.py
--rw-r--r--   0 runner    (1001) docker     (127)    15134 2024-02-26 23:58:35.000000 zeus-ml-0.8.2/zeus/run/master.py
--rw-r--r--   0 runner    (1001) docker     (127)    36483 2024-02-26 23:58:35.000000 zeus-ml-0.8.2/zeus/simulate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 23:58:43.522227 zeus-ml-0.8.2/zeus/util/
--rw-r--r--   0 runner    (1001) docker     (127)      854 2024-02-26 23:58:35.000000 zeus-ml-0.8.2/zeus/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2022 2024-02-26 23:58:35.000000 zeus-ml-0.8.2/zeus/util/async_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3133 2024-02-26 23:58:35.000000 zeus-ml-0.8.2/zeus/util/env.py
--rw-r--r--   0 runner    (1001) docker     (127)     1783 2024-02-26 23:58:35.000000 zeus-ml-0.8.2/zeus/util/framework.py
--rw-r--r--   0 runner    (1001) docker     (127)     1878 2024-02-26 23:58:35.000000 zeus-ml-0.8.2/zeus/util/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-02-26 23:58:35.000000 zeus-ml-0.8.2/zeus/util/lr_scaler.py
--rw-r--r--   0 runner    (1001) docker     (127)     3002 2024-02-26 23:58:35.000000 zeus-ml-0.8.2/zeus/util/metric.py
--rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-02-26 23:58:35.000000 zeus-ml-0.8.2/zeus/util/pydantic_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)     6813 2024-02-26 23:58:35.000000 zeus-ml-0.8.2/zeus/util/testing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 23:58:43.522227 zeus-ml-0.8.2/zeus_ml.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9722 2024-02-26 23:58:43.000000 zeus-ml-0.8.2/zeus_ml.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2890 2024-02-26 23:58:43.000000 zeus-ml-0.8.2/zeus_ml.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-26 23:58:43.000000 zeus-ml-0.8.2/zeus_ml.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-02-26 23:58:43.000000 zeus-ml-0.8.2/zeus_ml.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-02-26 23:58:43.000000 zeus-ml-0.8.2/zeus_ml.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:51:24.052604 zeus_ml-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-06 15:51:18.000000 zeus_ml-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7584 2024-05-06 15:51:24.052604 zeus_ml-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4419 2024-05-06 15:51:18.000000 zeus_ml-0.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:51:24.028604 zeus_ml-0.9.0/capriccio/
+-rw-r--r--   0 runner    (1001) docker     (127)     3637 2024-05-06 15:51:18.000000 zeus_ml-0.9.0/capriccio/generate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:51:24.028604 zeus_ml-0.9.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1864 2024-05-06 15:51:18.000000 zeus_ml-0.9.0/docs/gen_ref_pages.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:51:24.024604 zeus_ml-0.9.0/examples/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:51:24.024604 zeus_ml-0.9.0/examples/batch_size_optimizer/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:51:24.028604 zeus_ml-0.9.0/examples/batch_size_optimizer/capriccio/
+-rw-r--r--   0 runner    (1001) docker     (127)    12726 2024-05-06 15:51:19.000000 zeus_ml-0.9.0/examples/batch_size_optimizer/capriccio/train.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:51:24.028604 zeus_ml-0.9.0/examples/batch_size_optimizer/mnist/
+-rw-r--r--   0 runner    (1001) docker     (127)     9613 2024-05-06 15:51:19.000000 zeus_ml-0.9.0/examples/batch_size_optimizer/mnist/train_dp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8093 2024-05-06 15:51:19.000000 zeus_ml-0.9.0/examples/batch_size_optimizer/mnist/train_single_gpu.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:51:24.028604 zeus_ml-0.9.0/examples/huggingface/
+-rw-r--r--   0 runner    (1001) docker     (127)    30412 2024-05-06 15:51:19.000000 zeus_ml-0.9.0/examples/huggingface/run_clm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5662 2024-05-06 15:51:19.000000 zeus_ml-0.9.0/examples/huggingface/run_gemma_sft_qlora.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:51:24.028604 zeus_ml-0.9.0/examples/pipeline_frequency_optimizer/
+-rw-r--r--   0 runner    (1001) docker     (127)     2202 2024-05-06 15:51:19.000000 zeus_ml-0.9.0/examples/pipeline_frequency_optimizer/profile_p2p.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8640 2024-05-06 15:51:19.000000 zeus_ml-0.9.0/examples/pipeline_frequency_optimizer/run_optimization.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:51:24.028604 zeus_ml-0.9.0/examples/power_limit_optimizer/
+-rw-r--r--   0 runner    (1001) docker     (127)    12553 2024-05-06 15:51:19.000000 zeus_ml-0.9.0/examples/power_limit_optimizer/train_dp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11621 2024-05-06 15:51:19.000000 zeus_ml-0.9.0/examples/power_limit_optimizer/train_single.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:51:24.024604 zeus_ml-0.9.0/examples/research_reproducibility/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:51:24.032604 zeus_ml-0.9.0/examples/research_reproducibility/zeus_nsdi23/
+-rw-r--r--   0 runner    (1001) docker     (127)     5369 2024-05-06 15:51:19.000000 zeus_ml-0.9.0/examples/research_reproducibility/zeus_nsdi23/run_alibaba.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3901 2024-05-06 15:51:19.000000 zeus_ml-0.9.0/examples/research_reproducibility/zeus_nsdi23/run_single.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3588 2024-05-06 15:51:19.000000 zeus_ml-0.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 15:51:24.052604 zeus_ml-0.9.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:51:24.032604 zeus_ml-0.9.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:51:24.032604 zeus_ml-0.9.0/tests/optimizer/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:51:24.032604 zeus_ml-0.9.0/tests/optimizer/batch_size/
+-rw-r--r--   0 runner    (1001) docker     (127)     2799 2024-05-06 15:51:19.000000 zeus_ml-0.9.0/tests/optimizer/batch_size/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20383 2024-05-06 15:51:19.000000 zeus_ml-0.9.0/tests/optimizer/batch_size/simulate_with_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5546 2024-05-06 15:51:19.000000 zeus_ml-0.9.0/tests/optimizer/batch_size/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6857 2024-05-06 15:51:19.000000 zeus_ml-0.9.0/tests/optimizer/batch_size/test_explorer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11531 2024-05-06 15:51:19.000000 zeus_ml-0.9.0/tests/optimizer/batch_size/test_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4307 2024-05-06 15:51:19.000000 zeus_ml-0.9.0/tests/optimizer/batch_size/test_simulator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11018 2024-05-06 15:51:19.000000 zeus_ml-0.9.0/tests/optimizer/test_power_limit_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17477 2024-05-06 15:51:19.000000 zeus_ml-0.9.0/tests/test_monitor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:51:24.032604 zeus_ml-0.9.0/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     2715 2024-05-06 15:51:19.000000 zeus_ml-0.9.0/tests/utils/test_env.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:51:24.032604 zeus_ml-0.9.0/zeus/
+-rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-05-06 15:51:19.000000 zeus_ml-0.9.0/zeus/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:51:24.032604 zeus_ml-0.9.0/zeus/_legacy/
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-06 15:51:19.000000 zeus_ml-0.9.0/zeus/_legacy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5031 2024-05-06 15:51:19.000000 zeus_ml-0.9.0/zeus/_legacy/job.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:51:24.036605 zeus_ml-0.9.0/zeus/_legacy/policy/
+-rw-r--r--   0 runner    (1001) docker     (127)     1185 2024-05-06 15:51:19.000000 zeus_ml-0.9.0/zeus/_legacy/policy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3928 2024-05-06 15:51:19.000000 zeus_ml-0.9.0/zeus/_legacy/policy/interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6664 2024-05-06 15:51:19.000000 zeus_ml-0.9.0/zeus/_legacy/policy/mab.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19971 2024-05-06 15:51:19.000000 zeus_ml-0.9.0/zeus/_legacy/policy/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36929 2024-05-06 15:51:19.000000 zeus_ml-0.9.0/zeus/_legacy/simulate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3455 2024-05-06 15:51:19.000000 zeus_ml-0.9.0/zeus/callback.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:51:24.036605 zeus_ml-0.9.0/zeus/device/
+-rw-r--r--   0 runner    (1001) docker     (127)     4083 2024-05-06 15:51:19.000000 zeus_ml-0.9.0/zeus/device/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-06 15:51:19.000000 zeus_ml-0.9.0/zeus/device/exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37348 2024-05-06 15:51:19.000000 zeus_ml-0.9.0/zeus/device/gpu.py
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-05-06 15:51:19.000000 zeus_ml-0.9.0/zeus/exception.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:51:24.036605 zeus_ml-0.9.0/zeus/monitor/
+-rw-r--r--   0 runner    (1001) docker     (127)      910 2024-05-06 15:51:19.000000 zeus_ml-0.9.0/zeus/monitor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4257 2024-05-06 15:51:19.000000 zeus_ml-0.9.0/zeus/monitor/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12713 2024-05-06 15:51:19.000000 zeus_ml-0.9.0/zeus/monitor/energy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9625 2024-05-06 15:51:19.000000 zeus_ml-0.9.0/zeus/monitor/power.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:51:24.036605 zeus_ml-0.9.0/zeus/optimizer/
+-rw-r--r--   0 runner    (1001) docker     (127)      633 2024-05-06 15:51:19.000000 zeus_ml-0.9.0/zeus/optimizer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:51:24.036605 zeus_ml-0.9.0/zeus/optimizer/batch_size/
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-05-06 15:51:19.000000 zeus_ml-0.9.0/zeus/optimizer/batch_size/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7892 2024-05-06 15:51:19.000000 zeus_ml-0.9.0/zeus/optimizer/batch_size/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5712 2024-05-06 15:51:19.000000 zeus_ml-0.9.0/zeus/optimizer/batch_size/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)      691 2024-05-06 15:51:19.000000 zeus_ml-0.9.0/zeus/optimizer/batch_size/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:51:24.036605 zeus_ml-0.9.0/zeus/optimizer/batch_size/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     2756 2024-05-06 15:51:19.000000 zeus_ml-0.9.0/zeus/optimizer/batch_size/migrations/env.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:51:24.040604 zeus_ml-0.9.0/zeus/optimizer/batch_size/server/
+-rw-r--r--   0 runner    (1001) docker     (127)     2431 2024-05-06 15:51:19.000000 zeus_ml-0.9.0/zeus/optimizer/batch_size/server/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:51:24.040604 zeus_ml-0.9.0/zeus/optimizer/batch_size/server/batch_size_state/
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-06 15:51:19.000000 zeus_ml-0.9.0/zeus/optimizer/batch_size/server/batch_size_state/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4222 2024-05-06 15:51:19.000000 zeus_ml-0.9.0/zeus/optimizer/batch_size/server/batch_size_state/commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8675 2024-05-06 15:51:19.000000 zeus_ml-0.9.0/zeus/optimizer/batch_size/server/batch_size_state/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9950 2024-05-06 15:51:19.000000 zeus_ml-0.9.0/zeus/optimizer/batch_size/server/batch_size_state/repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-05-06 15:51:19.000000 zeus_ml-0.9.0/zeus/optimizer/batch_size/server/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:51:24.040604 zeus_ml-0.9.0/zeus/optimizer/batch_size/server/database/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-06 15:51:19.000000 zeus_ml-0.9.0/zeus/optimizer/batch_size/server/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2600 2024-05-06 15:51:19.000000 zeus_ml-0.9.0/zeus/optimizer/batch_size/server/database/db_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-06 15:51:19.000000 zeus_ml-0.9.0/zeus/optimizer/batch_size/server/database/repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6931 2024-05-06 15:51:19.000000 zeus_ml-0.9.0/zeus/optimizer/batch_size/server/database/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-05-06 15:51:19.000000 zeus_ml-0.9.0/zeus/optimizer/batch_size/server/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5497 2024-05-06 15:51:19.000000 zeus_ml-0.9.0/zeus/optimizer/batch_size/server/explorer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:51:24.040604 zeus_ml-0.9.0/zeus/optimizer/batch_size/server/job/
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-06 15:51:19.000000 zeus_ml-0.9.0/zeus/optimizer/batch_size/server/job/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5354 2024-05-06 15:51:19.000000 zeus_ml-0.9.0/zeus/optimizer/batch_size/server/job/commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2587 2024-05-06 15:51:19.000000 zeus_ml-0.9.0/zeus/optimizer/batch_size/server/job/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5887 2024-05-06 15:51:19.000000 zeus_ml-0.9.0/zeus/optimizer/batch_size/server/job/repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11140 2024-05-06 15:51:19.000000 zeus_ml-0.9.0/zeus/optimizer/batch_size/server/mab.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10989 2024-05-06 15:51:19.000000 zeus_ml-0.9.0/zeus/optimizer/batch_size/server/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7127 2024-05-06 15:51:19.000000 zeus_ml-0.9.0/zeus/optimizer/batch_size/server/router.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:51:24.040604 zeus_ml-0.9.0/zeus/optimizer/batch_size/server/services/
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-06 15:51:19.000000 zeus_ml-0.9.0/zeus/optimizer/batch_size/server/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      952 2024-05-06 15:51:19.000000 zeus_ml-0.9.0/zeus/optimizer/batch_size/server/services/commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14176 2024-05-06 15:51:19.000000 zeus_ml-0.9.0/zeus/optimizer/batch_size/server/services/service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:51:24.044604 zeus_ml-0.9.0/zeus/optimizer/pipeline_frequency/
+-rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-05-06 15:51:19.000000 zeus_ml-0.9.0/zeus/optimizer/pipeline_frequency/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11589 2024-05-06 15:51:19.000000 zeus_ml-0.9.0/zeus/optimizer/pipeline_frequency/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2959 2024-05-06 15:51:19.000000 zeus_ml-0.9.0/zeus/optimizer/pipeline_frequency/frequency_controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8591 2024-05-06 15:51:19.000000 zeus_ml-0.9.0/zeus/optimizer/pipeline_frequency/optimizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:51:24.044604 zeus_ml-0.9.0/zeus/optimizer/pipeline_frequency/server/
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-05-06 15:51:19.000000 zeus_ml-0.9.0/zeus/optimizer/pipeline_frequency/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9466 2024-05-06 15:51:19.000000 zeus_ml-0.9.0/zeus/optimizer/pipeline_frequency/server/job_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3815 2024-05-06 15:51:19.000000 zeus_ml-0.9.0/zeus/optimizer/pipeline_frequency/server/router.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12170 2024-05-06 15:51:19.000000 zeus_ml-0.9.0/zeus/optimizer/pipeline_frequency/server/scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22745 2024-05-06 15:51:19.000000 zeus_ml-0.9.0/zeus/optimizer/power_limit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:51:24.044604 zeus_ml-0.9.0/zeus/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-06 15:51:19.000000 zeus_ml-0.9.0/zeus/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2024 2024-05-06 15:51:19.000000 zeus_ml-0.9.0/zeus/utils/async_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-05-06 15:51:19.000000 zeus_ml-0.9.0/zeus/utils/env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1784 2024-05-06 15:51:19.000000 zeus_ml-0.9.0/zeus/utils/framework.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1878 2024-05-06 15:51:19.000000 zeus_ml-0.9.0/zeus/utils/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-05-06 15:51:19.000000 zeus_ml-0.9.0/zeus/utils/lr_scaler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4391 2024-05-06 15:51:19.000000 zeus_ml-0.9.0/zeus/utils/metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-05-06 15:51:19.000000 zeus_ml-0.9.0/zeus/utils/pydantic_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6845 2024-05-06 15:51:19.000000 zeus_ml-0.9.0/zeus/utils/testing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:51:24.044604 zeus_ml-0.9.0/zeus_ml.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7584 2024-05-06 15:51:24.000000 zeus_ml-0.9.0/zeus_ml.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3547 2024-05-06 15:51:24.000000 zeus_ml-0.9.0/zeus_ml.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 15:51:24.000000 zeus_ml-0.9.0/zeus_ml.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      748 2024-05-06 15:51:24.000000 zeus_ml-0.9.0/zeus_ml.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-06 15:51:24.000000 zeus_ml-0.9.0/zeus_ml.egg-info/top_level.txt
```

### Comparing `zeus-ml-0.8.2/LICENSE` & `zeus_ml-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `zeus-ml-0.8.2/capriccio/generate.py` & `zeus_ml-0.9.0/capriccio/generate.py`

 * *Files identical despite different names*

### Comparing `zeus-ml-0.8.2/docs/gen_ref_pages.py` & `zeus_ml-0.9.0/docs/gen_ref_pages.py`

 * *Files 14% similar despite different names*

```diff
@@ -22,16 +22,20 @@
 
 
 nav = mkdocs_gen_files.Nav()
 
 for path in sorted(Path("zeus").rglob("*.py")):
     # Path to the generated markdown file.
     doc_path = path.relative_to("zeus").with_suffix(".md")
-    full_doc_path = REF_DIR / doc_path
 
+    # Skip BSO server migration-related files.
+    if str(doc_path).find("batch_size/migrations") != -1:
+        continue
+
+    full_doc_path = REF_DIR / doc_path
     module_path = path.with_suffix("")
     parts = tuple(module_path.parts)
 
     # zeus/run/__init__ can just be zeus/run.
     if parts[-1] == "__init__":
         parts = parts[:-1]
         doc_path = doc_path.with_name("index.md")
```

### Comparing `zeus-ml-0.8.2/examples/ZeusDataLoader/capriccio/run_zeus.py` & `zeus_ml-0.9.0/examples/batch_size_optimizer/mnist/train_single_gpu.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,184 +1,263 @@
-# Copyright (C) 2023 Jae-Won Chung <jwnchung@umich.edu>
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
+"""
+Based on https://github.com/kubeflow/pytorch-operator/blob/master/examples/mnist/mnist.py
+"""
 
-"""Example script for running Zeus on the Capriccio dataset."""
+from __future__ import print_function
 
 import argparse
-import sys
-from pathlib import Path
+import os
 
-from zeus.job import Job
-from zeus.policy import PruningGTSBatchSizeOptimizer
-from zeus.run import ZeusMaster
-from zeus.util import FileAndConsole
-
-
-def parse_args() -> argparse.Namespace:
-    """Parse commandline arguments."""
-    parser = argparse.ArgumentParser()
-
-    # This random seed is used for
-    # 1. Multi-Armed Bandit inside PruningGTSBatchSizeOptimizer, and
-    # 2. Providing random seeds for training.
-    # Especially for 2, the random seed given to the nth recurrence job is args.seed + n.
-    parser.add_argument("--seed", type=int, default=123, help="Random seed")
-
-    # Default batch size and learning rate.
-    # The first recurrence uses these parameters, and it must reach the target metric.
-    # In subsequent recurrences, when the batch size changes, the new learning rate is determined
-    # using an adequate learning rate scaling rule. Since this job uses AdamW (see constructor of
-    # `Job`), Square Root Scaling will be used.
-    parser.add_argument("--b_0", type=int, default=128, help="Default batch size")
+from tensorboardX import SummaryWriter
+from torchvision import datasets, transforms
+import torch
+import torch.distributed as dist
+import torch.nn as nn
+import torch.nn.functional as F
+import torch.optim as optim
+from zeus.monitor import ZeusMonitor
+from zeus.optimizer.power_limit import GlobalPowerLimitOptimizer
+from zeus.optimizer.batch_size import BatchSizeOptimizer, JobSpec
+from zeus.utils.lr_scaler import LinearScaler
+
+
+WORLD_SIZE = int(os.environ.get("WORLD_SIZE", 1))
+
+class Net(nn.Module):
+    def __init__(self):
+        super(Net, self).__init__()
+        self.conv1 = nn.Conv2d(1, 20, 5, 1)
+        self.conv2 = nn.Conv2d(20, 50, 5, 1)
+        self.fc1 = nn.Linear(4 * 4 * 50, 500)
+        self.fc2 = nn.Linear(500, 10)
+
+    def forward(self, x):
+        x = F.relu(self.conv1(x))
+        x = F.max_pool2d(x, 2, 2)
+        x = F.relu(self.conv2(x))
+        x = F.max_pool2d(x, 2, 2)
+        x = x.view(-1, 4 * 4 * 50)
+        x = F.relu(self.fc1(x))
+        x = self.fc2(x)
+        return F.log_softmax(x, dim=1)
+
+
+def train(args, model, device, train_loader, optimizer, epoch, writer, plo):
+    model.train()
+    for batch_idx, (data, target) in enumerate(train_loader):
+        plo.on_step_begin()
+
+        data, target = data.to(device), target.to(device)
+        optimizer.zero_grad()
+        output = model(data)
+        loss = F.nll_loss(output, target)
+        loss.backward()
+        optimizer.step()
+
+        if batch_idx % args.log_interval == 0:
+            print(
+                "Train Epoch: {} [{}/{} ({:.0f}%)]\tloss={:.4f}".format(
+                    epoch,
+                    batch_idx * len(data),
+                    len(train_loader.dataset),
+                    100.0 * batch_idx / len(train_loader),
+                    loss.item(),
+                )
+            )
+            niter = epoch * len(train_loader) + batch_idx
+            writer.add_scalar("loss", loss.item(), niter)
+        plo.on_step_end()
+
+
+def test(args, model, device, test_loader, writer, epoch):
+    model.eval()
+    test_loss = 0
+    correct = 0
+    with torch.no_grad():
+        for data, target in test_loader:
+            data, target = data.to(device), target.to(device)
+            output = model(data)
+            test_loss += F.nll_loss(
+                output, target, reduction="sum"
+            ).item()  # sum up batch loss
+            pred = output.max(1, keepdim=True)[
+                1
+            ]  # get the index of the max log-probability
+            correct += pred.eq(target.view_as(pred)).sum().item()
+
+    test_loss /= len(test_loader.dataset)
+    print("\naccuracy={:.4f}\n".format(float(correct) / len(test_loader.dataset)))
+    writer.add_scalar("accuracy", float(correct) / len(test_loader.dataset), epoch)
+
+    return float(correct) / len(test_loader.dataset)
+
+
+def should_distribute():
+    return dist.is_available() and WORLD_SIZE > 1
+
+
+def is_distributed():
+    return dist.is_available() and dist.is_initialized()
+
+
+def main():
+    # Training settings
+    parser = argparse.ArgumentParser(description="PyTorch MNIST Example")
     parser.add_argument(
-        "--lr_0", type=float, default=4.00e-7, help="Default learning rate"
+        "--test-batch-size",
+        type=int,
+        default=1000,
+        metavar="N",
+        help="input batch size for testing (default: 1000)",
     )
-
-    # The range of batch sizes to consider. The example script generates a list of power-of-two
-    # batch sizes, but batch sizes need not be power-of-two for Zeus.
     parser.add_argument(
-        "--b_min", type=int, default=8, help="Smallest batch size to consider"
+        "--epochs",
+        type=int,
+        default=1,
+        metavar="N",
+        help="number of epochs to train (default: 10)",
     )
     parser.add_argument(
-        "--b_max", type=int, default=128, help="Largest batch size to consider"
+        "--momentum",
+        type=float,
+        default=0.5,
+        metavar="M",
+        help="SGD momentum (default: 0.5)",
     )
-
-    # The total number of recurrences. Capriccio has 38 time-overlapping slices.
     parser.add_argument(
-        "--num_recurrence", type=int, default=38, help="Total number of recurrences"
+        "--no-cuda", action="store_true", default=False, help="disables CUDA training"
     )
-
-    # The \\eta knob trades off time and energy consumption. See Equation 2 in the paper.
-    # The \\beta knob defines the early stopping threshold. See Section 4.4 in the paper.
     parser.add_argument(
-        "--eta_knob", type=float, default=0.5, help="TTA-ETA tradeoff knob"
+        "--seed", type=int, default=1, metavar="S", help="random seed (default: 1)"
     )
     parser.add_argument(
-        "--beta_knob", type=float, default=2.0, help="Early stopping threshold"
+        "--log-interval",
+        type=int,
+        default=10,
+        metavar="N",
+        help="how many batches to wait before logging training status",
     )
-
-    # Jobs are terminated when one of the three happens:
-    # 1. The target validation metric is reached.
-    # 2. The number of epochs exceeds the maximum number of epochs set.
-    # 3. The cost of the next epoch is expected to exceed the early stopping threshold.
     parser.add_argument(
-        "--target_metric", type=float, default=0.84, help="Target validation metric"
+        "--save-model",
+        action="store_true",
+        default=False,
+        help="For Saving the current Model",
     )
     parser.add_argument(
-        "--max_epochs", type=int, default=10, help="Max number of epochs to train"
+        "--dir",
+        default="logs",
+        metavar="L",
+        help="directory where summary logs are stored",
     )
-
-    # Zeus employs windowing to adapt to data drift. This argument defines the size of the window.
     parser.add_argument(
-        "--window_size", type=int, default=10, help="Size of the MAB observation window"
-    )
-
-    return parser.parse_args()
-
-
-def main(args: argparse.Namespace) -> None:
-    """Run Zeus on Capriccio."""
-    # Zeus's batch size optimizer.
-    # First prunes unpromising batch sizes, and then runs Gaussian Thompson Sampling MAB.
-    bso = PruningGTSBatchSizeOptimizer(
-        window_size=args.window_size, seed=args.seed, verbose=True
-    )
-
-    # The top-level class for running Zeus.
-    # - The batch size optimizer is desinged as a pluggable policy.
-    # - Paths (log_base and monitor_path) assume our Docker image's directory structure.
-    master = ZeusMaster(
-        batch_size_optimizer=bso,
-        log_base="/workspace/zeus_logs",
-        seed=args.seed,
-        monitor_path="/workspace/zeus/zeus_monitor/zeus_monitor",
-        observer_mode=False,
-    )
-
-    # Definition of the Capriccio job.
-    # The `Job` class encloses all information needed to run training. The `command` parameter is
-    # a command template. Curly-braced parameters are recognized by Zeus and automatically filled.
-    job = Job(
-        dataset="capriccio",
-        network="bert_base_uncased",
-        optimizer="adamw",
-        target_metric=args.target_metric,
-        max_epochs=args.max_epochs,
-        default_bs=args.b_0,
-        default_lr=args.lr_0,
-        workdir="/workspace/zeus/examples/capriccio",
-        # fmt: off
-        command=[
-            "python",
-            "train.py",
-            "--zeus",
-            "--model_name_or_path", "bert-base-uncased",
-            "--data_dir", "../../capriccio/data/",
-            "--slice_number", "{slice_number}",  # This will be filled with the current recurrence number.
-            "--max_length", "128",
-            "--batch_size", "{batch_size}",
-            "--learning_rate", "{learning_rate}",
-            "--num_train_epochs", "{epochs}",
-            "--seed", "{seed}",
-        ],
-        # fmt: on
-    )
-
-    # Generate a list of batch sizes with only power-of-two values.
-    batch_sizes = [args.b_min]
-    while (bs := batch_sizes[-1] * 2) <= args.b_max:
-        batch_sizes.append(bs)
-
-    # Create a designated log directory inside `args.log_base` just for this run of Zeus.
-    # Six types of outputs are generated.
-    # 1. Power monitor ouptut (`bs{batch_size}+e{epoch_num}+gpu{device_id}.power.log`):
-    #      Raw output of the Zeus power monitor.
-    # 2. Profiling results (`bs{batch_size}.power.json`):
-    #      Train-time average power consumption and throughput for each power limit,
-    #      the optimal power limit determined from the result of profiling, and
-    #      eval-time average power consumption and throughput for the optimal power limit.
-    # 3. Training script output (`rec{recurrence_num}+try{trial_num}.train.log`):
-    #      The raw output of the training script. `trial_num` exists because the job
-    #      may be early stopped and re-run with another batch size.
-    # 4. Training result (`rec{recurrence_num}+try{trial_num}+bs{batch_size}.train.json`):
-    #      The total energy, time, and cost consumed, and the number of epochs trained
-    #      until the job terminated. Also, whether the job reached the target metric at the
-    #      time of termination. Early-stopped jobs will not have reached their target metric.
-    # 5. ZeusMaster output (`master.log`): Output from ZeusMaster, including MAB outputs.
-    # 6. Job history (`history.py`):
-    #      A python file holding a list of `HistoryEntry` objects. Intended use is:
-    #      `history = eval(open("history.py").read())` after importing `HistoryEntry`.
-    master_logdir = master.build_logdir(
-        job=job,
-        num_recurrence=args.num_recurrence,
-        eta_knob=args.eta_knob,
-        beta_knob=args.beta_knob,
-        exist_ok=False,  # Should err if this directory exists.
-    )
-
-    # Overwrite the stdout file descriptor with an instance of `FileAndConsole`, so that
-    # all calls to `print` will write to both the console and the master log file.
-    sys.stdout = FileAndConsole(Path(master_logdir) / "master.log")
-
-    # Run Zeus!
-    master.run(
-        job=job,
-        num_recurrence=args.num_recurrence,
-        batch_sizes=batch_sizes,
-        beta_knob=args.beta_knob,
-        eta_knob=args.eta_knob,
-    )
+        "--target-accuracy",
+        type=float,
+        default=0.5,
+        help="Target accuracy (default: 0.5)",
+    )
+    if dist.is_available():
+        parser.add_argument(
+            "--backend",
+            type=str,
+            help="Distributed backend",
+            choices=[dist.Backend.GLOO, dist.Backend.NCCL, dist.Backend.MPI],
+            default=dist.Backend.GLOO,
+        )
+    args = parser.parse_args()
+    use_cuda = not args.no_cuda and torch.cuda.is_available()
+    if use_cuda:
+        print("Using CUDA")
+
+    writer = SummaryWriter(args.dir)
+
+    torch.manual_seed(args.seed)
+
+    device = torch.device("cuda" if use_cuda else "cpu")
+
+    if should_distribute():
+        print("Using distributed PyTorch with {} backend".format(args.backend))
+        dist.init_process_group(backend=args.backend)
+
+    kwargs = {"num_workers": 1, "pin_memory": True} if use_cuda else {}
+
+    ########################## Zeus ##########################
+    monitor = ZeusMonitor(gpu_indices=[0])
+    plo = GlobalPowerLimitOptimizer(monitor)
+    bso = BatchSizeOptimizer(
+        monitor=monitor,
+        server_url=os.environ["ZEUS_SERVER_URL"],
+        job=JobSpec(
+            job_id=os.environ.get("ZEUS_JOB_ID", None),
+            job_id_prefix="mnist-dev",
+            default_batch_size=256,
+            batch_sizes=[32, 64, 256, 512, 1024, 4096, 2048],
+            max_epochs=args.epochs,
+            target_metric=args.target_accuracy,
+        ),
+    )
+    # Fetch the batch size from the BSO server.
+    batch_size = bso.get_batch_size()
+    print("Chosen batach_size:", batch_size)
+    # Scale the learning rate accordingly.
+    # Default was batch size 64 and learing rate 0.01, and we use the linear
+    # scaling rule since the optimizer is SGD.
+    args.lr = LinearScaler(bs=64, lr=0.01).compute_lr(new_bs=batch_size)
+    ##########################################################
+
+    train_loader = torch.utils.data.DataLoader(
+        datasets.FashionMNIST(
+            "../data",
+            train=True,
+            download=True,
+            transform=transforms.Compose(
+                [transforms.ToTensor(), transforms.Normalize((0.1307,), (0.3081,))]
+            ),
+        ),
+        batch_size=batch_size,
+        shuffle=True,
+        **kwargs,
+    )
+    test_loader = torch.utils.data.DataLoader(
+        datasets.FashionMNIST(
+            "../data",
+            train=False,
+            transform=transforms.Compose(
+                [transforms.ToTensor(), transforms.Normalize((0.1307,), (0.3081,))]
+            ),
+        ),
+        batch_size=args.test_batch_size,
+        shuffle=False,
+        **kwargs,
+    )
+
+    model = Net().to(device)
+
+    if is_distributed():
+        Distributor = (
+            nn.parallel.DistributedDataParallel
+            if use_cuda
+            else nn.parallel.DistributedDataParallelCPU
+        )
+        model = Distributor(model)
+
+    optimizer = optim.SGD(model.parameters(), lr=args.lr, momentum=args.momentum)
+    
+    ########################## Zeus ##########################
+    bso.on_train_begin()
+
+    for epoch in range(1, args.epochs + 1):
+        plo.on_epoch_begin()
+        train(args, model, device, train_loader, optimizer, epoch, writer, plo)
+        plo.on_epoch_end()
+        acc = test(args, model, device, test_loader, writer, epoch)
+        bso.on_evaluate(acc)
+
+        if bso.training_finished:
+            break
+    ##########################################################
+        
+    if args.save_model:
+        torch.save(model.state_dict(), "mnist_cnn.pt")
 
 
 if __name__ == "__main__":
-    main(parse_args())
+    main()
```

### Comparing `zeus-ml-0.8.2/examples/ZeusDataLoader/capriccio/train.py` & `zeus_ml-0.9.0/examples/batch_size_optimizer/capriccio/train.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Finetuning a 🤗 Transformers model for sentiment analysis on Capriccio."""
 
+import os
 import argparse
 import logging
 import random
 from pathlib import Path
 
 import datasets
 import torch
@@ -32,58 +33,51 @@
     AutoModelForSequenceClassification,
     AutoTokenizer,
     DataCollatorWithPadding,
     default_data_collator,
     set_seed,
 )
 
-# ZEUS
-from zeus.run import ZeusDataLoader
+from zeus.monitor import ZeusMonitor
+from zeus.optimizer.power_limit import GlobalPowerLimitOptimizer
+from zeus.optimizer.batch_size import BatchSizeOptimizer, JobSpec
+from zeus.utils.lr_scaler import SquareRootScaler
 
 logger = logging.getLogger(__name__)
 
 
 def parse_args() -> argparse.Namespace:
     """Parse command line arguments."""
     parser = argparse.ArgumentParser(
         description="Finetune a transformers model on a text classification task"
     )
 
-    # CAPRICCIO
+    ########################## Zeus ##########################
     parser.add_argument(
         "--data_dir",
         type=str,
-        help="Directory where Capriccio is stored.",
+        help="Directory where the Capriccio dataset is stored.",
         required=True,
     )
     parser.add_argument(
         "--slice_number",
         type=int,
         help=(
-            "Which dataset slice to use."
+            "Which Capriccio dataset slice to use. "
             "Together with --data_dir, the paths to the train and val files are determined."
         ),
         required=True,
     )
-
-    # ZEUS
-    runtime_mode = parser.add_mutually_exclusive_group()
-    runtime_mode.add_argument(
-        "--zeus", action="store_true", help="Whether to run Zeus."
-    )
-
     parser.add_argument(
         "--target_metric",
-        default=None,
+        default=0.84,
         type=float,
-        help=(
-            "Stop training when the target metric is reached. This is ignored when running in Zeus mode because"
-            " ZeusDataLoader will receive the target metric via environment variable and stop training by itself."
-        ),
+        help="Stop training when the target metric is reached.",
     )
+    ##########################################################
 
     parser.add_argument(
         "--max_length",
         type=int,
         default=128,
         help=(
             "The maximum total input sequence length after tokenization. Sequences longer than this will be truncated,"
@@ -103,48 +97,45 @@
     )
     parser.add_argument(
         "--use_slow_tokenizer",
         action="store_true",
         help="If passed, will use a slow tokenizer (not backed by the 🤗 Tokenizers library).",
     )
     parser.add_argument(
-        "--batch_size",
-        type=int,
-        help="Batch size  for the training and eval dataloader.",
-        required=True,
-    )
-    parser.add_argument(
         "--learning_rate",
         type=float,
-        default=5e-5,
+        default=4.00e-7,
         help="Initial learning rate (after the potential warmup period) to use.",
     )
     parser.add_argument(
         "--weight_decay", type=float, default=0.0, help="Weight decay to use."
     )
     parser.add_argument(
-        "--num_train_epochs",
+        "--max_epochs",
         type=int,
-        default=3,
-        help="Total number of training epochs to perform.",
+        default=10,
+        help="Maximum number of training epochs to perform.",
     )
     parser.add_argument(
-        "--seed", type=int, default=None, help="A seed for reproducible training."
+        "--seed", type=int, default=123, help="A seed for reproducible training."
     )
     args = parser.parse_args()
 
-    # CAPRICCIO
-    if not (
-        train_file := Path(args.data_dir) / f"{args.slice_number}_train.json"
-    ).exists():
+    ########################## Zeus ##########################
+    # Determine the paths to the Capriccio train and val files.
+    train_file = Path(args.data_dir) / f"{args.slice_number}_train.json"
+    if not train_file.exists():
         raise ValueError(f"'{train_file}' does not exist")
     args.train_file = str(train_file)
-    if not (val_file := Path(args.data_dir) / f"{args.slice_number}_val.json").exists():
+
+    val_file = Path(args.data_dir) / f"{args.slice_number}_val.json"
+    if not val_file.exists():
         raise ValueError(f"'{val_file}' does not exist")
     args.val_file = str(val_file)
+    ##########################################################
 
     return args
 
 
 def main() -> None:
     """Run the main training routine."""
     args = parse_args()
@@ -161,16 +152,40 @@
     datasets.utils.logging.set_verbosity_warning()
     transformers.utils.logging.set_verbosity_info()
 
     # If passed along, set the training seed now.
     if args.seed is not None:
         set_seed(args.seed)
 
-    # Load the dataset.
-    # CAPRICCIO
+    ########################## Zeus ##########################
+    monitor = ZeusMonitor(gpu_indices=[0])  # Assumes single-GPU training.
+    plo = GlobalPowerLimitOptimizer(monitor)
+    bso = BatchSizeOptimizer(
+        monitor=monitor,
+        server_url=os.environ["ZEUS_SERVER_URL"],
+        job=JobSpec(
+            job_id=os.environ.get("ZEUS_JOB_ID"),
+            job_id_prefix="capriccio",
+            default_batch_size=128,
+            batch_sizes=[8, 16, 32, 64, 128],
+            max_epochs=args.max_epochs,
+            target_metric=args.target_metric,
+            window_size=10,
+        ),
+    )
+    # Fetch the batch size from the BSO server.
+    batch_size = bso.get_batch_size()
+    print("Chosen batach size:", batch_size)
+    # Scale the learning rate accordingly.
+    # Default was batch size 128 and learing rate 4.00e-7, and we use the square root
+    # scaling rule since the optimizer is AdamW.
+    args.learning_rate = SquareRootScaler(bs=128, lr=4.00e-7).compute_lr(new_bs=batch_size)
+    ##########################################################
+
+    # Load the specific slice of the Capriccio dataset.
     data_path = dict(train=args.train_file, validation=args.val_file)
     logger.info("Using dataset slice: %s", data_path)
     raw_datasets = load_dataset("json", data_files=data_path)
 
     label_list = raw_datasets["train"].unique("label")
     label_list.sort()
     num_labels = len(label_list)
@@ -187,15 +202,14 @@
     )
     model = AutoModelForSequenceClassification.from_pretrained(
         args.model_name_or_path,
         from_tf=bool(".ckpt" in args.model_name_or_path),
         config=config,
     )
 
-    # CAPRICCIO
     sentence1_key = "text"
     sentence2_key = None
 
     label_to_id = {v: i for i, v in enumerate(label_list)}
     model.config.label2id = label_to_id
     model.config.id2label = {id: label for label, id in config.label2id.items()}
 
@@ -224,15 +238,14 @@
     processed_datasets = raw_datasets.map(
         preprocess_function,
         batched=True,
         remove_columns=raw_datasets["train"].column_names,
         desc="Running tokenizer on dataset",
     )
 
-    # CAPRICCIO
     train_dataset = processed_datasets["train"]
     eval_dataset = processed_datasets["validation"]
 
     # Log a few random samples from the training set:
     for index in random.sample(range(len(train_dataset)), 3):
         logger.info("Sample %s of the training set: %s.", index, train_dataset[index])
 
@@ -243,36 +256,23 @@
         data_collator = default_data_collator
     else:
         # Otherwise, `DataCollatorWithPadding` will apply dynamic padding for us (by padding to the maximum length of
         # the samples passed). When using mixed precision, we add `pad_to_multiple_of=8` to pad all tensors to multiple
         # of 8s, which will enable the use of Tensor Cores on NVIDIA hardware with compute capability >= 7.5 (Volta).
         data_collator = DataCollatorWithPadding(tokenizer)
 
-    # ZEUS
-    if args.zeus:
-        train_dataloader = ZeusDataLoader(
-            train_dataset,
-            batch_size=args.batch_size,
-            max_epochs=args.num_train_epochs,
-            shuffle=True,
-            collate_fn=data_collator,
-        )
-        eval_dataloader = ZeusDataLoader(
-            eval_dataset, batch_size=args.batch_size, collate_fn=data_collator
-        )
-    else:
-        train_dataloader = DataLoader(
-            train_dataset,
-            shuffle=True,
-            collate_fn=data_collator,
-            batch_size=args.batch_size,
-        )
-        eval_dataloader = DataLoader(
-            eval_dataset, collate_fn=data_collator, batch_size=args.batch_size
-        )
+    train_dataloader = DataLoader(
+        train_dataset,
+        shuffle=True,
+        collate_fn=data_collator,
+        batch_size=batch_size,
+    )
+    eval_dataloader = DataLoader(
+        eval_dataset, collate_fn=data_collator, batch_size=batch_size
+    )
 
     # Optimizer
     # Split weights in two groups, one with weight decay and the other not.
     no_decay = ["bias", "LayerNorm.weight"]
     optimizer_grouped_parameters = [
         {
             "params": [
@@ -296,55 +296,59 @@
     # Send model to CUDA.
     model = model.cuda()
 
     # Note -> the training dataloader needs to be prepared before we grab his length below (cause its length will be
     # shorter in multiprocess)
 
     # Compute the total number of training steps.
-    args.max_train_steps = args.num_train_epochs * len(train_dataloader)
+    args.max_train_steps = args.max_epochs * len(train_dataloader)
 
     # Get the metric function
     metric = load_metric("accuracy")
 
     # Train!
     logger.info("***** Running training *****")
     logger.info("  Num examples = %s", len(train_dataset))
-    logger.info("  Num Epochs = %s", args.num_train_epochs)
+    logger.info("  Max Epochs = %s", args.max_epochs)
     logger.info(
         "  Total train batch size (w. parallel, distributed & accumulation) = %s",
-        args.batch_size,
+        batch_size,
     )
     logger.info("  Total optimization steps = %s", args.max_train_steps)
     if args.target_metric is not None:
         logger.info("  Target metric = %s", args.target_metric)
     # Only show the progress bar once on each machine.
     progress_bar = tqdm(range(args.max_train_steps))
     completed_steps = 0
 
-    # ZEUS
-    if args.zeus:
-        assert isinstance(train_dataloader, ZeusDataLoader)
-        epoch_iter = train_dataloader.epochs()
-    else:
-        epoch_iter = range(args.num_train_epochs)
+    ########################## Zeus ##########################
+    bso.on_train_begin()
+
+    for epoch in range(args.max_epochs):
+        plo.on_epoch_begin()
 
-    for epoch in epoch_iter:
         model.train()
         for batch in train_dataloader:
+            plo.on_step_begin()
+
             for key, val in batch.items():
                 if torch.is_tensor(val):
                     batch[key] = val.cuda()
             outputs = model(**batch)
             loss = outputs.loss
             loss.backward()
             optimizer.step()
             optimizer.zero_grad()
             progress_bar.update(1)
             completed_steps += 1
 
+            plo.on_step_end()
+
+        plo.on_epoch_end()
+
         model.eval()
         for batch in eval_dataloader:
             for key, val in batch.items():
                 if torch.is_tensor(val):
                     batch[key] = val.cuda()
             outputs = model(**batch)
             predictions = outputs.logits.argmax(dim=-1)
@@ -352,26 +356,15 @@
                 predictions=predictions,
                 references=batch["labels"],
             )
 
         eval_metric = metric.compute()
         logger.info("epoch %s: %s", epoch, eval_metric)
 
-        # ZEUS
-        if args.zeus:
-            assert isinstance(train_dataloader, ZeusDataLoader)
-            train_dataloader.report_metric(
-                eval_metric["accuracy"], higher_is_better=True
-            )
-        # If this were Zeus, the train dataloader will stop training by itself.
-        elif args.target_metric is not None:
-            if eval_metric["accuracy"] >= args.target_metric:
-                logger.info(
-                    "Reached target metric %s in %s epochs.",
-                    args.target_metric,
-                    epoch + 1,
-                )
-                break
+        bso.on_evaluate(eval_metric["accuracy"])
 
+        if bso.training_finished:
+            break
+        ##########################################################
 
 if __name__ == "__main__":
     main()
```

### Comparing `zeus-ml-0.8.2/examples/ZeusDataLoader/imagenet/train.py` & `zeus_ml-0.9.0/examples/huggingface/run_clm.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,819 +1,769 @@
+#!/usr/bin/env python
+# coding=utf-8
+# Copyright 2020 The HuggingFace Inc. team. All rights reserved.
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
 """
-This script trains an image classification model from `torchvision` on the ImageNet dataset.
-Currently it only supports single node training.
-    - Enable Zeus with `--zeus`.
-
-Launching methods of multi-GPU data parallel training:
-    - Using `torch.multiprocessing`
-        $ python train.py [DATA_DIR] --multiprocessing_distributed --zeus [OTHER_OPTIONS]
-    - Using `torch.distributed.launch` utility:
-        $ python -m torch.distributed.launch --nnodes=1 --nproc_per_node=[NUM_OF_GPUS] train.py [DATA_DIR] --zeus [OTHER_OPTIONS]
-    - Using `torchrun`:
-        $ torchrun --nnodes 1 --nproc_per_node [NUM_OF_GPUS] train.py [DATA_DIR] --zeus --torchrun [OTHER_OPTIONS]
-    - Using Slurm:
-        - Example script.sh:
-            ```sh
-            #!/bin/bash
-            #SBATCH --partition=gpu
-            #SBATCH --nodes=1                           # number of nodes (single node)
-            #SBATCH --ntasks-per-node=[NUM_OF_GPUS]     # number of tasks per node (1 task per GPU)
-            #SBATCH --gres=gpu:[NUM_OF_GPUS]            # number of GPUs reserved per node (here all the GPUs)
-            #SBATCH --mem=64GB
-            python train.py --zeus
-            ```
-        - On terminal:
-            $ sbatch script.sh
-
-Important notes:
-    1. Zeus will always use **ALL** the GPUs available to it. If you want to use specific GPUs on your node, please 
-       use our Docker image and replace the argument following `--gpus` in the `docker run` command with your preference. 
-       For example:
-        - Mount 2 GPUs to the Docker container: `--gpus 2`.
-        - Mount specific GPUs to the Docker container: `--gpus '"device=0,1"'`.
-       Please see the full instructions in README.md.
-    2. Please ensure that the global batch size passed in by `--batch_size` or `-b` is divisible by the number of
-       GPUs available. You can check the number of GPUs available by `torch.cuda.device_count()`.
-    3. Please do NOT set `cudnn.benchmark = True`. CuDNN's benchmarking will make the first few iterations very slow
-       and thus, ruin Zeus power profiling. This issue will be fixed soon in a later release of Zeus.
-    4. If `ZeusCostThresholdExceededException` is raised when running Zeus, it means the next predicted cost exceeds
-       the cost threshold, so the training stops. When doing data parallel, we utilize this customized exception to
-       terminate all the processes.
-
-Simplified example code:
-    It is critical to follow the correct steps when writing your own data parallel training script. Thus, we provide a
-    simplified version to specify each steps for a better comprehension.
-
-    ```python
-    import torch
-    import torchvision
-
-    from zeus.run import ZeusDataLoader
-
-    # Step 1: Initialize the default process group.
-    dist.init_process_group(
-        backend=args.dist_backend,
-        init_method=args.dist_url,
-    )
-
-    # Step 2: Create a model and wrap it with `DistributedDataParallel`.
-    model = torchvision.models.resnet18()
-    torch.cuda.set_device(local_rank)
-    model.cuda(local_rank)
-    # Zeus only supports one process per GPU profiling. If you are doing data
-    # parallel training, please use `DistributedDataParallel` for model replication
-    # and specify the `device_ids` and `output_device` correctly.
-    model = torch.nn.parallel.DistributedDataParallel(
-        model,
-        device_ids=[local_rank],
-        output_device=local_rank,
-    )
-
-    # Step 3: Create instances of `DistributedSampler` to partition the dataset
-	# across the GPUs.    
-    train_sampler = torch.utils.data.distributed.DistributedSampler(train_set)
-    eval_sampler = torch.utils.data.distributed.DistributedSampler(eval_set)
-
-    # Step 4: Create instances of `ZeusDataLoader`.
-    # Pass "dp" to `distributed` and samplers in the previous step to
-    # `sampler`.
-    # The one instantiated with `max_epochs` becomes the train dataloader.
-    train_loader = ZeusDataLoader(train_set, batch_size=256, max_epochs=100, 
-                                sampler=train_sampler, distributed="dp")
-    eval_loader = ZeusDataLoader(eval_set, batch_size=256, sampler=eval_sampler,
-                                distributed="dp")
-
-    # Step 5: Put your training code here.
-    for epoch_number in train_loader.epochs():
-        for batch in train_loader:
-            # Learn from batch
-        for batch in eval_loader:
-            # Evaluate on batch
-
-        # If doing data parallel training, please make sure to call 
-        # `torch.distributed.all_reduce()` to reduce the validation metric 
-        # across all GPUs before calling `train_loader.report_metric()`.
-        train_loader.report_metric(validation_metric)
-    ```
+Fine-tuning the library models for causal language modeling (GPT, GPT-2, CTRL, ...) on a text file or a dataset. Adapted from HuggingFace for Zeus.
+
+Here is the full list of checkpoints on the hub that can be fine-tuned by this script:
+https://huggingface.co/models?filter=text-generation
+
+Forked from https://github.com/huggingface/transformers/tree/f3aa7db439a2a3942f76c115197fe953984ac334/examples/pytorch/language-modeling
 """
+# You can also adapt this script on your own causal language modeling task. Pointers for this are left as comments.
 
-import argparse
+import logging
+import math
 import os
-import random
-import time
+import sys
 import warnings
-import subprocess
-from enum import Enum
+from dataclasses import dataclass, field
+from itertools import chain
+from typing import Optional
 
+import datasets
+import evaluate
 import torch
-import torch.nn as nn
-import torch.nn.parallel
-import torch.backends.cudnn as cudnn
-import torch.distributed as dist
-import torch.optim
-from torch.optim.lr_scheduler import StepLR
-import torch.multiprocessing as mp
-import torch.utils.data
-from torch.utils.data import DataLoader
-import torch.utils.data.distributed
-import torchvision.transforms as transforms
-import torchvision.datasets as datasets
-import torchvision.models as models
-from torch.utils.data import Subset
-
-# ZEUS
-from zeus.run import ZeusDataLoader
-
-
-def parse_args() -> argparse.Namespace:
-    """Parse command line arguments.
-
-    Raises:
-        ValueError: Launching methods arguments are mixed together. Please note that
-            `--multiprocessing-distributed` is dedicated to using `torch.multiprocessing.launch`
-            and `--torchrun` is dedicated to using `torchrun`. See more in the script docstring.
+from datasets import load_dataset
+import transformers
+from transformers import (
+    CONFIG_MAPPING,
+    MODEL_FOR_CAUSAL_LM_MAPPING,
+    AutoConfig,
+    AutoModelForCausalLM,
+    AutoTokenizer,
+    HfArgumentParser,
+    Trainer,
+    TrainingArguments,
+    default_data_collator,
+    is_torch_tpu_available,
+    set_seed,
+)
+from transformers.testing_utils import CaptureLogger
+from transformers.trainer_utils import get_last_checkpoint
+from transformers.utils import check_min_version, send_example_telemetry
+from transformers.utils.versions import require_version
+
+from zeus.monitor import ZeusMonitor
+from zeus.optimizer import HFGlobalPowerLimitOptimizer
+
+# Will error if the minimal version of Transformers is not installed. Remove at your own risks.
+check_min_version("4.37.2")
+
+require_version(
+    "datasets>=1.8.0",
+    "To fix: pip install -r examples/pytorch/language-modeling/requirements.txt",
+)
+
+logger = logging.getLogger(__name__)
+
+
+MODEL_CONFIG_CLASSES = list(MODEL_FOR_CAUSAL_LM_MAPPING.keys())
+MODEL_TYPES = tuple(conf.model_type for conf in MODEL_CONFIG_CLASSES)
+
+
+@dataclass
+class ModelArguments:
+    """
+    Arguments pertaining to which model/config/tokenizer we are going to fine-tune, or train from scratch.
     """
 
-    # List choices of models
-    model_names = sorted(
-        name
-        for name in models.__dict__
-        if name.islower()
-        and not name.startswith("__")
-        and callable(models.__dict__[name])
-    )
-
-    parser = argparse.ArgumentParser(description="PyTorch ImageNet Training")
-
-    parser.add_argument(
-        "data",
-        metavar="DIR",
-        help="Path to the ImageNet directory",
-    )
-    parser.add_argument(
-        "-a",
-        "--arch",
-        metavar="ARCH",
-        default="resnet18",
-        choices=model_names,
-        help="model architecture: " + " | ".join(model_names) + " (default: resnet18)",
-    )
-    parser.add_argument(
-        "-j",
-        "--workers",
-        default=4,
-        type=int,
-        metavar="N",
-        help="number of data loading workers (default: 4)",
-    )
-    parser.add_argument(
-        "--epochs",
-        default=90,
-        type=int,
-        metavar="N",
-        help="number of total epochs to run",
-    )
-    parser.add_argument(
-        "--start_epoch",
-        default=0,
-        type=int,
-        metavar="N",
-        help="manual epoch number (useful on restarts)",
-    )
-    parser.add_argument(
-        "-b",
-        "--batch_size",
-        default=256,
-        type=int,
-        metavar="N",
-        help="mini-batch size (default: 256), this is the total "
-        "batch size of all GPUs on the current node when "
-        "using Data Parallel or Distributed Data Parallel",
-    )
-    parser.add_argument(
-        "--lr",
-        "--learning_rate",
-        default=0.1,
-        type=float,
-        metavar="LR",
-        help="initial learning rate",
-        dest="lr",
-    )
-    parser.add_argument(
-        "--momentum", default=0.9, type=float, metavar="M", help="momentum"
-    )
-    parser.add_argument(
-        "--wd",
-        "--weight_decay",
-        default=1e-4,
-        type=float,
-        metavar="W",
-        help="weight decay (default: 1e-4)",
-        dest="weight_decay",
-    )
-    parser.add_argument(
-        "-p",
-        "--print_freq",
-        default=10,
-        type=int,
-        metavar="N",
-        help="print frequency (default: 10)",
-    )
-    parser.add_argument(
-        "-e",
-        "--evaluate",
-        dest="evaluate",
-        action="store_true",
-        help="evaluate model on validation set",
-    )
-    parser.add_argument(
-        "--pretrained",
-        dest="pretrained",
-        action="store_true",
-        help="use pre-trained model",
-    )
-    parser.add_argument(
-        "--dist_url",
-        default="tcp://127.0.0.1:12306",
-        type=str,
-        help="url used to set up distributed training",
-    )
-    parser.add_argument(
-        "--dist_backend", default="nccl", type=str, help="distributed backend"
-    )
-    parser.add_argument(
-        "--seed", default=None, type=int, help="seed for initializing training. "
-    )
-    parser.add_argument("--gpu", default=None, type=int, help="GPU id to use.")
-    parser.add_argument(
-        "--multiprocessing_distributed",
-        action="store_true",
-        help="Use `torch.multiprocessing` to launch N processes on this node, "
-        "which has N GPUs. PLEASE DO NOT use this argument if you are using "
-        "`torchrun` or ``torch.distributed.launch`.",
-    )
-    parser.add_argument(
-        "--dummy", action="store_true", help="use fake data to benchmark"
-    )
-
-    # ZEUS
-    parser.add_argument("--zeus", action="store_true", help="Whether to run Zeus.")
-    parser.add_argument(
-        "--target_metric",
-        default=None,
-        type=float,
-        help=(
-            "Stop training when the target metric is reached. This is ignored when running in Zeus mode because"
-            " ZeusDataLoader will receive the target metric via environment variable and stop training by itself."
-        ),
-    )
-
-    # DATA PARALLEL
-    parser.add_argument(
-        "--local_rank",
-        default=-1,
-        type=int,
-        help="Local rank for data parallel training. This is necessary for using the `torch.distributed.launch` utility.",
-    )
-    parser.add_argument(
-        "--local_world_size",
-        default=-1,
-        type=int,
-        help="Local world size for data parallel training.",
-    )
-    parser.add_argument(
-        "--torchrun",
-        action="store_true",
-        help="Use torchrun. This means we will read local_rank from environment variable set by `torchrun`.",
+    model_name_or_path: Optional[str] = field(
+        default=None,
+        metadata={
+            "help": (
+                "The model checkpoint for weights initialization. Don't set if you want to train a model from scratch."
+            )
+        },
+    )
+    model_type: Optional[str] = field(
+        default=None,
+        metadata={
+            "help": "If training from scratch, pass a model type from the list: "
+            + ", ".join(MODEL_TYPES)
+        },
+    )
+    config_overrides: Optional[str] = field(
+        default=None,
+        metadata={
+            "help": (
+                "Override some existing default config settings when a model is trained from scratch. Example: "
+                "n_embd=10,resid_pdrop=0.2,scale_attn_weights=false,summary_type=cls_index"
+            )
+        },
+    )
+    config_name: Optional[str] = field(
+        default=None,
+        metadata={
+            "help": "Pretrained config name or path if not the same as model_name"
+        },
+    )
+    tokenizer_name: Optional[str] = field(
+        default=None,
+        metadata={
+            "help": "Pretrained tokenizer name or path if not the same as model_name"
+        },
+    )
+    cache_dir: Optional[str] = field(
+        default=None,
+        metadata={
+            "help": "Where do you want to store the pretrained models downloaded from huggingface.co"
+        },
+    )
+    use_fast_tokenizer: bool = field(
+        default=True,
+        metadata={
+            "help": "Whether to use one of the fast tokenizer (backed by the tokenizers library) or not."
+        },
+    )
+    model_revision: str = field(
+        default="main",
+        metadata={
+            "help": "The specific model version to use (can be a branch name, tag name or commit id)."
+        },
+    )
+    token: str = field(
+        default=None,
+        metadata={
+            "help": (
+                "The token to use as HTTP bearer authorization for remote files. If not specified, will use the token "
+                "generated when running `huggingface-cli login` (stored in `~/.huggingface`)."
+            )
+        },
+    )
+    use_auth_token: bool = field(
+        default=None,
+        metadata={
+            "help": "The `use_auth_token` argument is deprecated and will be removed in v4.34. Please use `token` instead."
+        },
+    )
+    trust_remote_code: bool = field(
+        default=False,
+        metadata={
+            "help": (
+                "Whether or not to allow for custom models defined on the Hub in their own modeling files. This option "
+                "should only be set to `True` for repositories you trust and in which you have read the code, as it will "
+                "execute code present on the Hub on your local machine."
+            )
+        },
+    )
+    torch_dtype: Optional[str] = field(
+        default=None,
+        metadata={
+            "help": (
+                "Override the default `torch.dtype` and load the model under this dtype. If `auto` is passed, the "
+                "dtype will be automatically derived from the model's weights."
+            ),
+            "choices": ["auto", "bfloat16", "float16", "float32"],
+        },
+    )
+    low_cpu_mem_usage: bool = field(
+        default=False,
+        metadata={
+            "help": (
+                "It is an option to create the model as an empty shell, then only materialize its parameters when the pretrained weights are loaded. "
+                "set True will benefit LLM loading time and RAM consumption."
+            )
+        },
     )
 
-    args = parser.parse_args()
+    def __post_init__(self):
+        if self.config_overrides is not None and (
+            self.config_name is not None or self.model_name_or_path is not None
+        ):
+            raise ValueError(
+                "--config_overrides can't be used in combination with --config_name or --model_name_or_path"
+            )
 
-    # Sanity check
-    if args.multiprocessing_distributed and (args.torchrun or args.local_rank >= 0):
-        raise ValueError(
-            "Can not set --multiprocessing-distributed when using `torch.distributed.launch` or `torchrun`. "
-            "Please refer to the docstring for more info about launching methods."
-        )
 
-    return args
+@dataclass
+class DataTrainingArguments:
+    """
+    Arguments pertaining to what data we are going to input our model for training and eval.
+    """
 
+    dataset_name: Optional[str] = field(
+        default=None,
+        metadata={"help": "The name of the dataset to use (via the datasets library)."},
+    )
+    dataset_config_name: Optional[str] = field(
+        default=None,
+        metadata={
+            "help": "The configuration name of the dataset to use (via the datasets library)."
+        },
+    )
+    train_file: Optional[str] = field(
+        default=None, metadata={"help": "The input training data file (a text file)."}
+    )
+    validation_file: Optional[str] = field(
+        default=None,
+        metadata={
+            "help": "An optional input evaluation data file to evaluate the perplexity on (a text file)."
+        },
+    )
+    max_train_samples: Optional[int] = field(
+        default=None,
+        metadata={
+            "help": (
+                "For debugging purposes or quicker training, truncate the number of training examples to this "
+                "value if set."
+            )
+        },
+    )
+    max_eval_samples: Optional[int] = field(
+        default=None,
+        metadata={
+            "help": (
+                "For debugging purposes or quicker training, truncate the number of evaluation examples to this "
+                "value if set."
+            )
+        },
+    )
+    streaming: bool = field(default=False, metadata={"help": "Enable streaming mode"})
+    block_size: Optional[int] = field(
+        default=None,
+        metadata={
+            "help": (
+                "Optional input sequence length after tokenization. "
+                "The training dataset will be truncated in block of this size for training. "
+                "Default to the model max input length for single sentence inputs (take into account special tokens)."
+            )
+        },
+    )
+    overwrite_cache: bool = field(
+        default=False,
+        metadata={"help": "Overwrite the cached training and evaluation sets"},
+    )
+    validation_split_percentage: Optional[int] = field(
+        default=5,
+        metadata={
+            "help": "The percentage of the train set used as validation set in case there's no validation split"
+        },
+    )
+    preprocessing_num_workers: Optional[int] = field(
+        default=None,
+        metadata={"help": "The number of processes to use for the preprocessing."},
+    )
+    keep_linebreaks: bool = field(
+        default=True,
+        metadata={"help": "Whether to keep line breaks when using TXT files or not."},
+    )
 
-def main():
-    """Main function that prepares values and spawns/calls the worker function.
+    def __post_init__(self):
+        if self.streaming:
+            require_version(
+                "datasets>=2.0.0", "The streaming feature requires `datasets>=2.0.0`"
+            )
 
-    Raises:
-        ValueError: The global batch size passed in by `--batch_size` or `-b`
-            is not divisible by the number of GPUs.
-    """
-    args = parse_args()
+        if (
+            self.dataset_name is None
+            and self.train_file is None
+            and self.validation_file is None
+        ):
+            raise ValueError(
+                "Need either a dataset name or a training/validation file."
+            )
+        else:
+            if self.train_file is not None:
+                extension = self.train_file.split(".")[-1]
+                assert extension in [
+                    "csv",
+                    "json",
+                    "txt",
+                ], "`train_file` should be a csv, a json or a txt file."
+            if self.validation_file is not None:
+                extension = self.validation_file.split(".")[-1]
+                assert extension in [
+                    "csv",
+                    "json",
+                    "txt",
+                ], "`validation_file` should be a csv, a json or a txt file."
 
-    if args.seed is not None:
-        random.seed(args.seed)
-        torch.manual_seed(args.seed)
-        cudnn.deterministic = True
 
-    if args.gpu is not None:
-        warnings.warn(
-            "You have chosen a specific GPU. This will completely "
-            "disable data parallelism."
+def main():
+    # See all possible arguments in src/transformers/training_args.py
+    # or by passing the --help flag to this script.
+    # We now keep distinct sets of args, for a cleaner separation of concerns.
+
+    parser = HfArgumentParser(
+        (
+            ModelArguments,
+            DataTrainingArguments,
+            TrainingArguments,
+        )
+    )
+    if len(sys.argv) == 2 and sys.argv[1].endswith(".json"):
+        # If we pass only one argument to the script and it's the path to a json file,
+        # let's parse it to get our arguments.
+        model_args, data_args, training_args = parser.parse_json_file(
+            json_file=os.path.abspath(sys.argv[1])
         )
+    else:
+        (
+            model_args,
+            data_args,
+            training_args,
+        ) = parser.parse_args_into_dataclasses()
 
-    # DATA PARALLEL
-    # Preparation for SLURM
-    if "SLURM_PROCID" in os.environ:
-        # Retrieve local_rank.
-        # We only consider Single GPU for now. So `local_rank == rank`.
-        args.local_rank = int(os.environ["SLURM_PROCID"])
-
-        # Retrieve the node address
-        node_list = os.environ["SLURM_NODELIST"]
-        addr = subprocess.getoutput(f"scontrol show hostname {node_list} | head -n1")
-        # Specify master address and master port
-        if "MASTER_ADDR" not in os.environ:
-            os.environ["MASTER_ADDR"] = addr
-        if "MASTER_PORT" not in os.environ:
-            os.environ["MASTER_PORT"] = "29500"
-
-    # Preparation for torchrun.
-    # Integrate launching by `torchrun` and `torch.distributed.launch`
-    # by retrieving local rank from environment variable LOCAL_RANK.
-    if args.torchrun:
-        args.local_rank = int(os.environ["LOCAL_RANK"])
-        args.local_world_size = int(os.environ["LOCAL_WORLD_SIZE"])
-
-    args.distributed = args.multiprocessing_distributed or args.local_rank >= 0
-    ngpus_per_node = torch.cuda.device_count()
-
-    # The global batch size passed in by `--batch_size` or `-b` MUST be divisible
-    # by the number of GPUs available. You can check the number of GPUs available by
-    # `torch.cuda.device_count()`.
-    if args.batch_size % ngpus_per_node != 0:
-        raise ValueError(
-            "The global batch size passed in by `--batch_size` or `-b` MUST"
-            " be divisible by the number of GPUs available. Got"
-            f" global_batch_size={args.batch_size} with {ngpus_per_node} GPUs."
+    if model_args.use_auth_token is not None:
+        warnings.warn(
+            "The `use_auth_token` argument is deprecated and will be removed in v4.34. Please use `token` instead.",
+            FutureWarning,
         )
+        if model_args.token is not None:
+            raise ValueError(
+                "`token` and `use_auth_token` are both specified. Please set only the argument `token`."
+            )
+        model_args.token = model_args.use_auth_token
 
-    if args.multiprocessing_distributed:
-        # Use `torch.multiprocessing.spawn` to launch distributed processes: the
-        # main_worker process function.
-        mp.spawn(main_worker, nprocs=ngpus_per_node, args=(ngpus_per_node, args))
-    elif args.local_rank >= 0:
-        # Use `torch.distributed.launch` or `turchrun` or `slurm`.
-        # Simply call `main_worker` at `local_rank`.
-        main_worker(args.local_rank, ngpus_per_node, args)
-    else:
-        # Use a specific GPU.
-        # Simply call main_worker function.
-        main_worker(args.gpu, ngpus_per_node, args)
-
-
-def main_worker(gpu, ngpus_per_node, args):
-    """Worker function that runs on each process."""
-    args.gpu = gpu
-
-    if args.gpu is not None:
-        print(f"Use GPU {args.gpu} for training")
-
-    # DATA PARALLEL
-    # Step 1: Initialize the default process group.
-    if args.distributed:
-        if args.multiprocessing_distributed:
-            # Use `torch.multiprocessing`
-            # Spawn N processes, one for each GPU
-            dist.init_process_group(
-                backend=args.dist_backend,
-                init_method=args.dist_url,
-                world_size=ngpus_per_node,
-                rank=args.gpu,
+    # Sending telemetry. Tracking the example usage helps us better allocate resources to maintain them. The
+    # information sent is the one passed as arguments along with your Python/PyTorch versions.
+    send_example_telemetry("run_clm", model_args, data_args)
+
+    # Setup logging
+    logging.basicConfig(
+        format="%(asctime)s - %(levelname)s - %(name)s - %(message)s",
+        datefmt="%m/%d/%Y %H:%M:%S",
+        handlers=[logging.StreamHandler(sys.stdout)],
+    )
+
+    if training_args.should_log:
+        # The default of training_args.log_level is passive, so we set log level at info here to have that default.
+        transformers.utils.logging.set_verbosity_info()
+
+    log_level = training_args.get_process_log_level()
+    logger.setLevel(log_level)
+    datasets.utils.logging.set_verbosity(log_level)
+    transformers.utils.logging.set_verbosity(log_level)
+    transformers.utils.logging.enable_default_handler()
+    transformers.utils.logging.enable_explicit_format()
+
+    # Log on each process the small summary:
+    logger.warning(
+        f"Process rank: {training_args.local_rank}, device: {training_args.device}, n_gpu: {training_args.n_gpu}, "
+        + f"distributed training: {training_args.parallel_mode.value == 'distributed'}, 16-bits training: {training_args.fp16}"
+    )
+    logger.info(f"Training/evaluation parameters {training_args}")
+
+    # Detecting last checkpoint.
+    last_checkpoint = None
+    if (
+        os.path.isdir(training_args.output_dir)
+        and training_args.do_train
+        and not training_args.overwrite_output_dir
+    ):
+        last_checkpoint = get_last_checkpoint(training_args.output_dir)
+        if last_checkpoint is None and len(os.listdir(training_args.output_dir)) > 0:
+            raise ValueError(
+                f"Output directory ({training_args.output_dir}) already exists and is not empty. "
+                "Use --overwrite_output_dir to overcome."
+            )
+        elif (
+            last_checkpoint is not None and training_args.resume_from_checkpoint is None
+        ):
+            logger.info(
+                f"Checkpoint detected, resuming training at {last_checkpoint}. To avoid this behavior, change "
+                "the `--output_dir` or add `--overwrite_output_dir` to train from scratch."
             )
-        else:
-            # Use `torchrun`, `torch.distributed.launch` or SLURM
-            # `MASTER_ADDR` and `MASTER_PORT` are already set as environment variables,
-            # so no need to pass to `init_process_group``.
-            dist.init_process_group(backend=args.dist_backend)
 
-        if args.local_world_size < 0:
-            args.local_world_size = dist.get_world_size()
-    else:
-        args.local_world_size = 1
+    # Set seed before initializing model.
+    set_seed(training_args.seed)
 
-    # Step 2: Create a model and wrap it with `DistributedDataParallel`.
-    if args.pretrained:
-        print("=> using pre-trained model '{}'".format(args.arch))
-        model = models.__dict__[args.arch](pretrained=True)
-    else:
-        print("=> creating model '{}'".format(args.arch))
-        model = models.__dict__[args.arch]()
-    if not torch.cuda.is_available():
-        print("using CPU, this will be slow")
-    elif args.distributed:
-        # DATA PARALLEL
-        # For multiprocessing distributed, DistributedDataParallel constructor
-        # should always set the single device scope, otherwise,
-        # DistributedDataParallel will use all available devices.
-        if args.gpu is not None:
-            torch.cuda.set_device(args.gpu)
-            model.cuda(args.gpu)
-            # When using a single GPU per process and per
-            # DistributedDataParallel, we need to divide the batch size
-            # ourselves based on the total number of GPUs of the current node.
-            args.batch_size = int(args.batch_size / ngpus_per_node)
-            args.workers = int((args.workers + ngpus_per_node - 1) / ngpus_per_node)
-            model = torch.nn.parallel.DistributedDataParallel(
-                model,
-                device_ids=[args.gpu],
-                output_device=args.gpu,
+    # Get the datasets: you can either provide your own CSV/JSON/TXT training and evaluation files (see below)
+    # or just provide the name of one of the public datasets available on the hub at https://huggingface.co/datasets/
+    # (the dataset will be downloaded automatically from the datasets Hub).
+    #
+    # For CSV/JSON files, this script will use the column called 'text' or the first column if no column called
+    # 'text' is found. You can easily tweak this behavior (see below).
+    #
+    # In distributed training, the load_dataset function guarantee that only one local process can concurrently
+    # download the dataset.
+    if data_args.dataset_name is not None:
+        # Downloading and loading a dataset from the hub.
+        raw_datasets = load_dataset(
+            data_args.dataset_name,
+            data_args.dataset_config_name,
+            cache_dir=model_args.cache_dir,
+            token=model_args.token,
+            streaming=data_args.streaming,
+        )
+        if "validation" not in raw_datasets.keys():
+            raw_datasets["validation"] = load_dataset(
+                data_args.dataset_name,
+                data_args.dataset_config_name,
+                split=f"train[:{data_args.validation_split_percentage}%]",
+                cache_dir=model_args.cache_dir,
+                token=model_args.token,
+                streaming=data_args.streaming,
+            )
+            raw_datasets["train"] = load_dataset(
+                data_args.dataset_name,
+                data_args.dataset_config_name,
+                split=f"train[{data_args.validation_split_percentage}%:]",
+                cache_dir=model_args.cache_dir,
+                token=model_args.token,
+                streaming=data_args.streaming,
             )
-        else:
-            model.cuda()
-            # DistributedDataParallel will divide and allocate batch_size to all
-            # available GPUs if device_ids are not set
-            model = torch.nn.parallel.DistributedDataParallel(model)
-    elif args.gpu is not None:
-        torch.cuda.set_device(args.gpu)
-        model = model.cuda(args.gpu)
     else:
-        # DataParallel will divide and allocate batch_size to all available GPUs
-        if args.arch.startswith("alexnet") or args.arch.startswith("vgg"):
-            model.features = torch.nn.DataParallel(model.features)
-            model.cuda()
-        else:
-            model = torch.nn.DataParallel(model).cuda()
-
-    # define loss function (criterion), optimizer, and learning rate scheduler
-    criterion = nn.CrossEntropyLoss().cuda(args.gpu)
-
-    optimizer = torch.optim.SGD(
-        model.parameters(),
-        args.lr,
-        momentum=args.momentum,
-        weight_decay=args.weight_decay,
-    )
+        data_files = {}
+        dataset_args = {}
+        if data_args.train_file is not None:
+            data_files["train"] = data_args.train_file
+        if data_args.validation_file is not None:
+            data_files["validation"] = data_args.validation_file
+        extension = (
+            data_args.train_file.split(".")[-1]
+            if data_args.train_file is not None
+            else data_args.validation_file.split(".")[-1]
+        )
+        if extension == "txt":
+            extension = "text"
+            dataset_args["keep_linebreaks"] = data_args.keep_linebreaks
+        raw_datasets = load_dataset(
+            extension,
+            data_files=data_files,
+            cache_dir=model_args.cache_dir,
+            token=model_args.token,
+            **dataset_args,
+        )
+        # If no validation data is there, validation_split_percentage will be used to divide the dataset.
+        if "validation" not in raw_datasets.keys():
+            raw_datasets["validation"] = load_dataset(
+                extension,
+                data_files=data_files,
+                split=f"train[:{data_args.validation_split_percentage}%]",
+                cache_dir=model_args.cache_dir,
+                token=model_args.token,
+                **dataset_args,
+            )
+            raw_datasets["train"] = load_dataset(
+                extension,
+                data_files=data_files,
+                split=f"train[{data_args.validation_split_percentage}%:]",
+                cache_dir=model_args.cache_dir,
+                token=model_args.token,
+                **dataset_args,
+            )
 
-    """Sets the learning rate to the initial LR decayed by 10 every 30 epochs"""
-    scheduler = StepLR(optimizer, step_size=30, gamma=0.1)
+    # See more about loading any type of standard or custom dataset (from files, python dict, pandas DataFrame, etc) at
+    # https://huggingface.co/docs/datasets/loading_datasets.
 
-    # Data loading code
-    if args.dummy:
-        print("=> Dummy data is used!")
-        train_dataset = datasets.FakeData(
-            1281167, (3, 224, 224), 1000, transforms.ToTensor()
-        )
-        val_dataset = datasets.FakeData(
-            50000, (3, 224, 224), 1000, transforms.ToTensor()
+    # Load pretrained model and tokenizer
+    #
+    # Distributed training:
+    # The .from_pretrained methods guarantee that only one local process can concurrently
+    # download model & vocab.
+
+    config_kwargs = {
+        "cache_dir": model_args.cache_dir,
+        "revision": model_args.model_revision,
+        "token": model_args.token,
+        "trust_remote_code": model_args.trust_remote_code,
+    }
+    if model_args.config_name:
+        config = AutoConfig.from_pretrained(model_args.config_name, **config_kwargs)
+    elif model_args.model_name_or_path:
+        config = AutoConfig.from_pretrained(
+            model_args.model_name_or_path, **config_kwargs
         )
     else:
-        traindir = os.path.join(args.data, "train")
-        valdir = os.path.join(args.data, "val")
-        normalize = transforms.Normalize(
-            mean=[0.485, 0.456, 0.406], std=[0.229, 0.224, 0.225]
+        config = CONFIG_MAPPING[model_args.model_type]()
+        logger.warning("You are instantiating a new config instance from scratch.")
+        if model_args.config_overrides is not None:
+            logger.info(f"Overriding config: {model_args.config_overrides}")
+            config.update_from_string(model_args.config_overrides)
+            logger.info(f"New config: {config}")
+
+    tokenizer_kwargs = {
+        "cache_dir": model_args.cache_dir,
+        "use_fast": model_args.use_fast_tokenizer,
+        "revision": model_args.model_revision,
+        "token": model_args.token,
+        "trust_remote_code": model_args.trust_remote_code,
+    }
+    if model_args.tokenizer_name:
+        tokenizer = AutoTokenizer.from_pretrained(
+            model_args.tokenizer_name, **tokenizer_kwargs
+        )
+    elif model_args.model_name_or_path:
+        tokenizer = AutoTokenizer.from_pretrained(
+            model_args.model_name_or_path, **tokenizer_kwargs
         )
-
-        train_dataset = datasets.ImageFolder(
-            traindir,
-            transforms.Compose(
-                [
-                    transforms.RandomResizedCrop(224),
-                    transforms.RandomHorizontalFlip(),
-                    transforms.ToTensor(),
-                    normalize,
-                ]
-            ),
+    else:
+        raise ValueError(
+            "You are instantiating a new tokenizer from scratch. This is not supported by this script. "
+            "You can do it from another script, save it, and load it from here, using --tokenizer_name."
         )
 
-        val_dataset = datasets.ImageFolder(
-            valdir,
-            transforms.Compose(
-                [
-                    transforms.Resize(256),
-                    transforms.CenterCrop(224),
-                    transforms.ToTensor(),
-                    normalize,
-                ]
-            ),
+    if model_args.model_name_or_path:
+        torch_dtype = (
+            model_args.torch_dtype
+            if model_args.torch_dtype in ["auto", None]
+            else getattr(torch, model_args.torch_dtype)
+        )
+        model = AutoModelForCausalLM.from_pretrained(
+            model_args.model_name_or_path,
+            from_tf=bool(".ckpt" in model_args.model_name_or_path),
+            config=config,
+            cache_dir=model_args.cache_dir,
+            revision=model_args.model_revision,
+            token=model_args.token,
+            trust_remote_code=model_args.trust_remote_code,
+            torch_dtype=torch_dtype,
+            low_cpu_mem_usage=model_args.low_cpu_mem_usage,
         )
-
-    # DATA PARALLEL
-    # Step 3: Create instances of `DistributedSampler` to restrict data loading
-    # to a subset of the dataset.
-    if args.distributed:
-        train_sampler = torch.utils.data.distributed.DistributedSampler(train_dataset)
-        val_sampler = torch.utils.data.distributed.DistributedSampler(
-            val_dataset, shuffle=False, drop_last=True
+    else:
+        model = AutoModelForCausalLM.from_config(
+            config, trust_remote_code=model_args.trust_remote_code
         )
+        n_params = sum({p.data_ptr(): p.numel() for p in model.parameters()}.values())
+        logger.info(
+            f"Training new model from scratch - Total size={n_params/2**20:.2f}M params"
+        )
+
+    # We resize the embeddings only when necessary to avoid index errors. If you are creating a model from scratch
+    # on a small vocab and want a smaller embedding size, remove this test.
+    embedding_size = model.get_input_embeddings().weight.shape[0]
+    if len(tokenizer) > embedding_size:
+        model.resize_token_embeddings(len(tokenizer))
+
+    # Preprocessing the datasets.
+    # First we tokenize all the texts.
+    if training_args.do_train:
+        column_names = list(raw_datasets["train"].features)
     else:
-        train_sampler = None
-        val_sampler = None
+        column_names = list(raw_datasets["validation"].features)
+    text_column_name = "text" if "text" in column_names else column_names[0]
 
-    # ZEUS
-    # Step 4: Create instances of `ZeusDataLoader`.
-    if args.zeus:
-        # ZEUS
-        # Take either of the launching approaches of the data parallel training on
-        # single-node multi-GPU will activate the data parallel ("dp") mode in zeus.
-
-        # DATA PARALLEL
-        zeus_distributed = "dp" if args.distributed else None
-
-        train_loader = ZeusDataLoader(
-            train_dataset,
-            batch_size=args.batch_size,
-            distributed=zeus_distributed,
-            max_epochs=args.epochs,
-            shuffle=(train_sampler is None),
-            num_workers=args.workers,
-            pin_memory=True,
-            sampler=train_sampler,
-        )
-        val_loader = ZeusDataLoader(
-            val_dataset,
-            batch_size=args.batch_size,
-            distributed=zeus_distributed,
-            shuffle=False,
-            num_workers=args.workers,
-            pin_memory=True,
-            sampler=val_sampler,
-        )
+    # since this will be pickled to avoid _LazyModule error in Hasher force logger loading before tokenize_function
+    tok_logger = transformers.utils.logging.get_logger(
+        "transformers.tokenization_utils_base"
+    )
+
+    def tokenize_function(examples):
+        with CaptureLogger(tok_logger) as cl:
+            output = tokenizer(examples[text_column_name])
+        # clm input could be much much longer than block_size
+        if "Token indices sequence length is longer than the" in cl.out:
+            tok_logger.warning(
+                "^^^^^^^^^^^^^^^^ Please ignore the warning above - this long input will be chunked into smaller bits"
+                " before being passed to the model."
+            )
+        return output
+
+    with training_args.main_process_first(desc="dataset map tokenization"):
+        if not data_args.streaming:
+            tokenized_datasets = raw_datasets.map(
+                tokenize_function,
+                batched=True,
+                num_proc=data_args.preprocessing_num_workers,
+                remove_columns=column_names,
+                load_from_cache_file=not data_args.overwrite_cache,
+                desc="Running tokenizer on dataset",
+            )
+        else:
+            tokenized_datasets = raw_datasets.map(
+                tokenize_function,
+                batched=True,
+                remove_columns=column_names,
+            )
+    if hasattr(config, "max_position_embeddings"):
+        max_pos_embeddings = config.max_position_embeddings
     else:
-        train_loader = DataLoader(
-            train_dataset,
-            batch_size=args.batch_size,
-            shuffle=(train_sampler is None),
-            num_workers=args.workers,
-            pin_memory=True,
-            sampler=train_sampler,
-        )
-        val_loader = DataLoader(
-            val_dataset,
-            batch_size=args.batch_size,
-            shuffle=False,
-            num_workers=args.workers,
-            pin_memory=True,
-            sampler=val_sampler,
-        )
-
-    if args.evaluate:
-        validate(val_loader, model, criterion, args)
-        return
-
-    # ZEUS
-    if args.zeus:
-        assert isinstance(train_loader, ZeusDataLoader)
-        epoch_iter = train_loader.epochs()
+        # Define a default value if the attribute is missing in the config.
+        max_pos_embeddings = 1024
+
+    if data_args.block_size is None:
+        block_size = tokenizer.model_max_length
+        if block_size > max_pos_embeddings:
+            logger.warning(
+                f"The tokenizer picked seems to have a very large `model_max_length` ({tokenizer.model_max_length}). "
+                f"Using block_size={min(1024, max_pos_embeddings)} instead. You can change that default value by passing --block_size xxx."
+            )
+            if max_pos_embeddings > 0:
+                block_size = min(1024, max_pos_embeddings)
+            else:
+                block_size = 1024
     else:
-        epoch_iter = range(args.start_epoch, args.epochs)
+        if data_args.block_size > tokenizer.model_max_length:
+            logger.warning(
+                f"The block_size passed ({data_args.block_size}) is larger than the maximum length for the model "
+                f"({tokenizer.model_max_length}). Using block_size={tokenizer.model_max_length}."
+            )
+        block_size = min(data_args.block_size, tokenizer.model_max_length)
 
-    for epoch in epoch_iter:
-        # DATA PARALLEL
-        if args.distributed:
-            train_sampler.set_epoch(epoch)
-
-        # train for one epoch
-        train(train_loader, model, criterion, optimizer, epoch, args)
-
-        # evaluate on validation set
-        acc1 = validate(val_loader, model, criterion, args)
-
-        scheduler.step()
-
-        # ZEUS
-        if args.zeus:
-            assert isinstance(train_loader, ZeusDataLoader)
-            # Scale the accuracy and report to `train_loader`.`
-            train_loader.report_metric(acc1 / 100, higher_is_better=True)
-        elif args.target_metric is not None:
-            if acc1 / 100 >= args.target_metric:
-                print(
-                    "Reached target metric %s in %s epochs.",
-                    args.target_metric,
-                    epoch + 1,
-                )
-                break
-
-
-def train(train_loader, model, criterion, optimizer, epoch, args):
-    batch_time = AverageMeter("Time", ":6.3f")
-    data_time = AverageMeter("Data", ":6.3f")
-    losses = AverageMeter("Loss", ":.4e")
-    top1 = AverageMeter("Acc@1", ":6.2f")
-    top5 = AverageMeter("Acc@5", ":6.2f")
-
-    progress = ProgressMeter(
-        len(train_loader),
-        [batch_time, data_time, losses, top1, top5],
-        prefix="Epoch: [{}]".format(epoch),
-    )
-
-    # switch to train mode
-    model.train()
-
-    end = time.time()
-    for i, (images, target) in enumerate(train_loader):
-        # measure data loading time
-        data_time.update(time.time() - end)
-
-        # DATA PARALLEL
-        if args.gpu is not None:
-            images = images.cuda(args.gpu, non_blocking=True)
-        if torch.cuda.is_available():
-            target = target.cuda(args.gpu, non_blocking=True)
-
-        # compute output
-        output = model(images)
-        loss = criterion(output, target)
-
-        # measure accuracy and record loss
-        acc1, acc5 = accuracy(output, target, topk=(1, 5))
-        losses.update(loss.item(), images.size(0))
-        top1.update(acc1[0], images.size(0))
-        top5.update(acc5[0], images.size(0))
-
-        # compute gradient and do SGD step
-        optimizer.zero_grad()
-        loss.backward()
-        optimizer.step()
-
-        # measure elapsed time
-        batch_time.update(time.time() - end)
-        end = time.time()
-
-        if i % args.print_freq == 0:
-            progress.display(i + 1)
-
-
-def validate(val_loader, model, criterion, args):
-    def run_validate(loader, base_progress=0):
-        with torch.no_grad():
-            end = time.time()
-            for i, (images, target) in enumerate(loader):
-                i = base_progress + i
-                if args.gpu is not None:
-                    images = images.cuda(args.gpu, non_blocking=True)
-                if torch.cuda.is_available():
-                    target = target.cuda(args.gpu, non_blocking=True)
-
-                # compute output
-                output = model(images)
-                loss = criterion(output, target)
-
-                # measure accuracy and record loss
-                acc1, acc5 = accuracy(output, target, topk=(1, 5))
-                losses.update(loss.item(), images.size(0))
-                top1.update(acc1[0], images.size(0))
-                top5.update(acc5[0], images.size(0))
-
-                # measure elapsed time
-                batch_time.update(time.time() - end)
-                end = time.time()
-
-                if i % args.print_freq == 0:
-                    progress.display(i + 1)
-
-    batch_time = AverageMeter("Time", ":6.3f", Summary.NONE)
-    losses = AverageMeter("Loss", ":.4e", Summary.NONE)
-    top1 = AverageMeter("Acc@1", ":6.2f", Summary.AVERAGE)
-    top5 = AverageMeter("Acc@5", ":6.2f", Summary.AVERAGE)
-    progress = ProgressMeter(
-        len(val_loader)
-        + (
-            args.distributed
-            and (
-                len(val_loader.sampler) * args.local_world_size
-                < len(val_loader.dataset)
-            )
-        ),
-        [batch_time, losses, top1, top5],
-        prefix="Test: ",
-    )
-
-    # switch to evaluate mode
-    model.eval()
-
-    run_validate(val_loader)
-
-    # DATA PARALLEL
-    if args.distributed:
-        top1.all_reduce()
-        top5.all_reduce()
+    # Main data processing function that will concatenate all texts from our dataset and generate chunks of block_size.
+    def group_texts(examples):
+        # Concatenate all texts.
+        concatenated_examples = {k: list(chain(*examples[k])) for k in examples.keys()}
+        total_length = len(concatenated_examples[list(examples.keys())[0]])
+        # We drop the small remainder, and if the total_length < block_size  we exclude this batch and return an empty dict.
+        # We could add padding if the model supported it instead of this drop, you can customize this part to your needs.
+        total_length = (total_length // block_size) * block_size
+        # Split by chunks of max_len.
+        result = {
+            k: [t[i : i + block_size] for i in range(0, total_length, block_size)]
+            for k, t in concatenated_examples.items()
+        }
+        result["labels"] = result["input_ids"].copy()
+        return result
+
+    # Note that with `batched=True`, this map processes 1,000 texts together, so group_texts throws away a remainder
+    # for each of those groups of 1,000 texts. You can adjust that batch_size here but a higher value might be slower
+    # to preprocess.
+    #
+    # To speed up this part, we use multiprocessing. See the documentation of the map method for more information:
+    # https://huggingface.co/docs/datasets/process#map
+
+    with training_args.main_process_first(desc="grouping texts together"):
+        if not data_args.streaming:
+            lm_datasets = tokenized_datasets.map(
+                group_texts,
+                batched=True,
+                num_proc=data_args.preprocessing_num_workers,
+                load_from_cache_file=not data_args.overwrite_cache,
+                desc=f"Grouping texts in chunks of {block_size}",
+            )
+        else:
+            lm_datasets = tokenized_datasets.map(
+                group_texts,
+                batched=True,
+            )
 
-    if args.distributed and (
-        len(val_loader.sampler) * args.local_world_size < len(val_loader.dataset)
-    ):
-        aux_val_dataset = Subset(
-            val_loader.dataset,
-            range(
-                len(val_loader.sampler) * args.local_world_size, len(val_loader.dataset)
-            ),
-        )
-        aux_val_loader = torch.utils.data.DataLoader(
-            aux_val_dataset,
-            batch_size=args.batch_size,
-            shuffle=False,
-            num_workers=args.workers,
-            pin_memory=True,
-        )
-        run_validate(aux_val_loader, len(val_loader))
-
-    progress.display_summary()
-
-    return top1.avg
-
-
-class Summary(Enum):
-    NONE = 0
-    AVERAGE = 1
-    SUM = 2
-    COUNT = 3
-
-
-class AverageMeter(object):
-    """Computes and stores the average and current value"""
-
-    def __init__(self, name, fmt=":f", summary_type=Summary.AVERAGE):
-        self.name = name
-        self.fmt = fmt
-        self.summary_type = summary_type
-        self.reset()
-
-    def reset(self):
-        self.val = 0
-        self.avg = 0
-        self.sum = 0
-        self.count = 0
-
-    def update(self, val, n=1):
-        self.val = val
-        self.sum += val * n
-        self.count += n
-        self.avg = self.sum / self.count
-
-    # DATA PARALLEL
-    def all_reduce(self):
-        device = "cuda" if torch.cuda.is_available() else "cpu"
-        total = torch.tensor([self.sum, self.count], dtype=torch.float32, device=device)
-        dist.all_reduce(total, dist.ReduceOp.SUM, async_op=False)
-        self.sum, self.count = total.tolist()
-        self.avg = self.sum / self.count
-
-    def __str__(self):
-        fmtstr = "{name} {val" + self.fmt + "} ({avg" + self.fmt + "})"
-        return fmtstr.format(**self.__dict__)
-
-    def summary(self):
-        fmtstr = ""
-        if self.summary_type is Summary.NONE:
-            fmtstr = ""
-        elif self.summary_type is Summary.AVERAGE:
-            fmtstr = "{name} {avg:.3f}"
-        elif self.summary_type is Summary.SUM:
-            fmtstr = "{name} {sum:.3f}"
-        elif self.summary_type is Summary.COUNT:
-            fmtstr = "{name} {count:.3f}"
+    if training_args.do_train:
+        if "train" not in tokenized_datasets:
+            raise ValueError("--do_train requires a train dataset")
+        train_dataset = lm_datasets["train"]
+        if data_args.max_train_samples is not None:
+            max_train_samples = min(len(train_dataset), data_args.max_train_samples)
+            train_dataset = train_dataset.select(range(max_train_samples))
+
+    if training_args.do_eval:
+        if "validation" not in tokenized_datasets:
+            raise ValueError("--do_eval requires a validation dataset")
+        eval_dataset = lm_datasets["validation"]
+        if data_args.max_eval_samples is not None:
+            max_eval_samples = min(len(eval_dataset), data_args.max_eval_samples)
+            eval_dataset = eval_dataset.select(range(max_eval_samples))
+
+        def preprocess_logits_for_metrics(logits, labels):
+            if isinstance(logits, tuple):
+                # Depending on the model and config, logits may contain extra tensors,
+                # like past_key_values, but logits always come first
+                logits = logits[0]
+            return logits.argmax(dim=-1)
+
+        metric = evaluate.load("accuracy", cache_dir=model_args.cache_dir)
+
+        def compute_metrics(eval_preds):
+            preds, labels = eval_preds
+            # preds have the same shape as the labels, after the argmax(-1) has been calculated
+            # by preprocess_logits_for_metrics but we need to shift the labels
+            labels = labels[:, 1:].reshape(-1)
+            preds = preds[:, :-1].reshape(-1)
+            return metric.compute(predictions=preds, references=labels)
+
+    # Initialize our ZeusMonitor and HFGlobalPowerLimitOptimizer
+    monitor = ZeusMonitor()
+    optimizer = HFGlobalPowerLimitOptimizer(monitor)
+
+    # Initialize our Trainer
+    trainer = Trainer(
+        model=model,
+        args=training_args,
+        train_dataset=train_dataset if training_args.do_train else None,
+        eval_dataset=eval_dataset if training_args.do_eval else None,
+        tokenizer=tokenizer,
+        # Data collator will default to DataCollatorWithPadding, so we change it.
+        data_collator=default_data_collator,
+        compute_metrics=compute_metrics
+        if training_args.do_eval and not is_torch_tpu_available()
+        else None,
+        preprocess_logits_for_metrics=preprocess_logits_for_metrics
+        if training_args.do_eval and not is_torch_tpu_available()
+        else None,
+        callbacks=[optimizer],  # Add the optimizer callback
+    )
+
+    # Training
+    if training_args.do_train:
+        checkpoint = None
+        if training_args.resume_from_checkpoint is not None:
+            checkpoint = training_args.resume_from_checkpoint
+        elif last_checkpoint is not None:
+            checkpoint = last_checkpoint
+        train_result = trainer.train(resume_from_checkpoint=checkpoint)
+        trainer.save_model()  # Saves the tokenizer too for easy upload
+
+        metrics = train_result.metrics
+
+        max_train_samples = (
+            data_args.max_train_samples
+            if data_args.max_train_samples is not None
+            else len(train_dataset)
+        )
+        metrics["train_samples"] = min(max_train_samples, len(train_dataset))
+
+        trainer.log_metrics("train", metrics)
+        trainer.save_metrics("train", metrics)
+        trainer.save_state()
+
+    # Evaluation
+    if training_args.do_eval:
+        logger.info("*** Evaluate ***")
+
+        metrics = trainer.evaluate()
+
+        max_eval_samples = (
+            data_args.max_eval_samples
+            if data_args.max_eval_samples is not None
+            else len(eval_dataset)
+        )
+        metrics["eval_samples"] = min(max_eval_samples, len(eval_dataset))
+        try:
+            perplexity = math.exp(metrics["eval_loss"])
+        except OverflowError:
+            perplexity = float("inf")
+        metrics["perplexity"] = perplexity
+
+        trainer.log_metrics("eval", metrics)
+        trainer.save_metrics("eval", metrics)
+
+    kwargs = {
+        "finetuned_from": model_args.model_name_or_path,
+        "tasks": "text-generation",
+    }
+    if data_args.dataset_name is not None:
+        kwargs["dataset_tags"] = data_args.dataset_name
+        if data_args.dataset_config_name is not None:
+            kwargs["dataset_args"] = data_args.dataset_config_name
+            kwargs[
+                "dataset"
+            ] = f"{data_args.dataset_name} {data_args.dataset_config_name}"
         else:
-            raise ValueError("invalid summary type %r" % self.summary_type)
+            kwargs["dataset"] = data_args.dataset_name
 
-        return fmtstr.format(**self.__dict__)
+    if training_args.push_to_hub:
+        trainer.push_to_hub(**kwargs)
+    else:
+        trainer.create_model_card(**kwargs)
 
 
-class ProgressMeter(object):
-    def __init__(self, num_batches, meters, prefix=""):
-        self.batch_fmtstr = self._get_batch_fmtstr(num_batches)
-        self.meters = meters
-        self.prefix = prefix
-
-    def display(self, batch):
-        entries = [self.prefix + self.batch_fmtstr.format(batch)]
-        entries += [str(meter) for meter in self.meters]
-        print("\t".join(entries))
-
-    def display_summary(self):
-        entries = [" *"]
-        entries += [meter.summary() for meter in self.meters]
-        print(" ".join(entries))
-
-    def _get_batch_fmtstr(self, num_batches):
-        num_digits = len(str(num_batches // 1))
-        fmt = "{:" + str(num_digits) + "d}"
-        return "[" + fmt + "/" + fmt.format(num_batches) + "]"
-
-
-def accuracy(output, target, topk=(1,)):
-    """Computes the accuracy over the k top predictions for the specified values of k"""
-    with torch.no_grad():
-        maxk = max(topk)
-        batch_size = target.size(0)
-
-        _, pred = output.topk(maxk, 1, True, True)
-        pred = pred.t()
-        correct = pred.eq(target.view(1, -1).expand_as(pred))
-
-        res = []
-        for k in topk:
-            correct_k = correct[:k].reshape(-1).float().sum(0, keepdim=True)
-            res.append(correct_k.mul_(100.0 / batch_size))
-        return res
+def _mp_fn(index):
+    # For xla_spawn (TPUs)
+    main()
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `zeus-ml-0.8.2/examples/imagenet/train_dp.py` & `zeus_ml-0.9.0/examples/power_limit_optimizer/train_dp.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,17 +17,16 @@
 import torchvision.transforms as transforms
 import torchvision.datasets as datasets
 import torchvision.models as models
 from torch.utils.data import Subset
 
 # ZEUS
 from zeus.monitor import ZeusMonitor
-from zeus.optimizer import GlobalPowerLimitOptimizer
-from zeus.optimizer.power_limit import MaxSlowdownConstraint
-from zeus.util.env import get_env
+from zeus.optimizer.power_limit import MaxSlowdownConstraint, GlobalPowerLimitOptimizer
+from zeus.utils.env import get_env
 from zeus.callback import Callback, CallbackSet
 
 
 def parse_args() -> argparse.Namespace:
     """Parse command line arguments."""
     # List choices of models
     model_names = sorted(
```

### Comparing `zeus-ml-0.8.2/examples/imagenet/train_single.py` & `zeus_ml-0.9.0/examples/power_limit_optimizer/train_single.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,17 +16,16 @@
 import torch.utils.data.distributed
 import torchvision.transforms as transforms
 import torchvision.datasets as datasets
 import torchvision.models as models
 
 # ZEUS
 from zeus.monitor import ZeusMonitor
-from zeus.optimizer import GlobalPowerLimitOptimizer
-from zeus.optimizer.power_limit import MaxSlowdownConstraint
-from zeus.util.env import get_env
+from zeus.optimizer.power_limit import MaxSlowdownConstraint, GlobalPowerLimitOptimizer
+from zeus.utils.env import get_env
 
 
 def parse_args() -> argparse.Namespace:
     """Parse command line arguments."""
     # List choices of models
     model_names = sorted(
         name
```

### Comparing `zeus-ml-0.8.2/examples/perseus/profile_p2p.py` & `zeus_ml-0.9.0/examples/pipeline_frequency_optimizer/profile_p2p.py`

 * *Files identical despite different names*

### Comparing `zeus-ml-0.8.2/examples/perseus/run_optimization.py` & `zeus_ml-0.9.0/examples/pipeline_frequency_optimizer/run_optimization.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""Example script of running Perseus energy scheduling."""
+"""Example script of running pipeline frequency optimization."""
 
 from __future__ import annotations
 
 import time
 import itertools
 import logging
 from pathlib import Path
```

### Comparing `zeus-ml-0.8.2/examples/trace_driven/run_alibaba.py` & `zeus_ml-0.9.0/examples/research_reproducibility/zeus_nsdi23/run_alibaba.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,18 +21,17 @@
 import multiprocessing as mp
 from pprint import pprint
 from typing import Literal
 from functools import lru_cache
 
 import pandas as pd
 
-from zeus.job import Job
-from zeus.simulate import Simulator
-from zeus.analyze import HistoryEntry
-from zeus.policy import JITPowerLimitOptimizer, PruningGTSBatchSizeOptimizer
+from zeus._legacy.job import Job
+from zeus._legacy.simulate import Simulator, HistoryEntry
+from zeus._legacy.policy import JITPowerLimitOptimizer, PruningGTSBatchSizeOptimizer
 
 
 def parse_args() -> argparse.Namespace:
     """Parse commandline arguments."""
     parser = argparse.ArgumentParser()
     parser.add_argument(
         "--gpu", default="v100", choices=["a40", "v100", "p100", "rtx6000"]
@@ -45,15 +44,17 @@
 def run_simulator(
     gpu: Literal["a40", "v100", "p100", "rtx6000"],
     eta_knob: float,
     beta_knob: float,
 ) -> list[tuple[str, list[HistoryEntry]]]:
     """Run the simulator on the given job."""
     # Read in the Alibaba trace
-    alibaba_df = pd.DataFrame(pd.read_csv("../../trace/alibaba_groups.csv.xz"))
+    alibaba_df = pd.DataFrame(pd.read_csv("../../../trace/alibaba_groups.csv.xz"))
+    print("Read in the Alibaba trace.")
+    print(f"Number of groups: {alibaba_df.group.nunique()}")
 
     # Run simulation on all Alibaba recurring job groups.
     with mp.Pool(mp.cpu_count()) as p:
         alibaba_result = p.starmap(
             simulate_group,
             (
                 (group, gpu, eta_knob, beta_knob)
@@ -92,21 +93,21 @@
 
     return (group.dataset.unique().item(), history)
 
 
 @lru_cache(maxsize=1)
 def read_train_trace() -> pd.DataFrame:
     """Read the train trace file as a Pandas DataFrame."""
-    return pd.DataFrame(pd.read_csv("../../trace/summary_train.csv"))
+    return pd.DataFrame(pd.read_csv("../../../trace/summary_train.csv"))
 
 
 @lru_cache(maxsize=1)
 def read_power_trace(gpu: Literal["a40", "v100", "p100", "rtx6000"]) -> pd.DataFrame:
     """Read the power trace of the given GPU as a Pandas DataFrame."""
-    return pd.DataFrame(pd.read_csv(f"../../trace/summary_power_{gpu}.csv"))
+    return pd.DataFrame(pd.read_csv(f"../../../trace/summary_power_{gpu}.csv"))
 
 
 def get_job_with_defaults(
     gpu: Literal["a40", "v100", "p100", "rtx6000"], dataset: str
 ) -> Job:
     """Instantiate a Job instance with defaults for the given dataset."""
     if dataset not in [
```

### Comparing `zeus-ml-0.8.2/examples/trace_driven/run_single.py` & `zeus_ml-0.9.0/examples/research_reproducibility/zeus_nsdi23/run_single.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,18 +18,20 @@
 
 import argparse
 from pprint import pprint
 from typing import Literal
 
 import pandas as pd
 
-from zeus.job import Job
-from zeus.policy.optimizer import JITPowerLimitOptimizer, PruningGTSBatchSizeOptimizer
-from zeus.simulate import Simulator
-from zeus.analyze import HistoryEntry
+from zeus._legacy.job import Job
+from zeus._legacy.policy.optimizer import (
+    JITPowerLimitOptimizer,
+    PruningGTSBatchSizeOptimizer,
+)
+from zeus._legacy.simulate import Simulator, HistoryEntry
 
 
 def parse_args() -> argparse.Namespace:
     """Parse commandline arguments."""
     parser = argparse.ArgumentParser()
 
     parser.add_argument("--dataset", default="librispeech")
```

### Comparing `zeus-ml-0.8.2/pyproject.toml` & `zeus_ml-0.9.0/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -10,50 +10,58 @@
     {name = "Jae-Won Chung", email = "jwnchung@umich.edu"},
 ]
 license = {text = "Apache 2.0"}
 classifiers = [
     "Environment :: GPU :: NVIDIA CUDA",
     "License :: OSI Approved :: Apache Software License",
     "Topic :: Scientific/Engineering :: Artificial Intelligence",
-    "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
 ]
 keywords = ["deep-learning", "power", "energy", "sustainability", "mlsys"]
-requires-python = ">=3.8"
+requires-python = ">=3.9"
 dependencies = [
     "numpy",
     "pandas",
     "scikit-learn",
     "nvidia-ml-py",
-    "pydantic",  # The `zeus.util.pydantic_v1` compatibility layer allows us to unpin Pydantic in most cases.
+    "pydantic",  # The `zeus.utils.pydantic_v1` compatibility layer allows us to unpin Pydantic in most cases.
     "rich",
     "tyro",
 ]
 dynamic = ["version"]
 
 [project.urls]
 Repository = "https://github.com/ml-energy/zeus"
 Homepage = "https://ml.energy/zeus"
 Documentation = "https://ml.energy/zeus"
 
 [project.optional-dependencies]
 # One day FastAPI will drop support for Pydantic V1. Then fastapi has to be pinned as well.
-perseus = ["fastapi[all]", "pydantic<2", "lowtime", "aiofiles", "httpx"]
-lint = ["ruff", "black==22.6.0"]
-test = ["pytest==7.3.2", "pytest-mock==3.10.0", "pytest-xdist==3.3.1"]
-dev = ["zeus-ml[perseus,lint,test]"]
+pfo = ["pydantic<2", "httpx"]
+pfo-server = ["fastapi[all]", "pydantic<2", "lowtime", "aiofiles", "httpx", "torch"]
+bso = ["pydantic<2", "httpx"]
+bso-server = ["fastapi[all]", "sqlalchemy", "pydantic<2", "python-dotenv"]
+migration = ["alembic", "sqlalchemy", "pydantic<2", "python-dotenv"]
+lint = ["ruff", "black==22.6.0", "pyright", "pandas-stubs", "transformers"]
+test = ["fastapi[all]", "sqlalchemy", "pydantic<2", "httpx", "pytest==7.3.2", "pytest-mock==3.10.0", "pytest-xdist==3.3.1", "anyio==3.7.1", "aiosqlite==0.20.0"]
+docs = ["mkdocs-material[imaging]==9.5.19", "mkdocstrings[python]==0.25.0", "mkdocs-gen-files==0.5.0", "mkdocs-literate-nav==0.6.1", "mkdocs-section-index==0.3.9", "mkdocs-redirects==1.2.1", "urllib3<2", "black"]
+# greenlet is for supporting apple mac silicon for sqlalchemy(https://docs.sqlalchemy.org/en/20/faq/installation.html)
+dev = ["zeus-ml[pfo-server,bso,bso-server,migration,lint,test]", "greenlet"]
 
 [tool.setuptools.packages.find]
 where = ["."]
 
 [tool.setuptools.dynamic]
 version = {attr = "zeus.__version__"}
 
 [tool.ruff]
+line-length = 120
+
+[tool.ruff.lint]
 select = [
   "E",   # pycodestyle error
   "F",   # pyflakes
   "D",   # pydocstyle
   "PL",  # pylint
   "N",   # pep8-naming
   "B",   # flake8-bugbear (detects likely bugs)
@@ -67,20 +75,23 @@
   "PLR0912",  # Too many branches
   "B905",     # zip strict argument
   "PLR0915",  # Too many statements
   "PLR2004",  # Magic values
   "SIM115",   # Context manager for opening files
   "E501",     # Line too long
 ]
-line-length = 120
-
-[tool.ruff.pydocstyle]
-convention = "google"
+pydocstyle.convention = "google"
 
-[tool.ruff.per-file-ignores]
+[tool.ruff.lint.per-file-ignores]
 "**/__init__.py" = ["F401", "F403"]
-"zeus/optimizer/perseus/common.py" = ["N805"]
-"zeus/optimizer/perseus/server/router.py" = ["B008"]
-"zeus/util/pydantic_v1.py" = ["F403"]
+"zeus/optimizer/pipeline_frequency/common.py" = ["N805"]
+"zeus/optimizer/pipeline_frequency/server/router.py" = ["B008"]
+"zeus/utils/pydantic_v1.py" = ["F403"]
+"zeus/optimizer/batch_size/**/commands.py" = ["N805"]
+"zeus/optimizer/batch_size/**/models.py" = ["N805"]
+"zeus/optimizer/batch_size/server/config.py" = ["N805"]
+"zeus/optimizer/batch_size/server/router.py" = ["B008"]
+"zeus/optimizer/batch_size/common.py" = ["N805"]
+"zeus/device/gpu.py" = ["N802", "N803"]
 
 [tool.pytest.ini_options]
 addopts = "--numprocesses auto"
```

### Comparing `zeus-ml-0.8.2/tests/optimizer/test_power_limit_optimizer.py` & `zeus_ml-0.9.0/tests/optimizer/test_power_limit_optimizer.py`

 * *Files 9% similar despite different names*

```diff
@@ -19,25 +19,26 @@
 import typing
 from typing import Generator, Iterable
 from unittest.mock import call
 
 import pytest
 import pandas as pd
 
-from zeus.optimizer import GlobalPowerLimitOptimizer, HFGlobalPowerLimitOptimizer
 from zeus.optimizer.power_limit import (
+    GlobalPowerLimitOptimizer,
+    HFGlobalPowerLimitOptimizer,
     Ready,
     Done,
     Energy,
     Time,
     ZeusCost,
     MaxSlowdownConstraint,
 )
-from zeus.util.testing import ReplayZeusMonitor
-from zeus.util.metric import zeus_cost
+from zeus.utils.testing import ReplayZeusMonitor
+from zeus.utils.metric import zeus_cost
 
 if typing.TYPE_CHECKING:
     from pathlib import Path
     from pytest_mock import MockerFixture
 
 
 PROFILE_DATA_DIR = "tests/profile_data/"
@@ -58,46 +59,55 @@
 
 
 class ReplayLog:
     """Compute the optimal power limit from the JIT profiling log and the eta knob."""
 
     def __init__(self, log_file: str) -> None:
         df = typing.cast(pd.DataFrame, pd.read_csv(log_file))
-        assert all(col.startswith("gpu") and col.endswith("_energy") for col in df.columns[3:])
+        assert all(
+            col.startswith("gpu") and col.endswith("_energy") for col in df.columns[3:]
+        )
         self.gpu_indices = list(map(lambda x: int(x[3]), df.columns[3:]))
 
         df["energy"] = df[df.columns[3:]].sum(axis=1)  # type: ignore
         df["power_limit"] = df.window_name.map(lambda name: int(name.split("_")[-1]))
 
         self.df = df
         self.log_file = log_file
         self.power_limits = df.power_limit.to_list()
 
     def optimal_zeus_cost_power_limit(self, eta_knob: float) -> int:
-        cost = self.df.apply(lambda row: zeus_cost(
-            energy=row["energy"],
-            time=row["elapsed_time"],
-            eta_knob=eta_knob,
-            max_power=max(self.power_limits) * len(self.gpu_indices),
-        ), axis=1)
+        cost = self.df.apply(
+            lambda row: zeus_cost(
+                energy=row["energy"],
+                time=row["elapsed_time"],
+                eta_knob=eta_knob,
+                max_power=max(self.power_limits) * len(self.gpu_indices),
+            ),
+            axis=1,
+        )
         return int(self.df.iloc[cost.argmin()].power_limit)
 
     def optimal_time_power_limit(self) -> int:
         return int(self.df.iloc[self.df.elapsed_time.argmin()].power_limit)
 
     def optimal_energy_power_limit(self) -> int:
         return int(self.df.iloc[self.df.energy.argmin()].power_limit)
 
     def optimal_max_slowdown_constraint_power_limit(self, factor: float) -> int:
-        shortest_time = self.df.query(f"power_limit == {max(self.power_limits)}").elapsed_time.item()
+        shortest_time = self.df.query(
+            f"power_limit == {max(self.power_limits)}"
+        ).elapsed_time.item()
         filtered_df = self.df.query(f"elapsed_time <= {shortest_time * factor}")
         return int(filtered_df.power_limit.min())
 
 
-@pytest.fixture(params=map(lambda p: PROFILE_DATA_DIR + p, os.listdir(PROFILE_DATA_DIR)))
+@pytest.fixture(
+    params=map(lambda p: PROFILE_DATA_DIR + p, os.listdir(PROFILE_DATA_DIR))
+)
 def replay_log(request) -> ReplayLog:
     return ReplayLog(request.param)
 
 
 def training_loop(
     plo: GlobalPowerLimitOptimizer,
     train_loader: Iterable[int],
@@ -122,18 +132,20 @@
     mocker: MockerFixture,
     replay_log: ReplayLog,
     eta_knob: float,
     num_interrupts: int | str,
     tmp_path: Path,
 ):
     # Mock PyNVML.
-    pynvml_mock = mocker.patch("zeus.optimizer.power_limit.pynvml", autospec=True)
+    pynvml_mock = mocker.patch("zeus.device.gpu.pynvml", autospec=True)
     pynvml_mock.nvmlDeviceGetHandleByIndex.side_effect = lambda i: f"handle{i}"
-    pynvml_mock.nvmlDeviceGetPowerManagementLimitConstraints.side_effect = \
-        lambda _: (min(replay_log.power_limits) * 1000, max(replay_log.power_limits) * 1000)
+    pynvml_mock.nvmlDeviceGetPowerManagementLimitConstraints.side_effect = lambda _: (
+        min(replay_log.power_limits) * 1000,
+        max(replay_log.power_limits) * 1000,
+    )
 
     # Mock away the atexit hook, which raises an NVML error when testing finishes.
     mocker.patch("zeus.optimizer.power_limit.atexit", autospec=True)
 
     monitor = ReplayZeusMonitor(
         log_file=replay_log.log_file,
         ignore_sync_cuda=True,
@@ -203,22 +215,26 @@
                 break
             for i in sorted(monitor.gpu_indices):
                 call_list.append(call(f"handle{i}", power_limit * 1000))
         # The else clause runs if the for loop was not interrupted with `break`.
         else:
             # After being interrupted, the PLO will set the power limit to the max.
             for i in sorted(monitor.gpu_indices):
-                call_list.append(call(f"handle{i}", max(replay_log.power_limits) * 1000))
+                call_list.append(
+                    call(f"handle{i}", max(replay_log.power_limits) * 1000)
+                )
             # Return the power limit back to the list for retry.
             power_limits.insert(0, power_limit)
     # If the final power limit tried was the optimal one, the PLO will not set it again.
     if power_limit != optimal_pl:
         for i in sorted(monitor.gpu_indices):
             call_list.append(call(f"handle{i}", optimal_pl * 1000))
-    pynvml_mock.nvmlDeviceSetPowerManagementLimit.assert_has_calls(call_list, any_order=False)
+    pynvml_mock.nvmlDeviceSetPowerManagementLimit.assert_has_calls(
+        call_list, any_order=False
+    )
     pynvml_mock.reset_mock()
 
     # Print out the profile data for debugging purposes.
     with open(tmp_path / "power_limit_optimizer.json", "r") as f:
         print(f.read())
 
     ########################################
@@ -226,34 +242,41 @@
     ########################################
     temp_plo = GlobalPowerLimitOptimizer(
         monitor,
         optimum_selector=Energy(),
         profile_path=tmp_path / "power_limit_optimizer.json",
     )
     assert isinstance(temp_plo.state, Done)
-    assert temp_plo.state.optimal_power_limit == replay_log.optimal_energy_power_limit() * 1000
-
+    assert (
+        temp_plo.state.optimal_power_limit
+        == replay_log.optimal_energy_power_limit() * 1000
+    )
 
     temp_plo = GlobalPowerLimitOptimizer(
         monitor,
         optimum_selector=Time(),
         profile_path=tmp_path / "power_limit_optimizer.json",
     )
     assert isinstance(temp_plo.state, Done)
-    assert temp_plo.state.optimal_power_limit == replay_log.optimal_time_power_limit() * 1000
-
+    assert (
+        temp_plo.state.optimal_power_limit
+        == replay_log.optimal_time_power_limit() * 1000
+    )
 
     for factor in [1.0, 1.1, 1.2, 1.5, 2.0, 3.0, 5.0, 100.0]:
         temp_plo = GlobalPowerLimitOptimizer(
             monitor,
             optimum_selector=MaxSlowdownConstraint(factor=factor),
             profile_path=tmp_path / "power_limit_optimizer.json",
         )
         assert isinstance(temp_plo.state, Done)
-        assert temp_plo.state.optimal_power_limit == replay_log.optimal_max_slowdown_constraint_power_limit(factor) * 1000
+        assert (
+            temp_plo.state.optimal_power_limit
+            == replay_log.optimal_max_slowdown_constraint_power_limit(factor) * 1000
+        )
 
     ########################################
     # Test loading from saved profile data
     ########################################
     plo = GlobalPowerLimitOptimizer(
         monitor,
         optimum_selector=ZeusCost(
@@ -269,13 +292,16 @@
     training_loop(plo, train_loader, num_epochs=1)
 
     pynvml_mock.nvmlDeviceSetPowerManagementLimit.assert_has_calls(
         [call(f"handle{i}", optimal_pl * 1000) for i in sorted(monitor.gpu_indices)],
         any_order=False,
     )
 
+
 def test_HFGPLO_signature_equivalence() -> None:
     """Ensure that the constructor signatures of GlobalPowerLimitOptimizer and HFGlobalPowerLimitOptimizer are equivalent."""
     gplo_signature = inspect.signature(GlobalPowerLimitOptimizer.__init__)
     hfgplo_signature = inspect.signature(HFGlobalPowerLimitOptimizer.__init__)
 
-    assert gplo_signature == hfgplo_signature, "GlobalPowerLimitOptimizer and HFGlobalPowerLimitOptimizer signatures do not match."
+    assert (
+        gplo_signature == hfgplo_signature
+    ), "GlobalPowerLimitOptimizer and HFGlobalPowerLimitOptimizer signatures do not match."
```

### Comparing `zeus-ml-0.8.2/tests/test_monitor.py` & `zeus_ml-0.9.0/tests/test_monitor.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,41 +19,47 @@
 from itertools import product, combinations
 from typing import Generator, TYPE_CHECKING, Sequence
 
 import pynvml
 import pytest
 
 from zeus.monitor import Measurement, ZeusMonitor
-from zeus.util.testing import ReplayZeusMonitor
+from zeus.utils.testing import ReplayZeusMonitor
+import zeus.device.gpu
 
 if TYPE_CHECKING:
     from pathlib import Path
     from unittest.mock import MagicMock
     from pytest_mock import MockerFixture
 
 NUM_GPUS = 4
 ARCHS = [
     pynvml.NVML_DEVICE_ARCH_PASCAL,
     pynvml.NVML_DEVICE_ARCH_VOLTA,
     pynvml.NVML_DEVICE_ARCH_AMPERE,
 ]
 
 
+@pytest.fixture(autouse=True, scope="function")
+def reset_gpus() -> None:
+    """Reset the global variable `_gpus` to None on every test."""
+    zeus.device.gpu._gpus = None
+
+
 @pytest.fixture
 def pynvml_mock(mocker: MockerFixture):
     """Mock the entire pynvml module."""
-    mock = mocker.patch("zeus.monitor.energy.pynvml", autospec=True)
-    
+    # Mock the pynvml import in the gpu module.
+    mock = mocker.patch("zeus.device.gpu.pynvml", autospec=True)
+
     # Except for the arch constants.
     mock.NVML_DEVICE_ARCH_PASCAL = pynvml.NVML_DEVICE_ARCH_PASCAL
     mock.NVML_DEVICE_ARCH_VOLTA = pynvml.NVML_DEVICE_ARCH_VOLTA
     mock.NVML_DEVICE_ARCH_AMPERE = pynvml.NVML_DEVICE_ARCH_AMPERE
 
-    mocker.patch("zeus.util.env.pynvml", mock)
-
     return mock
 
 
 def gpu_cases():
     """Generates all the cases for different GPU indices and architectures.
 
     We start with `NUM_GPUS` GPUs. We then consider all possible combinations of
@@ -61,23 +67,28 @@
     creates a mapping between the indices visible to PyTorch and the indices visible
     to NVML. We then consider all possible combinations of `gpu_indices`, which
     creates a mapping between the indices visible to PyTorch and the indices visible
     to `ZeusMonitor`. Finally, with only the GPUs that were left after filtering
     with `CUDA_VISIBLE_DEVICES` and `gpu_monitor`, we assign all possible combinations
     GPU architectures to `gpu_archs`.
     """
-    def nonempty_subsequences(indices: Sequence[int]) -> Generator[list[int], None, None]:
+
+    def nonempty_subsequences(
+        indices: Sequence[int],
+    ) -> Generator[list[int], None, None]:
         """Returns all non-empty subsets of `indices`."""
         for length in range(1, len(indices) + 1):
             yield from map(list, combinations(indices, r=length))
 
     # `CUDA_VISIBLE_DEVICES` is given.
     for cuda_visible_devices in nonempty_subsequences(range(NUM_GPUS)):  # NVML index
         # `gpu_indices` is not `None`.
-        for gpu_indices in nonempty_subsequences(range(len(cuda_visible_devices))):  # PyTorch index
+        for gpu_indices in nonempty_subsequences(
+            range(len(cuda_visible_devices))
+        ):  # PyTorch index
             for gpu_archs in product(ARCHS, repeat=len(gpu_indices)):
                 yield cuda_visible_devices, gpu_indices, list(gpu_archs)
         # `gpu_indices` is `None` (use all GPUs visible to PyTorch).
         for gpu_archs in product(ARCHS, repeat=len(cuda_visible_devices)):
             yield cuda_visible_devices, None, list(gpu_archs)
     # `CUDA_VISIBLE_DEVICES` is not given (use all GPUs in the system).
     # `gpu_indices` is not `None`.
@@ -86,15 +97,17 @@
             yield None, gpu_indices, list(gpu_archs)
     # `gpu_indices` is `None` (use all GPUs visible to PyTorch).
     for gpu_archs in product(ARCHS, repeat=NUM_GPUS):
         yield None, None, list(gpu_archs)
 
 
 @pytest.fixture(params=gpu_cases())
-def mock_gpus(request, mocker: MockerFixture, pynvml_mock: MagicMock) -> tuple[tuple[int], tuple[int]]:
+def mock_gpus(
+    request, mocker: MockerFixture, pynvml_mock: MagicMock
+) -> tuple[tuple[int], tuple[int]]:
     """Mock `pynvml` so that it looks like there are GPUs with the given archs.
 
     This fixture automatically generates (1) all combinations of possible GPU indices
     (e.g., (0,), (1, 3), (0, 2, 3)) and takes assigns all possible combinations of
     GPU architectures (e.g., (PASCAL,), (VOLTA, VOLTA), (AMPERE, PASCAL, VOLTA)), and
     (2) all combinations of selecting four GPU architectures with replacement and
     matches it with `None` for the GPU indices (e.g., (None, (PASCAL, PASCAL, VOLTA, AMPERE))).
@@ -104,29 +117,35 @@
     Thus `request.param` has type `tuple[tuple[int], tuple[int]]` where the former
     is GPU indices and the latter is GPU architectures.
     """
     cuda_visible_devices, gpu_indices, archs = request.param
 
     def mock_pynvml(nvml_indices: list[int], archs: list[int]) -> None:
         assert len(nvml_indices) == len(archs)
-        index_to_handle = {i: f"handle{i}" for i in nvml_indices}
         handle_to_arch = {f"handle{i}": arch for i, arch in zip(nvml_indices, archs)}
         pynvml_mock.nvmlDeviceGetCount.return_value = NUM_GPUS
-        pynvml_mock.nvmlDeviceGetHandleByIndex.side_effect = lambda index: index_to_handle[index]
-        pynvml_mock.nvmlDeviceGetArchitecture.side_effect = lambda handle: handle_to_arch[handle]
+        pynvml_mock.nvmlDeviceGetHandleByIndex.side_effect = (
+            lambda index: f"handle{index}"
+        )  # GPU Monitoring object grabs all handles visible to system on initialization.
+        pynvml_mock.nvmlDeviceGetArchitecture.side_effect = (
+            lambda handle: handle_to_arch[handle]
+        )
 
     if cuda_visible_devices is None:  # All GPUs are visible to PyTorch.
         # When `CUDA_VISIBLE_DEVICES` is not given, NVML indices and PyTorch indices conincide.
         if gpu_indices is None:
             mock_pynvml(list(range(NUM_GPUS)), archs)
         else:
             mock_pynvml(gpu_indices, archs)
 
     else:  # `CUDA_VISIBLE_DEVICES` is given, limiting the set of visible GPUs to PyTorch.
-        mocker.patch.dict("os.environ", {"CUDA_VISIBLE_DEVICES": ",".join(map(str, cuda_visible_devices))})
+        mocker.patch.dict(
+            "os.environ",
+            {"CUDA_VISIBLE_DEVICES": ",".join(map(str, cuda_visible_devices))},
+        )
         # Valid NVML indices are determined by `cuda_visible_devices` and `gpu_indices`.
         if gpu_indices is None:
             mock_pynvml(cuda_visible_devices, archs)
         else:
             # We need to translate `gpu_indices` to NVML indices.
             mock_pynvml([cuda_visible_devices[idx] for idx in gpu_indices], archs)
 
@@ -147,40 +166,54 @@
             torch_gpu_indices = list(range(len(cuda_visible_devices)))
         else:
             nvml_gpu_indices = [cuda_visible_devices[idx] for idx in gpu_indices]
             torch_gpu_indices = gpu_indices
     assert len(nvml_gpu_indices) == len(torch_gpu_indices) == len(gpu_archs)
 
     num_gpus = len(gpu_archs)
-    is_old_nvml = {index: arch < pynvml.NVML_DEVICE_ARCH_VOLTA for index, arch in zip(nvml_gpu_indices, gpu_archs)}
-    is_old_torch = {index: arch < pynvml.NVML_DEVICE_ARCH_VOLTA for index, arch in zip(torch_gpu_indices, gpu_archs)}
+    is_old_nvml = {
+        index: arch < pynvml.NVML_DEVICE_ARCH_VOLTA
+        for index, arch in zip(nvml_gpu_indices, gpu_archs)
+    }
+    is_old_torch = {
+        index: arch < pynvml.NVML_DEVICE_ARCH_VOLTA
+        for index, arch in zip(torch_gpu_indices, gpu_archs)
+    }
     old_gpu_torch_indices = [index for index, is_old in is_old_torch.items() if is_old]
 
-    mocker.patch("zeus.monitor.energy.atexit.register")
-
     class MockPowerMonitor:
-        def __init__(self, gpu_indices: list[int] | None, update_period: float | None) -> None:
+        def __init__(
+            self, gpu_indices: list[int] | None, update_period: float | None
+        ) -> None:
             assert gpu_indices == old_gpu_torch_indices
             self.gpu_indices = gpu_indices
             self.update_period = update_period
+
         def get_energy(self, start: float, end: float) -> dict[int, float]:
             return {i: -1.0 for i in self.gpu_indices}
+
     mocker.patch("zeus.monitor.energy.PowerMonitor", MockPowerMonitor)
 
     time_counter = itertools.count(start=4, step=1)
     mocker.patch("zeus.monitor.energy.time", side_effect=time_counter)
 
     energy_counters = {
         f"handle{i}": itertools.count(start=1000, step=3)
-        for i in nvml_gpu_indices if not is_old_nvml[i]
+        for i in nvml_gpu_indices
+        if not is_old_nvml[i]
     }
-    pynvml_mock.nvmlDeviceGetTotalEnergyConsumption.side_effect = lambda handle: next(energy_counters[handle])
+    pynvml_mock.nvmlDeviceGetTotalEnergyConsumption.side_effect = lambda handle: next(
+        energy_counters[handle]
+    )
 
     log_file = tmp_path / "log.csv"
 
+    # want to make zeus.device.gpu.nvml_is_available is a function, want it to always return true when testing
+    mocker.patch("zeus.device.gpu.nvml_is_available", return_value=True)
+
     ########################################
     # Test ZeusMonitor initialization.
     ########################################
     monitor = ZeusMonitor(gpu_indices=gpu_indices, log_file=log_file)
 
     # Check GPU index parsing from the log file.
     replay_monitor = ReplayZeusMonitor(gpu_indices=None, log_file=log_file)
@@ -197,19 +230,20 @@
 
     def assert_window_begin(name: str, begin_time: int):
         """Assert monitor measurement states right after a window begins."""
         assert monitor.measurement_states[name][0] == begin_time
         assert monitor.measurement_states[name][1] == {
             # `4` is the time origin of `time_counter`.
             i: pytest.approx((1000 + 3 * (begin_time - 4)) / 1000.0)
-            for i in torch_gpu_indices if not is_old_torch[i]
+            for i in torch_gpu_indices
+            if not is_old_torch[i]
         }
-        pynvml_mock.nvmlDeviceGetTotalEnergyConsumption.assert_has_calls([
-            call(f"handle{i}") for i in nvml_gpu_indices if not is_old_nvml[i]
-        ])
+        pynvml_mock.nvmlDeviceGetTotalEnergyConsumption.assert_has_calls(
+            [call(f"handle{i}") for i in nvml_gpu_indices if not is_old_nvml[i]]
+        )
         pynvml_mock.nvmlDeviceGetTotalEnergyConsumption.reset_mock()
 
     def assert_measurement(
         name: str,
         measurement: Measurement,
         begin_time: int,
         elapsed_time: int,
@@ -232,39 +266,41 @@
             if not is_old_torch[i]:
                 # The energy counter increments with step size 3.
                 assert measurement.energy[i] == pytest.approx(elapsed_time * 3 / 1000.0)
 
         if not assert_calls:
             return
 
-        pynvml_mock.nvmlDeviceGetTotalEnergyConsumption.assert_has_calls([
-            call(f"handle{i}") for i in nvml_gpu_indices if not is_old_nvml[i]
-        ])
+        pynvml_mock.nvmlDeviceGetTotalEnergyConsumption.assert_has_calls(
+            [call(f"handle{i}") for i in nvml_gpu_indices if not is_old_nvml[i]]
+        )
         pynvml_mock.nvmlDeviceGetTotalEnergyConsumption.reset_mock()
 
-
     # Serial non-overlapping windows.
     monitor.begin_window("window1", sync_cuda=False)
     assert_window_begin("window1", 4)
 
     tick()
 
     # Calling `begin_window` again with the same name should raise an error.
     with pytest.raises(ValueError, match="already exists"):
         monitor.begin_window("window1", sync_cuda=False)
 
     measurement = monitor.end_window("window1", sync_cuda=False)
     assert_measurement("window1", measurement, begin_time=4, elapsed_time=2)
 
-    tick(); tick()
+    tick()
+    tick()
 
     monitor.begin_window("window2", sync_cuda=False)
     assert_window_begin("window2", 9)
 
-    tick(); tick(); tick()
+    tick()
+    tick()
+    tick()
 
     measurement = monitor.end_window("window2", sync_cuda=False)
     assert_measurement("window2", measurement, begin_time=9, elapsed_time=4)
 
     # Calling `end_window` again with the same name should raise an error.
     with pytest.raises(ValueError, match="does not exist"):
         monitor.end_window("window2", sync_cuda=False)
@@ -278,38 +314,43 @@
     assert_window_begin("window3", 14)
 
     tick()
 
     monitor.begin_window("window4", sync_cuda=False)
     assert_window_begin("window4", 16)
 
-    tick(); tick();
+    tick()
+    tick()
 
     measurement = monitor.end_window("window3", sync_cuda=False)
     assert_measurement("window3", measurement, begin_time=14, elapsed_time=5)
 
-    tick(); tick(); tick();
+    tick()
+    tick()
+    tick()
 
     measurement = monitor.end_window("window4", sync_cuda=False)
     assert_measurement("window4", measurement, begin_time=16, elapsed_time=7)
 
-
     # Nested windows.
     monitor.begin_window("window5", sync_cuda=False)
     assert_window_begin("window5", 24)
 
     monitor.begin_window("window6", sync_cuda=False)
     assert_window_begin("window6", 25)
 
-    tick(); tick();
+    tick()
+    tick()
 
     measurement = monitor.end_window("window6", sync_cuda=False)
     assert_measurement("window6", measurement, begin_time=25, elapsed_time=3)
 
-    tick(); tick(); tick();
+    tick()
+    tick()
+    tick()
 
     measurement = monitor.end_window("window5", sync_cuda=False)
     assert_measurement("window5", measurement, begin_time=24, elapsed_time=8)
 
     ########################################
     # Test content of `log_file`.
     ########################################
@@ -351,37 +392,49 @@
     ########################################
     # Currently the testing infrastructure does not support old GPU architectures that
     # require the Zeus monitor binary. So we skip this test if any of the GPUs are old.
     if any(is_old_nvml.values()):
         return
 
     replay_monitor.begin_window("window1", sync_cuda=False)
-    
+
     # Calling `begin_window` again with the same name should raise an error.
     with pytest.raises(RuntimeError, match="is already ongoing"):
         replay_monitor.begin_window("window1", sync_cuda=False)
 
     measurement = replay_monitor.end_window("window1", sync_cuda=False)
-    assert_measurement("window1", measurement, begin_time=5, elapsed_time=2, assert_calls=False)
+    assert_measurement(
+        "window1", measurement, begin_time=5, elapsed_time=2, assert_calls=False
+    )
 
     # Calling `end_window` with a non-existant window name should raise an error.
     with pytest.raises(RuntimeError, match="is not ongoing"):
         replay_monitor.end_window("window2", sync_cuda=False)
 
     replay_monitor.begin_window("window2", sync_cuda=False)
     measurement = replay_monitor.end_window("window2", sync_cuda=False)
-    assert_measurement("window2", measurement, begin_time=10, elapsed_time=4, assert_calls=False)
+    assert_measurement(
+        "window2", measurement, begin_time=10, elapsed_time=4, assert_calls=False
+    )
 
     replay_monitor.begin_window("window3", sync_cuda=False)
     replay_monitor.begin_window("window4", sync_cuda=False)
 
     measurement = replay_monitor.end_window("window3", sync_cuda=False)
-    assert_measurement("window3", measurement, begin_time=15, elapsed_time=5, assert_calls=False)
+    assert_measurement(
+        "window3", measurement, begin_time=15, elapsed_time=5, assert_calls=False
+    )
     measurement = replay_monitor.end_window("window4", sync_cuda=False)
-    assert_measurement("window4", measurement, begin_time=17, elapsed_time=7, assert_calls=False)
+    assert_measurement(
+        "window4", measurement, begin_time=17, elapsed_time=7, assert_calls=False
+    )
 
     replay_monitor.begin_window("window5", sync_cuda=False)
     replay_monitor.begin_window("window6", sync_cuda=False)
     measurement = replay_monitor.end_window("window6", sync_cuda=False)
-    assert_measurement("window6", measurement, begin_time=26, elapsed_time=3, assert_calls=False)
+    assert_measurement(
+        "window6", measurement, begin_time=26, elapsed_time=3, assert_calls=False
+    )
     measurement = replay_monitor.end_window("window5", sync_cuda=False)
-    assert_measurement("window5", measurement, begin_time=25, elapsed_time=8, assert_calls=False)
+    assert_measurement(
+        "window5", measurement, begin_time=25, elapsed_time=8, assert_calls=False
+    )
```

### Comparing `zeus-ml-0.8.2/tests/util/test_env.py` & `zeus_ml-0.9.0/tests/utils/test_env.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 import os
 from typing import Any
 from contextlib import contextmanager
 
 import pytest
 
-from zeus.util.env import get_env
+from zeus.utils.env import get_env
 
 
 @contextmanager
 def temp_env(key: str, value: Any):
     if key in os.environ:
         old = os.environ[key]
         os.environ[key] = str(value)
```

### Comparing `zeus-ml-0.8.2/zeus/__init__.py` & `zeus_ml-0.9.0/zeus/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,20 +10,16 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Zeus is a framework for deep learning energy measurement and optimization.
 
-- [`run`][zeus.run]: Machinery for actually running Zeus.
-- [`monitor`][zeus.monitor]: Class for profiling energy inside training scripts.
-- [`optimizer`][zeus.optimizer]: A collection of optimizers for various knobs.
-- [`callback`][zeus.callback]: Callback definition.
-- [`controller`][zeus.controller]: A collection of controllers that influence training flow.
-- [`analyze`][zeus.analyze]: Functions for analyzing log files.
-- [`job`][zeus.job]: Job specification.
-- [`simulate`][zeus.simulate]: Machinery for trace-driven Zeus.
-- [`policy`][zeus.policy]: Collection of optimization policies.
-- [`util`][zeus.util]: Utility functions and classes.
+- [`optimizer`][zeus.optimizer]: A collection of optimizers for time and energy
+- [`monitor`][zeus.monitor]: Programmatic power and energy measurement tools
+- [`utils`][zeus.utils]: Utility functions and classes.
+- [`_legacy`][zeus._legacy.policy]: Legacy code mostly to keep our papers reproducible
+- [`device`][zeus.device]: Abstraction layer over compute devices
+- [`callback`][zeus.callback]: Callback definition
 """
 
-__version__ = "0.8.2"
+__version__ = "0.9.0"
```

### Comparing `zeus-ml-0.8.2/zeus/analyze.py` & `zeus_ml-0.9.0/zeus/utils/metric.py`

 * *Files 15% similar despite different names*

```diff
@@ -8,44 +8,45 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""Utilities for result analysis."""
+"""Defines the energy-time cost metric function."""
 
 from __future__ import annotations
 
-from dataclasses import dataclass
 from datetime import timedelta
 from pathlib import Path
 from typing import cast
 
 import pandas as pd
 from sklearn.metrics import auc
 
 
-@dataclass
-class HistoryEntry:
-    """Represents the config and result of a job run that may have failed.
-
-    Attributes:
-        bs: Batch size
-        pl: Power limit
-        energy: Energy consumption in Joules
-        reached: Whether the target metric was reached at the end
-        time: Time consumption in seconds
-    """
+def zeus_cost(
+    energy: float, time: float, eta_knob: float, max_power: int | float
+) -> float:
+    """Compute Zeus's energy-time cost metric.
+
+    Trades off ETA and TTA based on the value of `eta_knob`.
+    The caller is expected to do bound checking for `eta_knob`,
+    because `eta_knob` does not change frequently.
+
+    Args:
+        energy: Joules
+        time: seconds
+        eta_knob: Real number in [0, 1].
+        max_power: The maximum power limit of the GPU.
 
-    bs: int
-    pl: int
-    energy: float
-    reached: bool
-    time: float
+    Returns:
+        The cost of the DL training job.
+    """
+    return eta_knob * energy + (1 - eta_knob) * max_power * time
 
 
 # ruff: noqa: PLR2004
 def energy(
     logfile: Path | str,
     start: float | None = None,
     end: float | None = None,
```

### Comparing `zeus-ml-0.8.2/zeus/callback.py` & `zeus_ml-0.9.0/zeus/callback.py`

 * *Files identical despite different names*

### Comparing `zeus-ml-0.8.2/zeus/job.py` & `zeus_ml-0.9.0/zeus/_legacy/job.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 from __future__ import annotations
 
 from dataclasses import dataclass, field
 
 import pandas as pd
 
-from zeus.util import LinearScaler, SquareRootScaler
+from zeus.utils.lr_scaler import LinearScaler, SquareRootScaler
 
 
 @dataclass(frozen=True, unsafe_hash=True)
 class Job:
     """Job specification tuple.
 
     Attributes:
@@ -32,15 +32,15 @@
         network: Name of the DNN model.
         optimizer: Name of the optimizer, e.g. Adam.
         target_metric: Target validation metric.
         max_epochs: Maximum number of epochs to train before terminating.
         default_bs: Initial batch size (b0) provided by the user.
         default_lr: Learning rate corresponding to the default batch size.
         workdir: Working directory in which to launch the job command.
-        command: Job command template. See [`gen_command`][zeus.job.Job.gen_command].
+        command: Job command template. See [`gen_command`][zeus._legacy.job.Job.gen_command].
     """
 
     dataset: str
     network: str
     optimizer: str
     target_metric: float
     max_epochs: int
```

### Comparing `zeus-ml-0.8.2/zeus/monitor/__init__.py` & `zeus_ml-0.9.0/zeus/monitor/__init__.py`

 * *Files identical despite different names*

### Comparing `zeus-ml-0.8.2/zeus/monitor/__main__.py` & `zeus_ml-0.9.0/zeus/monitor/__main__.py`

 * *Files identical despite different names*

### Comparing `zeus-ml-0.8.2/zeus/monitor/energy.py` & `zeus_ml-0.9.0/zeus/monitor/energy.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,26 +13,23 @@
 # limitations under the License.
 
 """Measure the GPU time and energy consumption of a block of code."""
 
 from __future__ import annotations
 
 import os
-import atexit
 from time import time
 from pathlib import Path
 from dataclasses import dataclass
-from functools import cached_property, lru_cache
-
-import pynvml
+from functools import cached_property
 
 from zeus.monitor.power import PowerMonitor
-from zeus.util.logging import get_logger
-from zeus.util.framework import cuda_sync
-from zeus.util.env import resolve_gpu_indices
+from zeus.utils.logging import get_logger
+from zeus.utils.framework import cuda_sync
+from zeus.device import get_gpus
 
 logger = get_logger(__name__)
 
 
 @dataclass
 class Measurement:
     """Measurement result of one window.
@@ -64,14 +61,17 @@
     energy and time consumed will be recorded. Multiple concurrent measurement windows
     are supported.
 
     For Volta or newer GPUs, energy consumption is measured very cheaply with the
     `nvmlDeviceGetTotalEnergyConsumption` API. On older architectures, this API is
     not supported, so a separate Python process is used to poll `nvmlDeviceGetPowerUsage`
     to get power samples over time, which are integrated to compute energy consumption.
+    Since it is spawning the process, the monitor should not be instantiated as a global variable.
+    Python puts a protection to prevent creating a process in global scope.
+    Refer to the "Safe importing of main module" section in https://docs.python.org/3/library/multiprocessing.html for more detail.
 
     ## Integration Example
 
     ```python
     from zeus.monitor import ZeusMontior
 
     # Time/Energy measurements for four GPUs will begin and end at the same time.
@@ -94,16 +94,14 @@
     for gpu_idx, gpu_energy in result.energy.items():
         print(f"GPU {gpu_idx} consumed {gpu_energy} Joules.")
     ```
 
     Attributes:
         gpu_indices (`list[int]`): Indices of all the CUDA devices to monitor, from the
             DL framework's perspective after applying `CUDA_VISIBLE_DEVICES`.
-        nvml_gpu_indices (`list[int]`): Indices of all the CUDA devices to monitor, from
-            NVML/system's perspective.
     """
 
     def __init__(
         self,
         gpu_indices: list[int] | None = None,
         approx_instant_energy: bool = False,
         log_file: str | Path | None = None,
@@ -124,26 +122,21 @@
                 instantaneous power consumption with the window's execution time. This should
                 be a better estimate than zero, but it's still an approximation.
             log_file: Path to the log CSV file. If `None`, logging will be disabled.
         """
         # Save arguments.
         self.approx_instant_energy = approx_instant_energy
 
-        # Initialize NVML.
-        pynvml.nvmlInit()
-        atexit.register(pynvml.nvmlShutdown)
-
-        # CUDA GPU indices and NVML GPU indices are different if `CUDA_VISIBLE_DEVICES` is set.
-        self.gpu_indices, self.nvml_gpu_indices = resolve_gpu_indices(gpu_indices)
-
-        # Save all the NVML GPU handles. These should be called with system-level GPU indices.
-        self.gpu_handles: dict[int, pynvml.c_nvmlDevice_t] = {}
-        for nvml_gpu_index, gpu_index in zip(self.nvml_gpu_indices, self.gpu_indices):
-            handle = pynvml.nvmlDeviceGetHandleByIndex(nvml_gpu_index)
-            self.gpu_handles[gpu_index] = handle
+        # Get gpus
+        self.gpus = get_gpus()
+
+        # Get GPU indices:
+        self.gpu_indices = (
+            gpu_indices if gpu_indices is not None else list(range(len(self.gpus)))
+        )
 
         # Initialize loggers.
         if log_file is None:
             self.log_file = None
         else:
             if dir := os.path.dirname(log_file):
                 os.makedirs(dir, exist_ok=True)
@@ -162,44 +155,28 @@
         #     2) Total energy consumed by each >= Volta GPU at the beginning of
         #        this window (`None` for older GPUs).
         self.measurement_states: dict[str, tuple[float, dict[int, float]]] = {}
 
         # Initialize power monitors for older architecture GPUs.
         old_gpu_indices = [
             gpu_index
-            for gpu_index, is_new in zip(self.gpu_indices, self._is_new_arch_flags)
-            if not is_new
+            for gpu_index in self.gpu_indices
+            if not self.gpus.supportsGetTotalEnergyConsumption(gpu_index)
         ]
         if old_gpu_indices:
             self.power_monitor = PowerMonitor(
                 gpu_indices=old_gpu_indices, update_period=None
             )
         else:
             self.power_monitor = None
 
-    @lru_cache
-    def _is_new_arch(self, gpu: int) -> bool:
-        """Return whether the GPU is Volta or newer."""
-        return (
-            pynvml.nvmlDeviceGetArchitecture(self.gpu_handles[gpu])
-            >= pynvml.NVML_DEVICE_ARCH_VOLTA
-        )
-
-    @cached_property
-    def _is_new_arch_flags(self) -> list[bool]:
-        """A list of flags indicating whether each GPU is Volta or newer."""
-        return [self._is_new_arch(gpu) for gpu in self.gpu_handles]
-
     def _get_instant_power(self) -> tuple[dict[int, float], float]:
         """Measure the power consumption of all GPUs at the current time."""
         power_measurement_start_time: float = time()
-        power = {
-            i: pynvml.nvmlDeviceGetPowerUsage(h) / 1000.0
-            for i, h in self.gpu_handles.items()
-        }
+        power = {i: self.gpus.getPowerUsage(i) / 1000.0 for i in self.gpu_indices}
         power_measurement_time = time() - power_measurement_start_time
         return power, power_measurement_time
 
     def begin_window(self, key: str, sync_cuda: bool = True) -> None:
         """Begin a new measurement window.
 
         Args:
@@ -209,27 +186,27 @@
         """
         # Make sure the key is unique.
         if key in self.measurement_states:
             raise ValueError(f"Measurement window '{key}' already exists")
 
         # Call cudaSynchronize to make sure we freeze at the right time.
         if sync_cuda:
-            for gpu_index in self.gpu_handles:
+            for gpu_index in self.gpu_indices:
                 cuda_sync(gpu_index)
 
         # Freeze the start time of the profiling window.
         timestamp: float = time()
         energy_state: dict[int, float] = {}
-        for gpu_index, gpu_handle in self.gpu_handles.items():
+        for gpu_index in self.gpu_indices:
             # Query energy directly if the GPU has newer architecture.
             # Otherwise, the Zeus power monitor is running in the background to
             # collect power consumption, so we just need to read the log file later.
-            if self._is_new_arch(gpu_index):
+            if self.gpus.supportsGetTotalEnergyConsumption(gpu_index):
                 energy_state[gpu_index] = (
-                    pynvml.nvmlDeviceGetTotalEnergyConsumption(gpu_handle) / 1000.0
+                    self.gpus.getTotalEnergyConsumption(gpu_index) / 1000.0
                 )
 
         # Add measurement state to dictionary.
         self.measurement_states[key] = (timestamp, energy_state)
         logger.debug("Measurement window '%s' started.", key)
 
     def end_window(
@@ -260,31 +237,29 @@
         # as early as possible will lead to more accurate energy approximation.
         power, power_measurement_time = (
             self._get_instant_power() if self.approx_instant_energy else ({}, 0.0)
         )
 
         # Call cudaSynchronize to make sure we freeze at the right time.
         if sync_cuda:
-            for gpu_index in self.gpu_handles:
+            for gpu_index in self.gpu_indices:
                 cuda_sync(gpu_index)
 
         # If the measurement window is cancelled, return an empty Measurement object.
         if cancel:
             logger.debug("Measurement window '%s' cancelled.", key)
-            return Measurement(time=0.0, energy={gpu: 0.0 for gpu in self.gpu_handles})
+            return Measurement(time=0.0, energy={gpu: 0.0 for gpu in self.gpu_indices})
 
         end_time: float = time()
         time_consumption: float = end_time - start_time
         energy_consumption: dict[int, float] = {}
-        for gpu_index, gpu_handle in self.gpu_handles.items():
+        for gpu_index in self.gpu_indices:
             # Query energy directly if the GPU has newer architecture.
-            if self._is_new_arch(gpu_index):
-                end_energy = (
-                    pynvml.nvmlDeviceGetTotalEnergyConsumption(gpu_handle) / 1000.0
-                )
+            if self.gpus.supportsGetTotalEnergyConsumption(gpu_index):
+                end_energy = self.gpus.getTotalEnergyConsumption(gpu_index) / 1000.0
                 energy_consumption[gpu_index] = end_energy - start_energy[gpu_index]
 
         # If there are older GPU architectures, the PowerMonitor will take care of those.
         if self.power_monitor is not None:
             energy = self.power_monitor.get_energy(start_time, end_time)
             # Fallback to the instant power measurement if the PowerMonitor does not
             # have the power samples.
```

### Comparing `zeus-ml-0.8.2/zeus/monitor/power.py` & `zeus_ml-0.9.0/zeus/monitor/power.py`

 * *Files 7% similar despite different names*

```diff
@@ -18,76 +18,76 @@
 
 import atexit
 import typing
 import tempfile
 from time import time, sleep
 import multiprocessing as mp
 
-import pynvml
 import pandas as pd
 from sklearn.metrics import auc
 
-from zeus.util.logging import get_logger
-from zeus.util.env import resolve_gpu_indices
+from zeus.utils.logging import get_logger
+from zeus.device import get_gpus
 
 
-def infer_counter_update_period(nvml_handles: list[pynvml.c_nvmlDevice_t]) -> float:
+def infer_counter_update_period(gpu_indicies: list[int]) -> float:
     """Infer the update period of the NVML power counter.
 
     NVML counters can update as slow as 10 Hz depending on the GPU model, so
     there's no need to poll them too faster than that. This function infers the
     update period for each unique GPU model and selects the fastest-updating
     period detected. Then, it returns half the period to ensure that the
     counter is polled at least twice per update period.
     """
-    pynvml.nvmlInit()
-
     logger = get_logger(__name__)
 
+    # get gpus
+    gpus = get_gpus()
+
     # For each unique GPU model, infer the update period.
     update_period = 0.0
     gpu_models_covered = set()
-    for handle in nvml_handles:
-        if (model := pynvml.nvmlDeviceGetName(handle)) not in gpu_models_covered:
+    for index in gpu_indicies:
+        if (model := gpus.getName(index)) not in gpu_models_covered:
             logger.info(
                 "Detected %s, inferring NVML power counter update period.", model
             )
             gpu_models_covered.add(model)
-            detected_period = _infer_counter_update_period_single(handle)
+            detected_period = _infer_counter_update_period_single(index)
             logger.info(
                 "Counter update period for %s is %.2f s",
                 model,
                 detected_period,
             )
             if update_period > detected_period:
                 update_period = detected_period
 
-    pynvml.nvmlShutdown()
-
     # Target half the update period to ensure that the counter is enough.
     update_period /= 2.0
 
     # Anything less than ten times a second is probably too slow.
     if update_period > 0.1:
         logger.warning(
             "Inferred update period (%.2f s) is too long. Using 0.1 s instead.",
             update_period,
         )
         update_period = 0.1
     return update_period
 
 
-def _infer_counter_update_period_single(nvml_handle: pynvml.c_nvmlDevice_t) -> float:
+def _infer_counter_update_period_single(gpu_index: int) -> float:
     """Infer the update period of the NVML power counter for a single GPU."""
+    # get gpus
+    gpus = get_gpus()
     # Collect 1000 samples of the power counter with timestamps.
     time_power_samples: list[tuple[float, int]] = [(0.0, 0) for _ in range(1000)]
     for i in range(len(time_power_samples)):
         time_power_samples[i] = (
             time(),
-            pynvml.nvmlDeviceGetPowerUsage(nvml_handle),
+            gpus.getPowerUsage(gpu_index),
         )
 
     # Find the timestamps when the power readings changed.
     changed_times = []
     prev_power = time_power_samples[0][1]
     for t, p in time_power_samples:
         if p != prev_power:
@@ -115,56 +115,59 @@
     def __init__(
         self,
         gpu_indices: list[int] | None = None,
         update_period: float | None = None,
     ) -> None:
         """Initialize the power monitor.
 
+        Initialization should not be done in global scope due to python's protection.
+        Refer to the "Safe importing of main module" section in https://docs.python.org/3/library/multiprocessing.html for more detail.
+
         Args:
             gpu_indices: Indices of the GPUs to monitor. If None, monitor all GPUs.
             update_period: Update period of the power monitor in seconds. If None,
                 infer the update period by max speed polling the power counter for
                 each GPU model.
         """
         if gpu_indices is not None and not gpu_indices:
             raise ValueError("`gpu_indices` must be either `None` or non-empty")
 
-        # Initialize NVML.
-        pynvml.nvmlInit()
+        # Get GPUs
+        gpus = get_gpus()
 
         # Set up logging.
         self.logger = get_logger(type(self).__name__)
 
-        # Get GPU indices and NVML handles.
-        self.gpu_indices, nvml_gpu_indices = resolve_gpu_indices(gpu_indices)
-        nvml_handles = [pynvml.nvmlDeviceGetHandleByIndex(i) for i in nvml_gpu_indices]
+        # Get GPUs
+        self.gpu_indices = (
+            gpu_indices if gpu_indices is not None else list(range(len(gpus)))
+        )
         self.logger.info("Monitoring power usage of GPUs %s", self.gpu_indices)
 
         # Infer the update period if necessary.
         if update_period is None:
-            update_period = infer_counter_update_period(nvml_handles)
+            update_period = infer_counter_update_period(self.gpu_indices)
         self.update_period = update_period
 
         # Create the CSV file for power measurements.
         power_csv = tempfile.mkstemp(suffix=".csv", text=True)[1]
         open(power_csv, "w").close()
         self.power_f = open(power_csv)
         self.power_df_columns = ["time"] + [f"power{i}" for i in self.gpu_indices]
         self.power_df = pd.DataFrame(columns=self.power_df_columns)
 
         # Spawn the power polling process.
         atexit.register(self._stop)
         self.process = mp.get_context("spawn").Process(
-            target=_polling_process, args=(nvml_gpu_indices, power_csv, update_period)
+            target=_polling_process, args=(self.gpu_indices, power_csv, update_period)
         )
         self.process.start()
 
     def _stop(self) -> None:
         """Stop monitoring power usage."""
-        pynvml.nvmlShutdown()
         if self.process is not None:
             self.process.terminate()
             self.process.join(timeout=1.0)
             self.process.kill()
             self.process = None
 
     def _update_df(self) -> None:
@@ -235,31 +238,29 @@
                 # This means that the time is after the last recorded power reading.
                 row = self.power_df.iloc[-1]
 
         return {i: float(row[f"power{i}"]) for i in self.gpu_indices}
 
 
 def _polling_process(
-    nvml_gpu_indices: list[int],
+    gpu_indices: list[int],
     power_csv: str,
     update_period: float,
 ) -> None:
     """Run the power monitor."""
     try:
-        pynvml.nvmlInit()
-        nvml_handles = [pynvml.nvmlDeviceGetHandleByIndex(i) for i in nvml_gpu_indices]
+        # Get GPUs
+        gpus = get_gpus()
 
         # Use line buffering.
         with open(power_csv, "w", buffering=1) as power_f:
             while True:
                 power: list[float] = []
                 now = time()
-                for nvml_handle in nvml_handles:
-                    power.append(pynvml.nvmlDeviceGetPowerUsage(nvml_handle))
+                for index in gpu_indices:
+                    power.append(gpus.getPowerUsage(index))
                 power_str = ",".join(map(lambda p: str(p / 1000), power))
                 power_f.write(f"{now},{power_str}\n")
                 if (sleep_time := update_period - (time() - now)) > 0:
                     sleep(sleep_time)
     except KeyboardInterrupt:
         return
-    finally:
-        pynvml.nvmlShutdown()
```

### Comparing `zeus-ml-0.8.2/zeus/optimizer/__init__.py` & `zeus_ml-0.9.0/zeus/utils/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,13 +8,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""A collection of optimizers for various knobs."""
-
-from zeus.optimizer.power_limit import (
-    GlobalPowerLimitOptimizer,
-    HFGlobalPowerLimitOptimizer,
-)
+"""Utility functions and classes."""
```

### Comparing `zeus-ml-0.8.2/zeus/optimizer/perseus/__init__.py` & `zeus_ml-0.9.0/zeus/optimizer/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,13 +8,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""Optimizer that schedules energy consumption with Perseus.
-
-Currently, this optimizer depends on PyTorch.
-"""
-
-from zeus.optimizer.perseus.optimizer import PerseusOptimizer
+"""Zeus energy optimizers."""
```

### Comparing `zeus-ml-0.8.2/zeus/optimizer/perseus/common.py` & `zeus_ml-0.9.0/zeus/optimizer/pipeline_frequency/common.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,41 +8,40 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""Shared constants and models between the Perseus server and the client (optimizer)."""
+"""Shared constants and models between the server and the client (optimizer)."""
 
 from __future__ import annotations
 
 import os
 import inspect
 from datetime import datetime
 from typing import Any, Optional
 
 import aiofiles
 import pandas as pd
 
-from zeus.util.pydantic_v1 import BaseModel, BaseSettings, Field, validator, PyObject
+from zeus.utils.pydantic_v1 import BaseModel, BaseSettings, Field, validator, PyObject
 
 GET_SERVER_INFO_URL = "/info"
 REGISTER_JOB_URL = "/register_job"
 REGISTER_RANK_URL = "/register_rank/{job_id}"
 GET_FREQUENCY_SCHEDULE_URL = "/schedule/{job_id}"
 REPORT_PROFILING_RESULT_URL = "/result/{job_id}"
 
 
-class PerseusSettings(BaseSettings):
-    """Perseus settings, configurable via environment variables.
+class PFOServerSettings(BaseSettings):
+    """PFO server settings, configurable via environment variables.
 
-    For instance, setting `PERSEUS_SCHEDULER=AllMaxFrequency` will automatically
-    import `zeus.optimizer.perseus.server.scheduler.AllMaxFrequency` and
-    the `scheduler` variable will hold it a reference to the class.
+    For instance, setting `ZEUS_PFO_LOG_LEVEL=INFO` will automatically set
+    the `log_level` variable to `"INFO"`.
 
     Attributes:
         scheduler: Name of the `FrequencyScheduler` to use.
         scheduler_args: Any extra arguments required by `scheduler.__init__`.
         log_level: Log level, e.g. "debug", "info".
         dump_data: Whether the scheduler should dump internal state to the filesystem
             (for future inspection purposes).
@@ -56,37 +55,37 @@
     log_level: str = "DEBUG"
     dump_data: bool = True
     dump_dir: str = "./dump"
     max_job_idle_time: int = 60 * 60 * 24 * 7  # 1 week
 
     @validator("scheduler", pre=True)
     def _fix_scheduler_import_path(cls, value):
-        """Prepend `zeus.optimizer.perseus.server.scheduler.` to the scheduler type name."""
-        return f"zeus.optimizer.perseus.server.scheduler.{value}"
+        """Prepend `zeus.optimizer.pipeline_frequency.server.scheduler.` to the scheduler type name."""
+        return f"zeus.optimizer.pipeline_frequency.server.scheduler.{value}"
 
     @validator("scheduler_args")
     def _validate_scheduler_args(cls, args, values):
         """Check whether args are as expected by the scheduler's constructor."""
         scheduler = values["scheduler"]
-        full_args = args | dict(job_info=None, rank_infos=None, perseus_settings=None)
+        full_args = args | dict(job_info=None, rank_infos=None, pfo_settings=None)
         constructor_args = inspect.signature(scheduler)
         try:
             constructor_args.bind(**full_args)
         except TypeError as e:
             raise ValueError(f"Invalid scheduler args: {e}") from None
         return args
 
     @validator("log_level")
     def _make_upper_case(cls, value):
         return value.upper()
 
-    class Config:
+    class Config:  # type: ignore
         """Configuration class read by pydantic."""
 
-        env_prefix = "perseus_"
+        env_prefix = "zeus_pfo_"
 
 
 class JobInfo(BaseModel):
     """Training job information reported to the server.
 
     Attributes:
         job_id: Globally unique ID of the training job, generated by the server.
```

### Comparing `zeus-ml-0.8.2/zeus/optimizer/perseus/frequency_controller.py` & `zeus_ml-0.9.0/zeus/optimizer/pipeline_frequency/frequency_controller.py`

 * *Files 26% similar despite different names*

```diff
@@ -16,28 +16,28 @@
 
 from __future__ import annotations
 
 import atexit
 import contextlib
 import multiprocessing as mp
 
-import pynvml
+from zeus.device import get_gpus, ZeusGPUNotSupportedError
 
 
 class FrequencyController:
     """Spawns a separate process that sets the GPU frequency."""
 
-    def __init__(self, nvml_device_id: int = 0) -> None:
+    def __init__(self, device_id: int = 0) -> None:
         """Instantiate the frequency controller.
 
         Args:
-            nvml_device_id: The NVML device ID of the GPU to control.
+            device_id: Device ID of the GPU to control.
         """
         self._q: mp.Queue[int | None] = mp.Queue()
-        self._proc = mp.Process(target=self._controller_process, args=(nvml_device_id,))
+        self._proc = mp.Process(target=self._controller_process, args=(device_id,))
 
         atexit.register(self.end)
         self._proc.start()
 
     def set_frequency(self, frequency: int) -> None:
         """Set the GPU's frequency asynchronously.
 
@@ -48,42 +48,34 @@
 
     def end(self) -> None:
         """Stop the controller process."""
         self._q.put(None, block=False)
 
     def _controller_process(self, device_id: int) -> None:
         """Receive frequency values through a queue and apply it."""
-        pynvml.nvmlInit()
-        handle = pynvml.nvmlDeviceGetHandleByIndex(device_id)
-
+        gpus = get_gpus()
         # Return the power limit to the default.
-        pynvml.nvmlDeviceSetPowerManagementLimit(
-            handle,
-            pynvml.nvmlDeviceGetPowerManagementDefaultLimit(handle),
-        )
+        gpus.resetPowerManagementLimit(device_id)
 
         # Set the memory frequency to be the highest.
-        max_mem_freq = max(pynvml.nvmlDeviceGetSupportedMemoryClocks(handle))
-        with contextlib.suppress(pynvml.NVMLError_NotSupported):  # type: ignore
-            pynvml.nvmlDeviceSetMemoryLockedClocks(handle, max_mem_freq, max_mem_freq)
+        max_mem_freq = max(gpus.getSupportedMemoryClocks(device_id))
+        with contextlib.suppress(ZeusGPUNotSupportedError):
+            gpus.setMemoryLockedClocks(device_id, max_mem_freq, max_mem_freq)
 
         # Set the SM frequency to be the highest.
-        max_freq = max(
-            pynvml.nvmlDeviceGetSupportedGraphicsClocks(handle, max_mem_freq)
-        )
-        pynvml.nvmlDeviceSetGpuLockedClocks(handle, max_freq, max_freq)
+        max_freq = max(gpus.getSupportedGraphicsClocks(device_id, max_mem_freq))
+        gpus.setGpuLockedClocks(device_id, max_freq, max_freq)
         current_freq = max_freq
 
         # Wait on the queue for the next frequency to set.
         while True:
             target_freq = self._q.get(block=True)
             if target_freq is None:
                 break
             if current_freq != target_freq:
-                pynvml.nvmlDeviceSetGpuLockedClocks(handle, target_freq, target_freq)
+                gpus.setGpuLockedClocks(device_id, target_freq, target_freq)
                 current_freq = target_freq
 
         # Reset everything.
-        with contextlib.suppress(pynvml.NVMLError_NotSupported):  # type: ignore
-            pynvml.nvmlDeviceResetMemoryLockedClocks(handle)
-        pynvml.nvmlDeviceResetGpuLockedClocks(handle)
-        pynvml.nvmlShutdown()
+        with contextlib.suppress(ZeusGPUNotSupportedError):
+            gpus.resetMemoryLockedClocks(device_id)
+        gpus.resetGpuLockedClocks(device_id)
```

### Comparing `zeus-ml-0.8.2/zeus/optimizer/perseus/optimizer.py` & `zeus_ml-0.9.0/zeus/optimizer/pipeline_frequency/optimizer.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,45 +8,44 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""Perseus optimizer implementation.
+"""Pipeline frequency optimizer implementation.
 
-The `PerseusOptimizer` is to be integrated into the user-side framework.
-It is responsible for communicating with the Perseus server and managing
+The `PipelineFrequencyOptimizer` is to be integrated into the training framework.
+It is responsible for communicating with the PFO server and managing
 the `FrequencyController` instance, which is responsible for controlling
 the frequency of the CPU of the current process.
 """
 
 from __future__ import annotations
 
 import httpx
-import pynvml
 import torch
 import torch.distributed as dist
 
 from zeus.callback import Callback
-from zeus.optimizer.perseus.frequency_controller import FrequencyController
-from zeus.optimizer.perseus.common import (
+from zeus.device import get_gpus
+from zeus.optimizer.pipeline_frequency.frequency_controller import FrequencyController
+from zeus.optimizer.pipeline_frequency.common import (
     GET_FREQUENCY_SCHEDULE_URL,
     REGISTER_JOB_URL,
     REGISTER_RANK_URL,
     JobInfo,
     RankInfo,
     FrequencySchedule,
 )
-from zeus.util.env import resolve_gpu_indices
-from zeus.util.framework import cuda_sync
+from zeus.utils.framework import cuda_sync
 
 
-class PerseusOptimizer(Callback):
-    """Perseus optimizer."""
+class PipelineFrequencyOptimizer(Callback):
+    """Pipeline frequency optimizer."""
 
     def __init__(
         self,
         rank: int,
         dp_rank: int,
         pp_rank: int,
         tp_rank: int,
@@ -54,183 +53,173 @@
         dp_degree: int,
         pp_degree: int,
         tp_degree: int,
         world_size: int,
         server_url: str,
         job_metadata: str | None = None,
     ) -> None:
-        """Initialize the Perseus optimizer.
+        """Initialize the Pipeline frequency optimizer.
 
         Assumptions:
             - `torch.distributed` has been initialized.
             - `torch.cuda.set_device` has been called with `device_id`.
                 This is needed to broadcast the job ID to all ranks.
 
         The master process (rank 0) will register the job with the Peresus
         server and retrieve the job ID of this job. Then, each rank will
-        report itself to the Perseus server with the job ID.
+        report itself to the PFO server with the job ID.
 
         Args:
             rank: Global rank of the current process.
             dp_rank: Rank in the data parallel group.
             pp_rank: Rank in the pipeline parallel group.
             tp_rank: Rank in the tensor parallel group.
             device_id: CUDA device ID that the current process manages.
             dp_degree: Size of the data parallel group.
             pp_degree: Size of the pipeline parallel group.
             tp_degree: Size of the tensor parallel group.
             world_size: Total number of ranks that participate in training.
-            server_url: URL of the Perseus server.
+            server_url: URL of the PFO server.
             job_metadata: An optional arbitrary string that describes the job. This will
                 be appended to the job ID if given. Typically for logging purposes.
         """
         if not dist.is_initialized():
             raise RuntimeError(
-                "Instantiate `PerseusOptimizer` after `init_process_group`."
+                "Instantiate `PipelineFrequencyOptimizer` after `init_process_group`."
             )
 
         self.server_url = server_url
         self.rank = rank
         self.dp_rank = dp_rank
         self.pp_rank = pp_rank
         self.tp_rank = tp_rank
+        self.device_id = device_id
 
-        cuda_device_ids, nvml_device_ids = resolve_gpu_indices([device_id])
-        self.cuda_device_id = cuda_device_ids[0]
-        nvml_device_id = nvml_device_ids[0]
-        # It is assumed that `torch.cuda.set_device` has been called with `device_id`.
-        # It won't hurt to call this again.
-        torch.cuda.set_device(self.cuda_device_id)
+        gpus = get_gpus()
+        torch.cuda.set_device(device_id)
 
-        # Rank 0 registers the job with the Perseus server and retrieves the job ID.
+        # Rank 0 registers the job with the PFO server and retrieves the job ID.
         job_id = None
         if rank == 0:
             job_info = JobInfo(
                 pp_degree=pp_degree,
                 dp_degree=dp_degree,
                 tp_degree=tp_degree,
                 world_size=world_size,
                 job_metadata=job_metadata,
             )
             response = httpx.post(
                 self.server_url + REGISTER_JOB_URL, json=job_info.dict()
             )
             if (code := response.status_code) != 200:
                 raise RuntimeError(
-                    f"Perseus server returned status code {code}: {response.text}"
+                    f"PFO server returned status code {code}: {response.text}"
                 )
             job_id = response.json()
             if not isinstance(job_id, str):
-                raise RuntimeError(
-                    f"Perseus server returned a strange job ID: {job_id=}"
-                )
+                raise RuntimeError(f"PFO server returned a strange job ID: {job_id=}")
 
         # Rank 0 broadcasts the job ID across all ranks.
         objects = [job_id]
         dist.broadcast_object_list(objects, src=0)
         self.job_id = objects[0]
         if self.job_id is None:
             raise RuntimeError("Failed to broadcast job ID to all ranks")
 
         # Query the list of available frequencies of the GPU.
-        pynvml.nvmlInit()
-        handle = pynvml.nvmlDeviceGetHandleByIndex(nvml_device_id)
-        max_mem_freq = max(pynvml.nvmlDeviceGetSupportedMemoryClocks(handle))
+        max_mem_freq = max(gpus.getSupportedMemoryClocks(device_id))
         freqs = sorted(
-            pynvml.nvmlDeviceGetSupportedGraphicsClocks(handle, max_mem_freq),
+            gpus.getSupportedGraphicsClocks(device_id, max_mem_freq),
             reverse=True,
         )
-        pynvml.nvmlShutdown()
 
-        # Each rank reports itself to the Perseus server with the job ID.
+        # Each rank reports itself to the PFO server with the job ID.
         rank_info = RankInfo(
             rank=self.rank,
             dp_rank=self.dp_rank,
             pp_rank=self.pp_rank,
             tp_rank=self.tp_rank,
             available_frequencies=freqs,
         )
         response = httpx.post(
             self.server_url + REGISTER_RANK_URL.format(job_id=self.job_id),
             json=rank_info.dict(),
         )
         if (code := response.status_code) != 200:
             raise RuntimeError(
-                f"Perseus server returned status code {code}: {response.text}"
+                f"PFO server returned status code {code}: {response.text}"
             )
 
         # The frequency controller is responsible for controlling the frequency
-        # of the GPU (nvml_device_id) asynchronously.
-        self.frequency_controller = FrequencyController(nvml_device_id=nvml_device_id)
+        # of the GPU (device_id) asynchronously.
+        self.frequency_controller = FrequencyController(device_id=device_id)
 
-        # Fetch the frequency schedule from the Perseus server.
+        # Fetch the frequency schedule from the PFO server.
         self.freq_schedule = self._get_frequency_schedule()
         self.freq_schedule_iter = iter(self.freq_schedule)
 
     def _get_frequency_schedule(self) -> list[tuple[str, int]]:
-        """Get the frequency schedule from the Perseus server."""
+        """Get the frequency schedule from the PFO server."""
         response = httpx.get(
             self.server_url + GET_FREQUENCY_SCHEDULE_URL.format(job_id=self.job_id),
             params={"rank": self.rank},
             timeout=None,
         )
         if (code := response.status_code) != 200:
             raise RuntimeError(
-                f"Perseus server returned status code {code}: {response.text}"
+                f"PFO server returned status code {code}: {response.text}"
             )
         schedule = FrequencySchedule.parse_raw(response.text)
         if schedule.rank != self.rank:
             raise RuntimeError(
-                f"Perseus server returned a schedule for rank {schedule.rank} to rank {self.rank}"
+                f"PFO server returned a schedule for rank {schedule.rank} to rank {self.rank}"
             )
         return schedule.frequencies
 
     def on_step_begin(self) -> None:
         """Mark the beginning of a step.
 
         TODO(jaywonchung): InstructionProfiler iteration start mark.
         """
         pass
 
     def on_step_end(self) -> None:
         """Mark the end of a step.
 
         TODO(jaywonchung): InstructionProfiler iteration end mark.
-        Also report the profiling result to the Perseus server after N iterations.
+        Also report the profiling result to the PFO server after N iterations.
         """
         # Frequency schedule holds one iteration-worth of frequencies, so at
         # the end of each iteration, the iterator should be exhausted.
         item = next(self.freq_schedule_iter, None)
         if item is not None:
             raise RuntimeError(
-                "Perseus server returned more frequencies than expected. "
+                "PFO server returned more frequencies than expected. "
                 f"Next expected instruction and frequency is {item}"
             )
         self.freq_schedule_iter = iter(self.freq_schedule)
 
     def on_instruction_begin(self, name: str) -> None:
         """Mark the beginning of an instruction, like forward and backward.
 
         Retrieve the next frequency from the schedule, check whether the next
         expected instruction matches the name of the instruction, and set the
         frequency accordingly.
         """
-        cuda_sync(self.cuda_device_id)
+        cuda_sync(self.device_id)
 
         # Retrieve the next frequency from the schedule.
         item = next(self.freq_schedule_iter, None)
         if item is None:
-            raise RuntimeError(
-                "Perseus server returned fewer frequencies than expected"
-            )
+            raise RuntimeError("PFO server returned fewer frequencies than expected")
 
         # Check whether the next expected instruction matches the name of the instruction.
         instruction, frequency = item
         if instruction != name:
             raise RuntimeError(
                 f"The next expected instruction is not forward: {instruction}"
             )
 
         self.frequency_controller.set_frequency(frequency)
 
-    def on_instruction_end(self, _: str) -> None:
+    def on_instruction_end(self, name: str) -> None:
         """Mark the end of an instruction, like forward and backward."""
```

### Comparing `zeus-ml-0.8.2/zeus/optimizer/perseus/server/__init__.py` & `zeus_ml-0.9.0/zeus/optimizer/pipeline_frequency/server/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -8,15 +8,16 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""The Perseus server guides the PerseusOptimizer with frequency plans.
+"""The server guides the `PipelineFrequencyOptimizer` with frequency plans.
 
-The server is agnostic to the training framework the PerseusOptimizer
+The server is agnostic to the training framework the
+[`PipelineFrequencyOptimizer`][zeus.optimizer.pipeline_frequency.optimizer.PipelineFrequencyOptimizer]
 is integrated with. A server is useful because large model training is
 typically distributed, and we still need one place to coordinate the
 frequency plans. Later, the server will be extended to support complete
 online profiling and optimization.
 """
```

### Comparing `zeus-ml-0.8.2/zeus/optimizer/perseus/server/job_manager.py` & `zeus_ml-0.9.0/zeus/optimizer/pipeline_frequency/server/job_manager.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,53 +18,53 @@
 
 import time
 import asyncio
 import traceback
 
 from fastapi import HTTPException
 
-from zeus.optimizer.perseus.common import (
+from zeus.optimizer.pipeline_frequency.common import (
     JobInfo,
-    PerseusSettings,
+    PFOServerSettings,
     FrequencySchedule,
     ProfilingResult,
     RankInfo,
     save_prof,
     save_sched,
     save_ranks,
 )
-from zeus.util.logging import get_logger
-from zeus.util.async_utils import create_task
+from zeus.utils.logging import get_logger
+from zeus.utils.async_utils import create_task
 
 GLOBAL_JOB_MANAGER: JobManager | None = None
 
 logger = get_logger(__name__)
 
 
 class JobManager:
     """A singleton class that manages all states."""
 
-    def __init__(self, perseus_settings: PerseusSettings) -> None:
+    def __init__(self, pfo_settings: PFOServerSettings) -> None:
         """Initialize the job manager."""
-        self.perseus_settings = perseus_settings
+        self.pfo_settings = pfo_settings
 
         self._job_infos: dict[str, JobInfo] = {}
         self._job_rank_infos: dict[str, list[RankInfo]] = {}
         self._job_tasks: dict[str, asyncio.Task] = {}
         self._job_result_channels: dict[str, asyncio.Queue[ProfilingResult]] = {}
         self._job_sched_request_channels: dict[str, asyncio.Queue] = {}
         self._job_sched_response_channels: dict[str, list[asyncio.Queue]] = {}
         self._job_last_active_time: dict[str, float] = {}
 
         # Spawn cleanup task that evicts the state of jobs that have not been active
         # for a long time.
         create_task(
             self._cleanup_task(
                 cleanup_period=60,
-                max_idle_time=perseus_settings.max_job_idle_time,
+                max_idle_time=pfo_settings.max_job_idle_time,
             ),
             logger=logger,
         )
 
     def register_job(self, job_info: JobInfo) -> None:
         """Prepare internal state for a new job.
 
@@ -76,15 +76,15 @@
         self._job_rank_infos[job_id] = []
         self._job_result_channels[job_id] = asyncio.Queue(maxsize=world_size)
         self._job_sched_request_channels[job_id] = asyncio.Queue(maxsize=world_size)
         self._job_sched_response_channels[job_id] = [
             asyncio.Queue(maxsize=1) for _ in range(world_size)
         ]
         self._job_tasks[job_id] = create_task(
-            self._job_task(job_id, self.perseus_settings.dump_data),
+            self._job_task(job_id, self.pfo_settings.dump_data),
             logger=logger,
         )
         self._job_last_active_time[job_id] = time.monotonic()
 
     def register_rank(self, job_id: str, rank_info: RankInfo) -> None:
         """Register rank-specific information for an already registered job.
 
@@ -169,25 +169,25 @@
                 # in `self.job_rank_infos[job_id]`.
                 if len(rank_infos) == job_info.world_size:
                     break
 
             # Sort `RankInfo`s in rank order.
             rank_infos.sort(key=lambda r: r.rank)
 
-            # Create directory to dump Perseus states.
-            dump_dir = f"{self.perseus_settings.dump_dir}/{job_id}"
+            # Create directory to dump PFO server states.
+            dump_dir = f"{self.pfo_settings.dump_dir}/{job_id}"
             if dump_data:
                 await save_ranks(rank_infos, dump_dir)
 
             # Instantiate the frequency scheduler.
-            scheduler = self.perseus_settings.scheduler(
+            scheduler = self.pfo_settings.scheduler(
                 job_info,
                 rank_infos,
-                self.perseus_settings,
-                **self.perseus_settings.scheduler_args,
+                self.pfo_settings,
+                **self.pfo_settings.scheduler_args,
             )
 
             # Provide next schedules, observe profiling results, and repeat.
             schedule_num = 0
             while True:
                 # Compute the next `FrequencySchedule`s.
                 schedules = scheduler.next_schedule()
@@ -224,17 +224,17 @@
             # In case the scheduler errored, send out the exception to the clients.
             # The clients will receive the error when they ask for the next schedule.
             for chan in sched_resp_chan:
                 chan.put_nowait(exc)
             raise
 
 
-def init_global_job_manager(perseus_settings: PerseusSettings) -> None:
+def init_global_job_manager(pfo_settings: PFOServerSettings) -> None:
     """Instantiate the global singleton `JobManager`."""
     global GLOBAL_JOB_MANAGER
-    GLOBAL_JOB_MANAGER = JobManager(perseus_settings=perseus_settings)
+    GLOBAL_JOB_MANAGER = JobManager(pfo_settings=pfo_settings)
 
 
 def get_global_job_manager() -> JobManager:
     """Fetch the global singleton `JobManager`."""
     assert GLOBAL_JOB_MANAGER is not None, "`init_global_job_manager` was not called."
     return GLOBAL_JOB_MANAGER
```

### Comparing `zeus-ml-0.8.2/zeus/optimizer/perseus/server/router.py` & `zeus_ml-0.9.0/zeus/optimizer/pipeline_frequency/server/router.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,37 +8,37 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""Perseus server FastAPI router."""
+"""Pipeline frequency optimizer server FastAPI router."""
 
 from __future__ import annotations
 
 import logging
 from typing import Callable
 
 from fastapi import Depends, FastAPI, Response, Request
 from fastapi.routing import APIRoute
 
-from zeus.util.logging import get_logger
-from zeus.optimizer.perseus.common import (
+from zeus.utils.logging import get_logger
+from zeus.optimizer.pipeline_frequency.common import (
     REGISTER_JOB_URL,
     REGISTER_RANK_URL,
     GET_FREQUENCY_SCHEDULE_URL,
     REPORT_PROFILING_RESULT_URL,
     JobInfo,
     RankInfo,
-    PerseusSettings,
+    PFOServerSettings,
     ProfilingResult,
     FrequencySchedule,
 )
-from zeus.optimizer.perseus.server.job_manager import (
+from zeus.optimizer.pipeline_frequency.server.job_manager import (
     JobManager,
     init_global_job_manager,
     get_global_job_manager,
 )
 
 logger = get_logger(__name__)
 app = FastAPI()
@@ -61,15 +61,15 @@
                 response.body.decode(response.charset),
             )
             return response
 
         return custom_route_handler
 
 
-settings = PerseusSettings()
+settings = PFOServerSettings()
 logging.basicConfig(level=logging.getLevelName(settings.log_level))
 if logging.getLevelName(settings.log_level) <= logging.DEBUG:
     app.router.route_class = LoggingRoute
 
 
 @app.on_event("startup")
 async def startup_hook():
```

### Comparing `zeus-ml-0.8.2/zeus/optimizer/perseus/server/scheduler.py` & `zeus_ml-0.9.0/zeus/optimizer/pipeline_frequency/server/scheduler.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,46 +18,46 @@
 
 import copy
 from pathlib import Path
 from contextlib import suppress
 from abc import ABC, abstractmethod
 from typing import Callable, Generator, Sequence, Type
 
-from zeus.optimizer.perseus.common import (
-    PerseusSettings,
+from zeus.optimizer.pipeline_frequency.common import (
+    PFOServerSettings,
     JobInfo,
     RankInfo,
     FrequencySchedule,
     ProfilingResult,
 )
-from zeus.util.logging import get_logger
+from zeus.utils.logging import get_logger
 
 logger = get_logger(__name__)
 
 
 class FrequencyScheduler(ABC):
     """Interface for classes that enclose frequency scheduling policies."""
 
     def __init__(
         self,
         job_info: JobInfo,
         rank_infos: list[RankInfo],
-        perseus_settings: PerseusSettings,
+        pfo_settings: PFOServerSettings,
     ) -> None:
         """Initialize the scheduler.
 
         Args:
             job_info: Info about the training job.
             rank_infos: Info about all ranks. May not be sorted in rank order.
-            perseus_settings: PerseusSettings object.
+            pfo_settings: PFOServerSettings object.
         """
         self.job_info = job_info
         self.rank_infos = sorted(rank_infos, key=lambda info: info.rank)
         self.world_size = self.job_info.world_size
-        self.perseus_settings = perseus_settings
+        self.pfo_settings = pfo_settings
 
         self._generator = self._run()
         self._next_schedule: list[FrequencySchedule] | None = None
 
     def observe(self, profiling_results: list[ProfilingResult]) -> None:
         """Ingest the profiling results for the previous schedule.
 
@@ -134,15 +134,15 @@
     """
 
     class Wrapper(sched_cls):  # type: ignore[valid-type,misc]
         def __init__(
             self,
             job_info: JobInfo,
             rank_infos: list[RankInfo],
-            perseus_settings: PerseusSettings,
+            pfo_settings: PFOServerSettings,
             *args,
             **kwargs,
         ) -> None:
             self._orig_job_info = job_info
             self._orig_rank_infos = rank_infos
 
             # Give the wrapped scheduler a perfect illusion of pure pipeline parallelism
@@ -155,15 +155,15 @@
             new_rank_infos = []
             for rank_info in rank_infos:
                 if rank_info.dp_rank == 0 and rank_info.tp_rank == 0:
                     new_rank_info = copy.deepcopy(rank_info)
                     new_rank_info.rank = rank_info.pp_rank
                     new_rank_infos.append(new_rank_info)
 
-            super().__init__(job_info, rank_infos, perseus_settings, *args, **kwargs)
+            super().__init__(job_info, rank_infos, pfo_settings, *args, **kwargs)
 
         def observe(self, profiling_results: list[ProfilingResult]) -> None:
             """Aggregate results so that each pipeline stage has one result."""
             # Aggregate results from ranks that share the same pp_rank.
             rank_to_pp_rank = {
                 rank_info.rank: rank_info.pp_rank for rank_info in self._orig_rank_infos
             }
@@ -249,26 +249,26 @@
 class PointSolution(FrequencyScheduler):
     """Runs the given frequency schedule."""
 
     def __init__(
         self,
         job_info: JobInfo,
         rank_infos: list[RankInfo],
-        perseus_settings: PerseusSettings,
+        pfo_settings: PFOServerSettings,
         solution_path: str,
     ) -> None:
         """Initialize the scheduler.
 
         Args:
             job_info: Info about the training job.
             rank_infos: Info about all ranks. May not be sorted in rank order.
-            perseus_settings: PerseusSettings object.
+            pfo_settings: PFOServerSettings object.
             solution_path: Path to the frequency Python file generated by lowtime.
         """
-        super().__init__(job_info, rank_infos, perseus_settings)
+        super().__init__(job_info, rank_infos, pfo_settings)
 
         self.solution_path = Path(solution_path)
         if not self.solution_path.is_file():
             raise RuntimeError(f"Solution file not found: {solution_path}")
         if self.solution_path.suffix != ".py":
             raise RuntimeError(f"Solution file is not a Python file: {solution_path}")
```

### Comparing `zeus-ml-0.8.2/zeus/optimizer/power_limit.py` & `zeus_ml-0.9.0/zeus/optimizer/power_limit.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,21 +36,20 @@
 
 from __future__ import annotations
 
 import atexit
 from pathlib import Path
 from abc import ABC, abstractmethod
 
-import pynvml
-
 from zeus.callback import Callback
 from zeus.monitor import ZeusMonitor
-from zeus.util.logging import get_logger
-from zeus.util.metric import zeus_cost
-from zeus.util.pydantic_v1 import BaseModel, PositiveInt, PositiveFloat
+from zeus.utils.logging import get_logger
+from zeus.utils.metric import zeus_cost
+from zeus.utils.pydantic_v1 import BaseModel, PositiveInt, PositiveFloat
+from zeus.device import get_gpus, ZeusGPUNoPermissionError
 
 from typing import TYPE_CHECKING
 
 
 class OptimumSelector(ABC):
     """Base class for optimum power limit selectors."""
 
@@ -80,15 +79,15 @@
         """Select the optimal power limit (W) from measurements."""
         return min(measurements, key=lambda x: x.time).power_limit
 
 
 class ZeusCost(OptimumSelector):
     r"""Selects the power limit that minimizes a linear Zeus time-energy cost function.
 
-    Cost function is $C = \eta \cdot Energy + MaxPower \cdot (1 - \eta) \cdot Time$.
+    Cost function is $\eta \cdot \text{Energy} + (1 - \eta) \cdot \text{MaxPower} \cdot \text{Time}$.
     """
 
     def __init__(self, eta_knob: float, world_size: int = 1) -> None:
         r"""Initialize the selector.
 
         Args:
             eta_knob: The $0 \le \eta \le 1$ knob for the Zeus time-energy cost function.
@@ -267,37 +266,34 @@
         )
 
         # Setup logging.
         self.logger = get_logger(type(self).__name__)
 
         # Set the range of power limits to explore.
         # Assert that supported power limits ranges are uniform across GPUs.
-        pynvml.nvmlInit()
+        gpus = get_gpus(ensure_homogeneous=True)
         pls = []
-        self.handles = []
-        for index in monitor.nvml_gpu_indices:
-            device = pynvml.nvmlDeviceGetHandleByIndex(index)
-            self.handles.append(device)
-            pls.append(pynvml.nvmlDeviceGetPowerManagementLimitConstraints(device))
+        for index in monitor.gpu_indices:
+            pls.append(gpus.getPowerManagementLimitConstraints(index))
         if not all(pls[0] == pl for pl in pls):
             raise ValueError("Power limits ranges are not uniform across GPUs.")
         self.power_limits = list(
             range(pls[0][1], pls[0][0] - self.pl_step, -self.pl_step)
         )
 
         # Turn on persistence mode and set to the highest power limit.
         try:
-            for handle in self.handles:
-                pynvml.nvmlDeviceSetPersistenceMode(handle, pynvml.NVML_FEATURE_ENABLED)
-        except pynvml.NVMLError_NoPermission:  # type: ignore
+            for index in monitor.gpu_indices:
+                gpus.setPersistenceMode(index, enable=True)
+        except ZeusGPUNoPermissionError as ze:
             raise RuntimeError(
                 "SYS_ADMIN capability is required to modify GPU power limits. "
                 "Using --cap-add SYS_ADMIN when running the Docker container "
                 "is the easiest way to do this."
-            ) from None
+            ) from ze
         self.current_power_limit = 0
 
         # Store `Measurement` objects in a list, one for each power limit.
         self.measurements: list[PowerLimitMeasurement] = []
 
         # State for the profiler state machine.
         self.state: Ready | Warmup | Profiling | Done
@@ -442,19 +438,20 @@
 
     def _set_power_limit(self, power_limit: int) -> None:
         """Set the power limit for all GPUs.
 
         Args:
             power_limit: The power limit to set, in milliWatts.
         """
+        gpus = get_gpus()
         self.logger.info("Setting power limit to %d W.", power_limit // 1000)
         if self.current_power_limit == power_limit:
             return
-        for handle in self.handles:
-            pynvml.nvmlDeviceSetPowerManagementLimit(handle, power_limit)
+        for index in self.monitor.gpu_indices:
+            gpus.setPowerManagementLimit(index, power_limit)
         self.current_power_limit = power_limit
 
     def _compute_optimal_power_limit(self) -> int:
         """Compute the optimal power limit in milliWatts."""
         optimal_power_limit = self.optimum_selector.select(self.measurements) * 1000
         self.logger.info("Optimal power limit is %d W.", optimal_power_limit // 1000)
         return optimal_power_limit
@@ -488,15 +485,15 @@
 
     transformers_available = True
 except ModuleNotFoundError:
     transformers_available = False
     TrainerCallback = object  # Fallback base class
 
 
-class HFGlobalPowerLimitOptimizer(TrainerCallback):
+class HFGlobalPowerLimitOptimizer(TrainerCallback):  # type: ignore
     """[Wrapped for Hugging Face Trainer Callback] Optimizer for the power limit knob.
 
     This optimizer uses the JIT profiling log to determine the optimal power limit.
     See [`GlobalPowerLimitOptimizer`][zeus.optimizer.power_limit.GlobalPowerLimitOptimizer]
     for the underlying optimizer implementation.
     """
```

### Comparing `zeus-ml-0.8.2/zeus/policy/__init__.py` & `zeus_ml-0.9.0/zeus/_legacy/policy/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,20 +10,19 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Optimization policies for Zeus.
 
-[`PowerLimitOptimizer`][zeus.policy.interface.PowerLimitOptimizer] and
-[`BatchSizeOptimizer`][zeus.policy.interface.BatchSizeOptimizer] are
+[`PowerLimitOptimizer`][zeus._legacy.policy.interface.PowerLimitOptimizer] and
+[`BatchSizeOptimizer`][zeus._legacy.policy.interface.BatchSizeOptimizer] are
 abstract classes. Users can implement custom policies by extending the
-abstract classes and implementing required method.
-Currently, [`Simulator`][zeus.simulate.Simulator] supports custom policies
-for both classes, while [`ZeusMaster`][zeus.run.ZeusMaster] only supports
-custom [`BatchSizeOptimizer`][zeus.policy.interface.BatchSizeOptimizer]s.
-Custom [`PowerLimitOptimizer`][zeus.policy.PowerLimitOptimizer]s will
-have to be integrated into [`ZeusDataLoader`][zeus.run.ZeusDataLoader].
+abstract classes, implementing required methods, and plugging them into
+the [`Simulator`][zeus._legacy.simulate.Simulator].
 """
 
-from zeus.policy.interface import BatchSizeOptimizer, PowerLimitOptimizer
-from zeus.policy.optimizer import JITPowerLimitOptimizer, PruningGTSBatchSizeOptimizer
+from zeus._legacy.policy.interface import BatchSizeOptimizer, PowerLimitOptimizer
+from zeus._legacy.policy.optimizer import (
+    JITPowerLimitOptimizer,
+    PruningGTSBatchSizeOptimizer,
+)
```

### Comparing `zeus-ml-0.8.2/zeus/policy/interface.py` & `zeus_ml-0.9.0/zeus/_legacy/policy/interface.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,31 +14,31 @@
 
 """Abstract classes for implementing custom optimization policies."""
 
 from __future__ import annotations
 
 from abc import ABC, abstractmethod
 
-from zeus.job import Job
+from zeus._legacy.job import Job
 
 
 class BatchSizeOptimizer(ABC):
     """Finds out the best batch size to use for the job."""
 
     @property
     @abstractmethod
     def name(self) -> str:
         """Name of the batch size optimizer."""
 
     @abstractmethod
     def register_job(self, job: Job, batch_sizes: list[int]) -> None:
         """Prepare internal state so that it can handle the given job.
 
-        It is assumed that the state of each [`Job`][zeus.job.Job] will be
-        managed separately. Note that [`Job`][zeus.job.Job] is hashable,
+        It is assumed that the state of each [`Job`][zeus._legacy.job.Job] will be
+        managed separately. Note that [`Job`][zeus._legacy.job.Job] is hashable,
         and thus can be used as dictionary keys.
 
         Args:
             job: New jobs to register.
             batch_sizes: Batch sizes to consider.
         """
 
@@ -82,19 +82,19 @@
     @abstractmethod
     def predict(self, job: Job, batch_size: int) -> int | None:
         """Return the best power limit for the job and batch size.
 
         Args:
             job: The job to pick the best power limit for.
             batch_size: The batch size chosen by the
-                [`BatchSizeOptimizer`][zeus.policy.BatchSizeOptimizer] for this job.
+                [`BatchSizeOptimizer`][zeus._legacy.policy.BatchSizeOptimizer] for this job.
 
         Returns:
             The best power limit, or `None` if profiling results via
-            [`observe`][zeus.policy.interface.PowerLimitOptimizer.observe] are needed.
+            [`observe`][zeus._legacy.policy.interface.PowerLimitOptimizer.observe] are needed.
         """
 
     @abstractmethod
     def observe(self, job: Job, batch_size: int, power_limit: int, cost: float) -> None:
         """Observe the cost of using the given batch size and power limit for the job.
 
         Args:
```

### Comparing `zeus-ml-0.8.2/zeus/policy/mab.py` & `zeus_ml-0.9.0/zeus/_legacy/policy/mab.py`

 * *Files identical despite different names*

### Comparing `zeus-ml-0.8.2/zeus/policy/optimizer.py` & `zeus_ml-0.9.0/zeus/_legacy/policy/optimizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,29 +10,29 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Implementations of various optimization policies.
 
-[`JITPowerLimitOptimizer`][zeus.policy.optimizer.JITPowerLimitOptimizer] and
-[`PruningGTSBatchSizeOptimizer`][zeus.policy.optimizer.PruningGTSBatchSizeOptimizer]
+[`JITPowerLimitOptimizer`][zeus._legacy.policy.optimizer.JITPowerLimitOptimizer] and
+[`PruningGTSBatchSizeOptimizer`][zeus._legacy.policy.optimizer.PruningGTSBatchSizeOptimizer]
 are the implementations used in Zeus's publication.
 """
 
 from __future__ import annotations
 
 from collections import defaultdict
 from typing import Generator
 
 import numpy as np
 
-from zeus.job import Job
-from zeus.policy.interface import BatchSizeOptimizer, PowerLimitOptimizer
-from zeus.policy.mab import GaussianTS
+from zeus._legacy.job import Job
+from zeus._legacy.policy.interface import BatchSizeOptimizer, PowerLimitOptimizer
+from zeus._legacy.policy.mab import GaussianTS
 
 
 class GTSBatchSizeOptimizer(BatchSizeOptimizer):
     """One Gaussian Thompson Sampling MAB for each job."""
 
     # ruff: noqa: D417
     def __init__(
@@ -43,15 +43,15 @@
         prior_precision: float = 0.0,
         num_exploration: int = 1,
         seed: int = 123456,
         verbose: bool = True,
     ) -> None:
         """Initialze the optimizer.
 
-        Refer to the constructor of [`GaussianTS`][zeus.policy.mab.GaussianTS]
+        Refer to the constructor of [`GaussianTS`][zeus._legacy.policy.mab.GaussianTS]
         for descriptions of other arguments.
 
         Args:
             learn_reward_precision: Whether to learn the reward precision of
                 each arm as we accumulate observations.
         """
         self.learn_reward_precision = learn_reward_precision
@@ -274,15 +274,15 @@
         window_size: int = 0,
         concurrency: bool = False,
         seed: int = 123456,
         verbose: bool = True,
     ) -> None:
         """Initialze the optimizer.
 
-        Refer to the constructor of [`GaussianTS`][zeus.policy.mab.GaussianTS]
+        Refer to the constructor of [`GaussianTS`][zeus._legacy.policy.mab.GaussianTS]
         for descriptions of other arguments.
 
         Args:
             window_size: Size of the window for the MAB (for drift handling).
             concurrency: Whether to support concurrent job submissions.
         """
         self.prior_mean = prior_mean
```

### Comparing `zeus-ml-0.8.2/zeus/simulate.py` & `zeus_ml-0.9.0/zeus/_legacy/simulate.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,18 +19,36 @@
 import operator
 from copy import deepcopy
 from dataclasses import dataclass
 
 import numpy as np
 import pandas as pd
 
-from zeus.analyze import HistoryEntry
-from zeus.job import Job
-from zeus.policy import BatchSizeOptimizer, PowerLimitOptimizer
-from zeus.util import zeus_cost
+from zeus._legacy.job import Job
+from zeus._legacy.policy import BatchSizeOptimizer, PowerLimitOptimizer
+from zeus.utils.metric import zeus_cost
+
+
+@dataclass
+class HistoryEntry:
+    """Represents the config and result of a job run that may have failed.
+
+    Attributes:
+        bs: Batch size
+        pl: Power limit
+        energy: Energy consumption in Joules
+        reached: Whether the target metric was reached at the end
+        time: Time consumption in seconds
+    """
+
+    bs: int
+    pl: int
+    energy: float
+    reached: bool
+    time: float
 
 
 # ruff: noqa: PLR0912, PLR0915
 class Simulator:
     """Simulates job execution optimized by Zeus."""
 
     def __init__(
@@ -97,15 +115,15 @@
             num_recurrence: How many times the job recurs.
             beta_knob: `beta_knob * min_eta` is the early stopping cost threshold.
                 Set to `np.inf` to disable early stopping.
             eta_knob: $\eta$ used in the hybrid cost metric.
                 $\textrm{cost} = \eta \cdot \textrm{ETA} + (1 - \eta) \cdot \textrm{MaxPower} \cdot \textrm{TTA}$
 
         Returns:
-            A list of [`HistoryEntry`][zeus.analyze.HistoryEntry] objects for each job run.
+            A list of [`HistoryEntry`][zeus._legacy.simulate.HistoryEntry] objects for each job run.
         """
         # Copy all internal state so that simulation does not modify any
         # internal state and is deterministic w.r.t. the random seed.
         bso = deepcopy(self.bso)
         plo = deepcopy(self.plo)
         rng = np.random.default_rng(self.seed)
 
@@ -244,15 +262,15 @@
                     job runtime differences.
             beta_knob: `beta_knob * min_eta` is the early stopping cost threshold.
                 Set to `np.inf` to disable early stopping.
             eta_knob: $\eta$ used in the hybrid cost metric.
                 $\textrm{cost} = \eta \cdot \textrm{ETA} + (1 - \eta) \cdot \textrm{MaxPower} \cdot \textrm{TTA}$
 
         Returns:
-            A list of [`HistoryEntry`][zeus.analyze.HistoryEntry] objects for each job run.
+            A list of [`HistoryEntry`][zeus._legacy.simulate.HistoryEntry] objects for each job run.
         """
         # Copy all internal state so that simulation does not modify any
         # internal state and is deterministic w.r.t. the random seed.
         bso = deepcopy(self.bso)
         plo = deepcopy(self.plo)
         rng = np.random.default_rng(self.seed)
 
@@ -737,20 +755,20 @@
             if profile_power:
                 # Note that power_df holds rows with all power limits. Evenly splitting the
                 # epochs with the number of samples and running each slice with each power
                 # limit consumes (1/N) * e_100 + (1/N) * e_125 + ... + (1/N) * e_250.
                 # Also there are all runs 1, 2, ... included, but power info is actually
                 # completely duplicated across different runs in the DataFrame.
                 # Thus, taking the mean across the entire power_df gets us what we want.
-                energy_first_epoch = power_df.energy_per_epoch.mean().item()
+                energy_first_epoch = power_df.energy_per_epoch.mean().item()  # type: ignore
                 energy_from_second_epoch = path.energy_per_epoch.item() * (
                     num_epochs - 1
                 )
                 energy_consumption = energy_first_epoch + energy_from_second_epoch
-                time_first_epoch = power_df.time_per_epoch.mean().item()
+                time_first_epoch = power_df.time_per_epoch.mean().item()  # type: ignore
                 time_from_second_epoch = path.time_per_epoch.item() * (num_epochs - 1)
                 time_consumption = time_first_epoch + time_from_second_epoch
             # Just run num_epochs with the given power limit. Simple.
             else:
                 energy_consumption = path.energy_per_epoch.item() * num_epochs
                 time_consumption = path.time_per_epoch.item() * num_epochs
             return energy_consumption, time_consumption
```

### Comparing `zeus-ml-0.8.2/zeus/util/__init__.py` & `zeus_ml-0.9.0/zeus/optimizer/pipeline_frequency/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -8,13 +8,17 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""Utility functions and classes."""
+"""Optimize the energy consumption of large model training with Perseus.
 
-from zeus.util.env import get_env
-from zeus.util.logging import FileAndConsole
-from zeus.util.lr_scaler import LinearScaler, SquareRootScaler
-from zeus.util.metric import zeus_cost, ZeusCostThresholdExceededError
+A a high-level, this optimizer assigns each forward and backward computation
+in a pipeline parallel training iteration with a GPU frequency that leads to
+a Pareto-optimal training iteration time and energy consumption.
+
+Currently, this optimizer depends on PyTorch.
+"""
+
+from zeus.optimizer.pipeline_frequency.optimizer import PipelineFrequencyOptimizer
```

### Comparing `zeus-ml-0.8.2/zeus/util/async_utils.py` & `zeus_ml-0.9.0/zeus/utils/async_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from __future__ import annotations
 
 import asyncio
 import logging
 import functools
 from typing import Any, Coroutine, TypeVar
 
-from zeus.util.logging import get_logger
+from zeus.utils.logging import get_logger
 
 T = TypeVar("T")
 default_logger = get_logger(__name__)
 
 
 def create_task(
     coroutine: Coroutine[Any, Any, T],
@@ -34,15 +34,15 @@
     """Create an `asyncio.Task` but ensure that exceptions are logged.
 
     Reference: https://quantlane.com/blog/ensure-asyncio-task-exceptions-get-logged/
 
     Args:
         coroutine: The coroutine to be wrapped.
         logger: The logger to be used for logging exceptions. If `None`, the
-            the logger with the name `zeus.util.async_utils` is used.
+            the logger with the name `zeus.utils.async_utils` is used.
     """
     loop = asyncio.get_running_loop()
     task = loop.create_task(coroutine)
     task.add_done_callback(
         functools.partial(_handle_task_exception, logger=logger or default_logger)
     )
     return task
```

### Comparing `zeus-ml-0.8.2/zeus/util/framework.py` & `zeus_ml-0.9.0/zeus/utils/framework.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 """Utilities for framework-specific code."""
 
 from __future__ import annotations
 
 import types
 from functools import lru_cache
 
-from zeus.util.logging import get_logger
+from zeus.utils.logging import get_logger
 
 logger = get_logger(name=__name__)
 MODULE_CACHE: dict[str, types.ModuleType] = {}
 
 
 @lru_cache(maxsize=1)
 def torch_is_available():
```

### Comparing `zeus-ml-0.8.2/zeus/util/logging.py` & `zeus_ml-0.9.0/zeus/utils/logging.py`

 * *Files identical despite different names*

### Comparing `zeus-ml-0.8.2/zeus/util/lr_scaler.py` & `zeus_ml-0.9.0/zeus/utils/lr_scaler.py`

 * *Files identical despite different names*

### Comparing `zeus-ml-0.8.2/zeus/util/pydantic_v1.py` & `zeus_ml-0.9.0/zeus/utils/pydantic_v1.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,18 +11,20 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Compatibility layer for Pydantic v1 and v2.
 
 We don't want to pin any specific version of Pydantic. With this, we can
-import things from `zeus.util.pydantic_v1` and always use the V1 API
+import things from `zeus.utils.pydantic_v1` and always use the V1 API
 regardless of the installed version of Pydantic.
 
 Inspired by Deepspeed:
 https://github.com/microsoft/DeepSpeed/blob/5d754606/deepspeed/pydantic_v1.py
 """
 
+# pyright: reportWildcardImportFromLibrary=false
+
 try:
     from pydantic.v1 import *
 except ImportError:
     from pydantic import *
```

### Comparing `zeus-ml-0.8.2/zeus/util/testing.py` & `zeus_ml-0.9.0/zeus/utils/testing.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,16 +15,16 @@
 """Utilities for testing."""
 
 from __future__ import annotations
 
 from pathlib import Path
 
 from zeus.monitor import Measurement, ZeusMonitor
-from zeus.util.framework import cuda_sync
-from zeus.util.logging import get_logger
+from zeus.utils.framework import cuda_sync
+from zeus.utils.logging import get_logger
 
 
 class ReplayZeusMonitor(ZeusMonitor):
     """A mock ZeusMonitor that replays windows recorded by a real monitor.
 
     This class is for testing only. Based on a CSV log file that records the time
     and energy measurements of `ZeusMonitor` measurement windows, users can drop-in
@@ -41,38 +41,38 @@
     Attributes:
         gpu_indices (`list[int]`): Indices of all the CUDA devices to monitor.
     """
 
     def __init__(
         self,
         gpu_indices: list[int] | None = None,
-        monitor_exec: str = "zeus_monitor",
+        approx_instant_energy: bool = False,
         log_file: str | Path | None = None,
         ignore_sync_cuda: bool = False,
         match_window_name: bool = True,
     ) -> None:
         """Initialize the replay monitor.
 
         The log file should be a CSV file with the following header (e.g. gpu_indices=[0, 2]):
         `start_time,window_name,elapsed_time,gpu0_energy,gpu2_energy`
 
         Args:
             gpu_indices: Indices of all the CUDA devices to monitor. This should be consistent
                 with the indices used in the log file. If `None`, GPU indices will be inferred
                 from the log file header. Does not respect `CUDA_VISIBLE_DEVICES`.
                 (Default: `None`)
-            monitor_exec: Zeus monitor executable. Not used. (Default: `"zeus_monitor"`)
+            approx_instant_energy: Whether to approximate the instant energy consumption. Not used.
             log_file: Path to the log CSV file to replay events from. `None` is not allowed.
             ignore_sync_cuda: Whether to ignore `sync_cuda` calls. (Default: `False`)
             match_window_name: Whether to make sure window names match. (Default: `True`)
         """
         if log_file is None:
             raise ValueError("`log_file` cannot be `None` for `ReplayZeusMonitor`.")
 
-        self.monitor_exec = monitor_exec
+        self.approx_instant_energy = approx_instant_energy
         self.log_file = open(log_file)
         self.ignore_sync_cuda = ignore_sync_cuda
         self.match_window_name = match_window_name
 
         # Infer GPU indices from the log file if not provided.
         header = self.log_file.readline()
         if gpu_indices is None:
```

