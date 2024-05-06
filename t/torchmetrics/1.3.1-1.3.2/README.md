# Comparing `tmp/torchmetrics-1.3.1.tar.gz` & `tmp/torchmetrics-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torchmetrics-1.3.1.tar", last modified: Mon Feb 12 19:11:08 2024, max compression
+gzip compressed data, was "torchmetrics-1.3.2.tar", last modified: Mon Mar 18 12:39:34 2024, max compression
```

## Comparing `torchmetrics-1.3.1.tar` & `torchmetrics-1.3.2.tar`

### file list

```diff
@@ -1,374 +1,374 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 19:11:08.530630 torchmetrics-1.3.1/
--rw-r--r--   0 runner    (1001) docker     (127)    72918 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     2575 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (127)    11352 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      932 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    19943 2024-02-12 19:11:08.530630 torchmetrics-1.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12724 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 19:11:08.466630 torchmetrics-1.3.1/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)      368 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/requirements/_devel.txt
--rw-r--r--   0 runner    (1001) docker     (127)      546 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/requirements/_docs.txt
--rw-r--r--   0 runner    (1001) docker     (127)      343 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/requirements/_doctest.txt
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/requirements/_integrate.txt
--rw-r--r--   0 runner    (1001) docker     (127)      521 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/requirements/_tests.txt
--rw-r--r--   0 runner    (1001) docker     (127)      487 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/requirements/audio.txt
--rw-r--r--   0 runner    (1001) docker     (127)      513 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/requirements/audio_test.txt
--rw-r--r--   0 runner    (1001) docker     (127)      406 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/requirements/base.txt
--rw-r--r--   0 runner    (1001) docker     (127)      358 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/requirements/classification_test.txt
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/requirements/detection.txt
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/requirements/detection_test.txt
--rw-r--r--   0 runner    (1001) docker     (127)      390 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/requirements/image.txt
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/requirements/image_test.txt
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/requirements/multimodal.txt
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/requirements/nominal_test.txt
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/requirements/segmentation_test.txt
--rw-r--r--   0 runner    (1001) docker     (127)      494 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/requirements/text.txt
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/requirements/text_test.txt
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/requirements/typing.txt
--rw-r--r--   0 runner    (1001) docker     (127)      306 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/requirements/visual.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-12 19:11:08.530630 torchmetrics-1.3.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)    10931 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 19:11:08.458630 torchmetrics-1.3.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 19:11:08.470630 torchmetrics-1.3.1/src/torchmetrics/
--rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/__about__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8870 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    27283 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/aggregation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 19:11:08.470630 torchmetrics-1.3.1/src/torchmetrics/audio/
--rw-r--r--   0 runner    (1001) docker     (127)     1916 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/audio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4132 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/audio/_deprecated.py
--rw-r--r--   0 runner    (1001) docker     (127)     7340 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/audio/pesq.py
--rw-r--r--   0 runner    (1001) docker     (127)     6932 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/audio/pit.py
--rw-r--r--   0 runner    (1001) docker     (127)    15368 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/audio/sdr.py
--rw-r--r--   0 runner    (1001) docker     (127)    12748 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/audio/snr.py
--rw-r--r--   0 runner    (1001) docker     (127)     7474 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/audio/srmr.py
--rw-r--r--   0 runner    (1001) docker     (127)     6512 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/audio/stoi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 19:11:08.478630 torchmetrics-1.3.1/src/torchmetrics/classification/
--rw-r--r--   0 runner    (1001) docker     (127)     6454 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/classification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23317 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/classification/accuracy.py
--rw-r--r--   0 runner    (1001) docker     (127)    25539 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/classification/auroc.py
--rw-r--r--   0 runner    (1001) docker     (127)    25401 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/classification/average_precision.py
--rw-r--r--   0 runner    (1001) docker     (127)     1234 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/classification/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    17266 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/classification/calibration_error.py
--rw-r--r--   0 runner    (1001) docker     (127)    13691 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/classification/cohen_kappa.py
--rw-r--r--   0 runner    (1001) docker     (127)    23218 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/classification/confusion_matrix.py
--rw-r--r--   0 runner    (1001) docker     (127)    12441 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/classification/dice.py
--rw-r--r--   0 runner    (1001) docker     (127)    18421 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/classification/exact_match.py
--rw-r--r--   0 runner    (1001) docker     (127)    51767 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/classification/f_beta.py
--rw-r--r--   0 runner    (1001) docker     (127)    13841 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/classification/group_fairness.py
--rw-r--r--   0 runner    (1001) docker     (127)    24033 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/classification/hamming.py
--rw-r--r--   0 runner    (1001) docker     (127)    15807 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/classification/hinge.py
--rw-r--r--   0 runner    (1001) docker     (127)    19847 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/classification/jaccard.py
--rw-r--r--   0 runner    (1001) docker     (127)    17066 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/classification/matthews_corrcoef.py
--rw-r--r--   0 runner    (1001) docker     (127)    25336 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/classification/precision_fixed_recall.py
--rw-r--r--   0 runner    (1001) docker     (127)    46450 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/classification/precision_recall.py
--rw-r--r--   0 runner    (1001) docker     (127)    34599 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/classification/precision_recall_curve.py
--rw-r--r--   0 runner    (1001) docker     (127)    16435 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/classification/ranking.py
--rw-r--r--   0 runner    (1001) docker     (127)    25320 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/classification/recall_fixed_precision.py
--rw-r--r--   0 runner    (1001) docker     (127)    29763 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/classification/roc.py
--rw-r--r--   0 runner    (1001) docker     (127)    23594 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/classification/specificity.py
--rw-r--r--   0 runner    (1001) docker     (127)    18825 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/classification/specificity_sensitivity.py
--rw-r--r--   0 runner    (1001) docker     (127)    25335 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/classification/stat_scores.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 19:11:08.478630 torchmetrics-1.3.1/src/torchmetrics/clustering/
--rw-r--r--   0 runner    (1001) docker     (127)     1702 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/clustering/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5386 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/clustering/adjusted_mutual_info_score.py
--rw-r--r--   0 runner    (1001) docker     (127)     5163 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/clustering/adjusted_rand_score.py
--rw-r--r--   0 runner    (1001) docker     (127)     5365 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/clustering/calinski_harabasz_score.py
--rw-r--r--   0 runner    (1001) docker     (127)     5481 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/clustering/davies_bouldin_score.py
--rw-r--r--   0 runner    (1001) docker     (127)     4986 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/clustering/dunn_index.py
--rw-r--r--   0 runner    (1001) docker     (127)     4616 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/clustering/fowlkes_mallows_index.py
--rw-r--r--   0 runner    (1001) docker     (127)    12941 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/clustering/homogeneity_completeness_v_measure.py
--rw-r--r--   0 runner    (1001) docker     (127)     5041 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/clustering/mutual_info_score.py
--rw-r--r--   0 runner    (1001) docker     (127)     5279 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/clustering/normalized_mutual_info_score.py
--rw-r--r--   0 runner    (1001) docker     (127)     4882 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/clustering/rand_score.py
--rw-r--r--   0 runner    (1001) docker     (127)    30413 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/collections.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 19:11:08.482630 torchmetrics-1.3.1/src/torchmetrics/detection/
--rw-r--r--   0 runner    (1001) docker     (127)     1467 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/detection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2332 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/detection/_deprecated.py
--rw-r--r--   0 runner    (1001) docker     (127)    42493 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/detection/_mean_ap.py
--rw-r--r--   0 runner    (1001) docker     (127)     8234 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/detection/ciou.py
--rw-r--r--   0 runner    (1001) docker     (127)     8191 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/detection/diou.py
--rw-r--r--   0 runner    (1001) docker     (127)     7887 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/detection/giou.py
--rw-r--r--   0 runner    (1001) docker     (127)     4593 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/detection/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    12111 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/detection/iou.py
--rw-r--r--   0 runner    (1001) docker     (127)    50362 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/detection/mean_ap.py
--rw-r--r--   0 runner    (1001) docker     (127)    17536 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/detection/panoptic_qualities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 19:11:08.482630 torchmetrics-1.3.1/src/torchmetrics/functional/
--rw-r--r--   0 runner    (1001) docker     (127)     9439 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/functional/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 19:11:08.482630 torchmetrics-1.3.1/src/torchmetrics/functional/audio/
--rw-r--r--   0 runner    (1001) docker     (127)     2084 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/functional/audio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4483 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/functional/audio/_deprecated.py
--rw-r--r--   0 runner    (1001) docker     (127)     4832 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/functional/audio/pesq.py
--rw-r--r--   0 runner    (1001) docker     (127)     9867 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/functional/audio/pit.py
--rw-r--r--   0 runner    (1001) docker     (127)    12031 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/functional/audio/sdr.py
--rw-r--r--   0 runner    (1001) docker     (127)     5039 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/functional/audio/snr.py
--rw-r--r--   0 runner    (1001) docker     (127)    14302 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/functional/audio/srmr.py
--rw-r--r--   0 runner    (1001) docker     (127)     4241 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/functional/audio/stoi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 19:11:08.486630 torchmetrics-1.3.1/src/torchmetrics/functional/classification/
--rw-r--r--   0 runner    (1001) docker     (127)     7106 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/functional/classification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19927 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/functional/classification/accuracy.py
--rw-r--r--   0 runner    (1001) docker     (127)    23659 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/functional/classification/auroc.py
--rw-r--r--   0 runner    (1001) docker     (127)    23230 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/functional/classification/average_precision.py
--rw-r--r--   0 runner    (1001) docker     (127)    16940 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/functional/classification/calibration_error.py
--rw-r--r--   0 runner    (1001) docker     (127)    11633 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/functional/classification/cohen_kappa.py
--rw-r--r--   0 runner    (1001) docker     (127)    28064 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/functional/classification/confusion_matrix.py
--rw-r--r--   0 runner    (1001) docker     (127)     9362 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/functional/classification/dice.py
--rw-r--r--   0 runner    (1001) docker     (127)    11784 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/functional/classification/exact_match.py
--rw-r--r--   0 runner    (1001) docker     (127)    35850 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/functional/classification/f_beta.py
--rw-r--r--   0 runner    (1001) docker     (127)    16888 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/functional/classification/group_fairness.py
--rw-r--r--   0 runner    (1001) docker     (127)    20724 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/functional/classification/hamming.py
--rw-r--r--   0 runner    (1001) docker     (127)    12369 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/functional/classification/hinge.py
--rw-r--r--   0 runner    (1001) docker     (127)    16670 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/functional/classification/jaccard.py
--rw-r--r--   0 runner    (1001) docker     (127)    12395 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/functional/classification/matthews_corrcoef.py
--rw-r--r--   0 runner    (1001) docker     (127)    18072 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/functional/classification/precision_fixed_recall.py
--rw-r--r--   0 runner    (1001) docker     (127)    35234 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/functional/classification/precision_recall.py
--rw-r--r--   0 runner    (1001) docker     (127)    47018 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/functional/classification/precision_recall_curve.py
--rw-r--r--   0 runner    (1001) docker     (127)    11402 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/functional/classification/ranking.py
--rw-r--r--   0 runner    (1001) docker     (127)    21930 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/functional/classification/recall_fixed_precision.py
--rw-r--r--   0 runner    (1001) docker     (127)    28564 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/functional/classification/roc.py
--rw-r--r--   0 runner    (1001) docker     (127)    18560 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/functional/classification/specificity.py
--rw-r--r--   0 runner    (1001) docker     (127)    23561 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/functional/classification/specificity_sensitivity.py
--rw-r--r--   0 runner    (1001) docker     (127)    49635 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/functional/classification/stat_scores.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 19:11:08.486630 torchmetrics-1.3.1/src/torchmetrics/functional/clustering/
--rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/functional/clustering/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4470 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/functional/clustering/adjusted_mutual_info_score.py
--rw-r--r--   0 runner    (1001) docker     (127)     2422 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/functional/clustering/adjusted_rand_score.py
--rw-r--r--   0 runner    (1001) docker     (127)     2462 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/functional/clustering/calinski_harabasz_score.py
--rw-r--r--   0 runner    (1001) docker     (127)     2625 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/functional/clustering/davies_bouldin_score.py
--rw-r--r--   0 runner    (1001) docker     (127)     2789 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/functional/clustering/dunn_index.py
--rw-r--r--   0 runner    (1001) docker     (127)     2502 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/functional/clustering/fowlkes_mallows_index.py
--rw-r--r--   0 runner    (1001) docker     (127)     4399 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/functional/clustering/homogeneity_completeness_v_measure.py
--rw-r--r--   0 runner    (1001) docker     (127)     2616 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/functional/clustering/mutual_info_score.py
--rw-r--r--   0 runner    (1001) docker     (127)     2104 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/functional/clustering/normalized_mutual_info_score.py
--rw-r--r--   0 runner    (1001) docker     (127)     2602 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/functional/clustering/rand_score.py
--rw-r--r--   0 runner    (1001) docker     (127)    10123 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/functional/clustering/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 19:11:08.486630 torchmetrics-1.3.1/src/torchmetrics/functional/detection/
--rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/functional/detection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/functional/detection/_deprecated.py
--rw-r--r--   0 runner    (1001) docker     (127)    19799 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/functional/detection/_panoptic_quality_common.py
--rw-r--r--   0 runner    (1001) docker     (127)     4422 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/functional/detection/ciou.py
--rw-r--r--   0 runner    (1001) docker     (127)     4424 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/functional/detection/diou.py
--rw-r--r--   0 runner    (1001) docker     (127)     4423 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/functional/detection/giou.py
--rw-r--r--   0 runner    (1001) docker     (127)     4263 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/functional/detection/iou.py
--rw-r--r--   0 runner    (1001) docker     (127)     7896 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/functional/detection/panoptic_qualities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 19:11:08.490630 torchmetrics-1.3.1/src/torchmetrics/functional/image/
--rw-r--r--   0 runner    (1001) docker     (127)     2572 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/functional/image/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9322 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/functional/image/_deprecated.py
--rw-r--r--   0 runner    (1001) docker     (127)     5678 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/functional/image/d_lambda.py
--rw-r--r--   0 runner    (1001) docker     (127)    11145 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/functional/image/d_s.py
--rw-r--r--   0 runner    (1001) docker     (127)     4560 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/functional/image/ergas.py
--rw-r--r--   0 runner    (1001) docker     (127)     2900 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/functional/image/gradients.py
--rw-r--r--   0 runner    (1001) docker     (127)     5993 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/functional/image/helper.py
--rw-r--r--   0 runner    (1001) docker     (127)    16772 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/functional/image/lpips.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 19:11:08.490630 torchmetrics-1.3.1/src/torchmetrics/functional/image/lpips_models/
--rw-r--r--   0 runner    (1001) docker     (127)     6009 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/functional/image/lpips_models/alex.pth
--rw-r--r--   0 runner    (1001) docker     (127)    10811 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/functional/image/lpips_models/squeeze.pth
--rw-r--r--   0 runner    (1001) docker     (127)     7289 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/functional/image/lpips_models/vgg.pth
--rw-r--r--   0 runner    (1001) docker     (127)    13786 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/functional/image/perceptual_path_length.py
--rw-r--r--   0 runner    (1001) docker     (127)     5979 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/functional/image/psnr.py
--rw-r--r--   0 runner    (1001) docker     (127)     4527 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/functional/image/psnrb.py
--rw-r--r--   0 runner    (1001) docker     (127)     4018 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/functional/image/rase.py
--rw-r--r--   0 runner    (1001) docker     (127)     5518 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/functional/image/rmse_sw.py
--rw-r--r--   0 runner    (1001) docker     (127)     4331 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/functional/image/sam.py
--rw-r--r--   0 runner    (1001) docker     (127)     8698 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/functional/image/scc.py
--rw-r--r--   0 runner    (1001) docker     (127)    21528 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/functional/image/ssim.py
--rw-r--r--   0 runner    (1001) docker     (127)     2840 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/functional/image/tv.py
--rw-r--r--   0 runner    (1001) docker     (127)     6430 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/functional/image/uqi.py
--rw-r--r--   0 runner    (1001) docker     (127)     4795 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/functional/image/vif.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 19:11:08.490630 torchmetrics-1.3.1/src/torchmetrics/functional/multimodal/
--rw-r--r--   0 runner    (1001) docker     (127)      918 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/functional/multimodal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15552 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/functional/multimodal/clip_iqa.py
--rw-r--r--   0 runner    (1001) docker     (127)     7062 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/functional/multimodal/clip_score.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 19:11:08.494630 torchmetrics-1.3.1/src/torchmetrics/functional/nominal/
--rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/functional/nominal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7351 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/functional/nominal/cramers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4290 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/functional/nominal/fleiss_kappa.py
--rw-r--r--   0 runner    (1001) docker     (127)     6886 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/functional/nominal/pearson.py
--rw-r--r--   0 runner    (1001) docker     (127)     7125 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/functional/nominal/theils_u.py
--rw-r--r--   0 runner    (1001) docker     (127)     7650 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/functional/nominal/tschuprows.py
--rw-r--r--   0 runner    (1001) docker     (127)     5756 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/functional/nominal/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 19:11:08.494630 torchmetrics-1.3.1/src/torchmetrics/functional/pairwise/
--rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/functional/pairwise/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3499 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/functional/pairwise/cosine.py
--rw-r--r--   0 runner    (1001) docker     (127)     3449 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/functional/pairwise/euclidean.py
--rw-r--r--   0 runner    (1001) docker     (127)     2253 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/functional/pairwise/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3176 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/functional/pairwise/linear.py
--rw-r--r--   0 runner    (1001) docker     (127)     3196 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/functional/pairwise/manhattan.py
--rw-r--r--   0 runner    (1001) docker     (127)     3999 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/functional/pairwise/minkowski.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 19:11:08.494630 torchmetrics-1.3.1/src/torchmetrics/functional/regression/
--rw-r--r--   0 runner    (1001) docker     (127)     2664 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/functional/regression/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2878 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/functional/regression/concordance.py
--rw-r--r--   0 runner    (1001) docker     (127)     3635 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/functional/regression/cosine_similarity.py
--rw-r--r--   0 runner    (1001) docker     (127)     4862 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/functional/regression/csi.py
--rw-r--r--   0 runner    (1001) docker     (127)     5472 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/functional/regression/explained_variance.py
--rw-r--r--   0 runner    (1001) docker     (127)    15173 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/functional/regression/kendall.py
--rw-r--r--   0 runner    (1001) docker     (127)     4399 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/functional/regression/kl_divergence.py
--rw-r--r--   0 runner    (1001) docker     (127)     3525 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/functional/regression/log_cosh.py
--rw-r--r--   0 runner    (1001) docker     (127)     2599 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/functional/regression/log_mse.py
--rw-r--r--   0 runner    (1001) docker     (127)     2561 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/functional/regression/mae.py
--rw-r--r--   0 runner    (1001) docker     (127)     3030 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/functional/regression/mape.py
--rw-r--r--   0 runner    (1001) docker     (127)     3010 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/functional/regression/minkowski.py
--rw-r--r--   0 runner    (1001) docker     (127)     2900 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/functional/regression/mse.py
--rw-r--r--   0 runner    (1001) docker     (127)     5274 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/functional/regression/pearson.py
--rw-r--r--   0 runner    (1001) docker     (127)     6639 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/functional/regression/r2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2945 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/functional/regression/rse.py
--rw-r--r--   0 runner    (1001) docker     (127)     5142 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/functional/regression/spearman.py
--rw-r--r--   0 runner    (1001) docker     (127)     3305 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/functional/regression/symmetric_mape.py
--rw-r--r--   0 runner    (1001) docker     (127)     6096 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/functional/regression/tweedie_deviance.py
--rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/functional/regression/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2679 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/functional/regression/wmape.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 19:11:08.498630 torchmetrics-1.3.1/src/torchmetrics/functional/retrieval/
--rw-r--r--   0 runner    (1001) docker     (127)     1688 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/functional/retrieval/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5417 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/functional/retrieval/_deprecated.py
--rw-r--r--   0 runner    (1001) docker     (127)     2663 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/functional/retrieval/auroc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2605 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/functional/retrieval/average_precision.py
--rw-r--r--   0 runner    (1001) docker     (127)     2671 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/functional/retrieval/fall_out.py
--rw-r--r--   0 runner    (1001) docker     (127)     2409 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/functional/retrieval/hit_rate.py
--rw-r--r--   0 runner    (1001) docker     (127)     4328 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/functional/retrieval/ndcg.py
--rw-r--r--   0 runner    (1001) docker     (127)     2745 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/functional/retrieval/precision.py
--rw-r--r--   0 runner    (1001) docker     (127)     4044 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/functional/retrieval/precision_recall_curve.py
--rw-r--r--   0 runner    (1001) docker     (127)     2121 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/functional/retrieval/r_precision.py
--rw-r--r--   0 runner    (1001) docker     (127)     2504 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/functional/retrieval/recall.py
--rw-r--r--   0 runner    (1001) docker     (127)     2447 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/functional/retrieval/reciprocal_rank.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 19:11:08.498630 torchmetrics-1.3.1/src/torchmetrics/functional/segmentation/
--rw-r--r--   0 runner    (1001) docker     (127)      578 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/functional/segmentation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    44776 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/functional/segmentation/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 19:11:08.502630 torchmetrics-1.3.1/src/torchmetrics/functional/text/
--rw-r--r--   0 runner    (1001) docker     (127)     2067 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/functional/text/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14008 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/functional/text/_deprecated.py
--rw-r--r--   0 runner    (1001) docker     (127)    21062 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/functional/text/bert.py
--rw-r--r--   0 runner    (1001) docker     (127)     7578 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/functional/text/bleu.py
--rw-r--r--   0 runner    (1001) docker     (127)     2983 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/functional/text/cer.py
--rw-r--r--   0 runner    (1001) docker     (127)    26044 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/functional/text/chrf.py
--rw-r--r--   0 runner    (1001) docker     (127)     4771 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/functional/text/edit.py
--rw-r--r--   0 runner    (1001) docker     (127)    17547 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/functional/text/eed.py
--rw-r--r--   0 runner    (1001) docker     (127)    16996 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/functional/text/helper.py
--rw-r--r--   0 runner    (1001) docker     (127)    11874 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/functional/text/helper_embedding_metric.py
--rw-r--r--   0 runner    (1001) docker     (127)    28013 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/functional/text/infolm.py
--rw-r--r--   0 runner    (1001) docker     (127)     3031 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/functional/text/mer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5374 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/functional/text/perplexity.py
--rw-r--r--   0 runner    (1001) docker     (127)    21903 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/functional/text/rouge.py
--rw-r--r--   0 runner    (1001) docker     (127)    19053 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/functional/text/sacre_bleu.py
--rw-r--r--   0 runner    (1001) docker     (127)     9888 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/functional/text/squad.py
--rw-r--r--   0 runner    (1001) docker     (127)    23307 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/functional/text/ter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2974 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/functional/text/wer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3509 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/functional/text/wil.py
--rw-r--r--   0 runner    (1001) docker     (127)     3513 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/functional/text/wip.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 19:11:08.502630 torchmetrics-1.3.1/src/torchmetrics/image/
--rw-r--r--   0 runner    (1001) docker     (127)     2828 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/image/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8770 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/image/_deprecated.py
--rw-r--r--   0 runner    (1001) docker     (127)     6107 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/image/d_lambda.py
--rw-r--r--   0 runner    (1001) docker     (127)     8784 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/image/d_s.py
--rw-r--r--   0 runner    (1001) docker     (127)     5806 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/image/ergas.py
--rw-r--r--   0 runner    (1001) docker     (127)    19261 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/image/fid.py
--rw-r--r--   0 runner    (1001) docker     (127)     9092 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/image/inception.py
--rw-r--r--   0 runner    (1001) docker     (127)    14539 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/image/kid.py
--rw-r--r--   0 runner    (1001) docker     (127)     8075 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/image/lpip.py
--rw-r--r--   0 runner    (1001) docker     (127)    12651 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/image/mifid.py
--rw-r--r--   0 runner    (1001) docker     (127)     8730 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/image/perceptual_path_length.py
--rw-r--r--   0 runner    (1001) docker     (127)     8500 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/image/psnr.py
--rw-r--r--   0 runner    (1001) docker     (127)     5623 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/image/psnrb.py
--rw-r--r--   0 runner    (1001) docker     (127)     5077 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/image/rase.py
--rw-r--r--   0 runner    (1001) docker     (127)     5421 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/image/rmse_sw.py
--rw-r--r--   0 runner    (1001) docker     (127)     6823 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/image/sam.py
--rw-r--r--   0 runner    (1001) docker     (127)     3295 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/image/scc.py
--rw-r--r--   0 runner    (1001) docker     (127)    17181 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/image/ssim.py
--rw-r--r--   0 runner    (1001) docker     (127)     5307 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/image/tv.py
--rw-r--r--   0 runner    (1001) docker     (127)     6816 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/image/uqi.py
--rw-r--r--   0 runner    (1001) docker     (127)     3207 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/image/vif.py
--rw-r--r--   0 runner    (1001) docker     (127)    52001 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/metric.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 19:11:08.502630 torchmetrics-1.3.1/src/torchmetrics/multimodal/
--rw-r--r--   0 runner    (1001) docker     (127)      888 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/multimodal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11620 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/multimodal/clip_iqa.py
--rw-r--r--   0 runner    (1001) docker     (127)     7460 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/multimodal/clip_score.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 19:11:08.506630 torchmetrics-1.3.1/src/torchmetrics/nominal/
--rw-r--r--   0 runner    (1001) docker     (127)      986 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/nominal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6253 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/nominal/cramers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5701 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/nominal/fleiss_kappa.py
--rw-r--r--   0 runner    (1001) docker     (127)     6548 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/nominal/pearson.py
--rw-r--r--   0 runner    (1001) docker     (127)     5783 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/nominal/theils_u.py
--rw-r--r--   0 runner    (1001) docker     (127)     6319 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/nominal/tschuprows.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 19:11:08.506630 torchmetrics-1.3.1/src/torchmetrics/regression/
--rw-r--r--   0 runner    (1001) docker     (127)     2345 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/regression/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5419 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/regression/concordance.py
--rw-r--r--   0 runner    (1001) docker     (127)     5207 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/regression/cosine_similarity.py
--rw-r--r--   0 runner    (1001) docker     (127)     4821 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/regression/csi.py
--rw-r--r--   0 runner    (1001) docker     (127)     6920 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/regression/explained_variance.py
--rw-r--r--   0 runner    (1001) docker     (127)     8186 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/regression/kendall.py
--rw-r--r--   0 runner    (1001) docker     (127)     6453 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/regression/kl_divergence.py
--rw-r--r--   0 runner    (1001) docker     (127)     5413 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/regression/log_cosh.py
--rw-r--r--   0 runner    (1001) docker     (127)     4686 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/regression/log_mse.py
--rw-r--r--   0 runner    (1001) docker     (127)     4497 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/regression/mae.py
--rw-r--r--   0 runner    (1001) docker     (127)     5066 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/regression/mape.py
--rw-r--r--   0 runner    (1001) docker     (127)     4576 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/regression/minkowski.py
--rw-r--r--   0 runner    (1001) docker     (127)     5581 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/regression/mse.py
--rw-r--r--   0 runner    (1001) docker     (127)     8377 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/regression/pearson.py
--rw-r--r--   0 runner    (1001) docker     (127)     7332 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/regression/r2.py
--rw-r--r--   0 runner    (1001) docker     (127)     5442 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/regression/rse.py
--rw-r--r--   0 runner    (1001) docker     (127)     5751 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/regression/spearman.py
--rw-r--r--   0 runner    (1001) docker     (127)     4793 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/regression/symmetric_mape.py
--rw-r--r--   0 runner    (1001) docker     (127)     5891 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/regression/tweedie_deviance.py
--rw-r--r--   0 runner    (1001) docker     (127)     4859 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/regression/wmape.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 19:11:08.510630 torchmetrics-1.3.1/src/torchmetrics/retrieval/
--rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/retrieval/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9222 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/retrieval/_deprecated.py
--rw-r--r--   0 runner    (1001) docker     (127)     6974 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/retrieval/auroc.py
--rw-r--r--   0 runner    (1001) docker     (127)     6540 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/retrieval/average_precision.py
--rw-r--r--   0 runner    (1001) docker     (127)     8020 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/retrieval/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     8159 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/retrieval/fall_out.py
--rw-r--r--   0 runner    (1001) docker     (127)     6511 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/retrieval/hit_rate.py
--rw-r--r--   0 runner    (1001) docker     (127)     6637 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/retrieval/ndcg.py
--rw-r--r--   0 runner    (1001) docker     (127)     6892 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/retrieval/precision.py
--rw-r--r--   0 runner    (1001) docker     (127)    17854 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/retrieval/precision_recall_curve.py
--rw-r--r--   0 runner    (1001) docker     (127)     5600 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/retrieval/r_precision.py
--rw-r--r--   0 runner    (1001) docker     (127)     6489 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/retrieval/recall.py
--rw-r--r--   0 runner    (1001) docker     (127)     6530 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/retrieval/reciprocal_rank.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 19:11:08.514630 torchmetrics-1.3.1/src/torchmetrics/text/
--rw-r--r--   0 runner    (1001) docker     (127)     1819 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/text/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8261 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/text/_deprecated.py
--rw-r--r--   0 runner    (1001) docker     (127)    14222 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/text/bert.py
--rw-r--r--   0 runner    (1001) docker     (127)     5857 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/text/bleu.py
--rw-r--r--   0 runner    (1001) docker     (127)     5285 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/text/cer.py
--rw-r--r--   0 runner    (1001) docker     (127)    10476 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/text/chrf.py
--rw-r--r--   0 runner    (1001) docker     (127)     7342 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/text/edit.py
--rw-r--r--   0 runner    (1001) docker     (127)     6359 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/text/eed.py
--rw-r--r--   0 runner    (1001) docker     (127)    10155 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/text/infolm.py
--rw-r--r--   0 runner    (1001) docker     (127)     5228 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/text/mer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5064 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/text/perplexity.py
--rw-r--r--   0 runner    (1001) docker     (127)     9404 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/text/rouge.py
--rw-r--r--   0 runner    (1001) docker     (127)     6075 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/text/sacre_bleu.py
--rw-r--r--   0 runner    (1001) docker     (127)     6045 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/text/squad.py
--rw-r--r--   0 runner    (1001) docker     (127)     6745 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/text/ter.py
--rw-r--r--   0 runner    (1001) docker     (127)     5210 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/text/wer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5337 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/text/wil.py
--rw-r--r--   0 runner    (1001) docker     (127)     5358 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/text/wip.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 19:11:08.514630 torchmetrics-1.3.1/src/torchmetrics/utilities/
--rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    34595 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/utilities/checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     5078 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/utilities/compute.py
--rw-r--r--   0 runner    (1001) docker     (127)     8406 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/utilities/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     5801 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/utilities/distributed.py
--rw-r--r--   0 runner    (1001) docker     (127)     3712 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/utilities/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)      830 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/utilities/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3334 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/utilities/imports.py
--rw-r--r--   0 runner    (1001) docker     (127)    12973 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/utilities/plot.py
--rw-r--r--   0 runner    (1001) docker     (127)     2382 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/utilities/prints.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 19:11:08.514630 torchmetrics-1.3.1/src/torchmetrics/wrappers/
--rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/wrappers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/wrappers/abstract.py
--rw-r--r--   0 runner    (1001) docker     (127)     8770 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/wrappers/bootstrapping.py
--rw-r--r--   0 runner    (1001) docker     (127)     9112 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/wrappers/classwise.py
--rw-r--r--   0 runner    (1001) docker     (127)     5983 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/wrappers/feature_share.py
--rw-r--r--   0 runner    (1001) docker     (127)     6241 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/wrappers/minmax.py
--rw-r--r--   0 runner    (1001) docker     (127)     9483 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/wrappers/multioutput.py
--rw-r--r--   0 runner    (1001) docker     (127)    13700 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/wrappers/multitask.py
--rw-r--r--   0 runner    (1001) docker     (127)     8335 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/wrappers/running.py
--rw-r--r--   0 runner    (1001) docker     (127)    14700 2024-02-12 19:11:04.000000 torchmetrics-1.3.1/src/torchmetrics/wrappers/tracker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 19:11:08.514630 torchmetrics-1.3.1/src/torchmetrics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    19943 2024-02-12 19:11:08.000000 torchmetrics-1.3.1/src/torchmetrics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    14589 2024-02-12 19:11:08.000000 torchmetrics-1.3.1/src/torchmetrics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-12 19:11:08.000000 torchmetrics-1.3.1/src/torchmetrics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-12 19:11:08.000000 torchmetrics-1.3.1/src/torchmetrics.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)     1930 2024-02-12 19:11:08.000000 torchmetrics-1.3.1/src/torchmetrics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-02-12 19:11:08.000000 torchmetrics-1.3.1/src/torchmetrics.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 12:39:34.957125 torchmetrics-1.3.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    73802 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2575 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (127)    11352 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      932 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    19911 2024-03-18 12:39:34.957125 torchmetrics-1.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12724 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 12:39:34.893125 torchmetrics-1.3.2/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/requirements/_devel.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/requirements/_docs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/requirements/_doctest.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/requirements/_integrate.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/requirements/_tests.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      487 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/requirements/audio.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/requirements/audio_test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/requirements/base.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/requirements/classification_test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/requirements/detection.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/requirements/detection_test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/requirements/image.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/requirements/image_test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/requirements/multimodal.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/requirements/nominal_test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/requirements/segmentation_test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/requirements/text.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/requirements/text_test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/requirements/typing.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      306 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/requirements/visual.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-18 12:39:34.957125 torchmetrics-1.3.2/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10931 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 12:39:34.885125 torchmetrics-1.3.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 12:39:34.893125 torchmetrics-1.3.2/src/torchmetrics/
+-rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8871 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27285 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/aggregation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 12:39:34.893125 torchmetrics-1.3.2/src/torchmetrics/audio/
+-rw-r--r--   0 runner    (1001) docker     (127)     1916 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/audio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4132 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/audio/_deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7340 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/audio/pesq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6932 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/audio/pit.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15368 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/audio/sdr.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12749 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/audio/snr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7474 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/audio/srmr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6513 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/audio/stoi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 12:39:34.897125 torchmetrics-1.3.2/src/torchmetrics/classification/
+-rw-r--r--   0 runner    (1001) docker     (127)     6454 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/classification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23385 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/classification/accuracy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25578 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/classification/auroc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25440 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/classification/average_precision.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1234 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/classification/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17268 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/classification/calibration_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13693 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/classification/cohen_kappa.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23221 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/classification/confusion_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12442 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/classification/dice.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18447 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/classification/exact_match.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51823 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/classification/f_beta.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13843 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/classification/group_fairness.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24058 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/classification/hamming.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15809 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/classification/hinge.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19849 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/classification/jaccard.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17066 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/classification/matthews_corrcoef.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25339 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/classification/precision_fixed_recall.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46542 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/classification/precision_recall.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35008 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/classification/precision_recall_curve.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16435 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/classification/ranking.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25323 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/classification/recall_fixed_precision.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30081 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/classification/roc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23622 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/classification/specificity.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18828 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/classification/specificity_sensitivity.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25363 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/classification/stat_scores.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 12:39:34.901125 torchmetrics-1.3.2/src/torchmetrics/clustering/
+-rw-r--r--   0 runner    (1001) docker     (127)     1702 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/clustering/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5386 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/clustering/adjusted_mutual_info_score.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5163 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/clustering/adjusted_rand_score.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5366 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/clustering/calinski_harabasz_score.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5482 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/clustering/davies_bouldin_score.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4986 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/clustering/dunn_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4616 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/clustering/fowlkes_mallows_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12941 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/clustering/homogeneity_completeness_v_measure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5041 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/clustering/mutual_info_score.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5279 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/clustering/normalized_mutual_info_score.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4882 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/clustering/rand_score.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30413 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/collections.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 12:39:34.901125 torchmetrics-1.3.2/src/torchmetrics/detection/
+-rw-r--r--   0 runner    (1001) docker     (127)     1467 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/detection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2332 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/detection/_deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42494 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/detection/_mean_ap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8235 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/detection/ciou.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8192 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/detection/diou.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7888 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/detection/giou.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4593 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/detection/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12112 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/detection/iou.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50363 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/detection/mean_ap.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17538 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/detection/panoptic_qualities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 12:39:34.901125 torchmetrics-1.3.2/src/torchmetrics/functional/
+-rw-r--r--   0 runner    (1001) docker     (127)     9439 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/functional/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 12:39:34.905125 torchmetrics-1.3.2/src/torchmetrics/functional/audio/
+-rw-r--r--   0 runner    (1001) docker     (127)     2084 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/functional/audio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4484 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/functional/audio/_deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4832 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/functional/audio/pesq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9867 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/functional/audio/pit.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12017 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/functional/audio/sdr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5039 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/functional/audio/snr.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14302 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/functional/audio/srmr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4241 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/functional/audio/stoi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 12:39:34.909125 torchmetrics-1.3.2/src/torchmetrics/functional/classification/
+-rw-r--r--   0 runner    (1001) docker     (127)     7106 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/functional/classification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20015 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/functional/classification/accuracy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23719 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/functional/classification/auroc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23230 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/functional/classification/average_precision.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16940 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/functional/classification/calibration_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11633 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/functional/classification/cohen_kappa.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27782 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/functional/classification/confusion_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9362 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/functional/classification/dice.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11784 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/functional/classification/exact_match.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35850 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/functional/classification/f_beta.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16890 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/functional/classification/group_fairness.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20724 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/functional/classification/hamming.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12369 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/functional/classification/hinge.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16670 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/functional/classification/jaccard.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12395 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/functional/classification/matthews_corrcoef.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18072 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/functional/classification/precision_fixed_recall.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35321 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/functional/classification/precision_recall.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47018 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/functional/classification/precision_recall_curve.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11402 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/functional/classification/ranking.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21930 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/functional/classification/recall_fixed_precision.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28564 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/functional/classification/roc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18560 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/functional/classification/specificity.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23561 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/functional/classification/specificity_sensitivity.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49360 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/functional/classification/stat_scores.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 12:39:34.909125 torchmetrics-1.3.2/src/torchmetrics/functional/clustering/
+-rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/functional/clustering/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4470 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/functional/clustering/adjusted_mutual_info_score.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2422 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/functional/clustering/adjusted_rand_score.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2462 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/functional/clustering/calinski_harabasz_score.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2625 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/functional/clustering/davies_bouldin_score.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2789 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/functional/clustering/dunn_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2502 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/functional/clustering/fowlkes_mallows_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4399 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/functional/clustering/homogeneity_completeness_v_measure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2616 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/functional/clustering/mutual_info_score.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2104 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/functional/clustering/normalized_mutual_info_score.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2602 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/functional/clustering/rand_score.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10090 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/functional/clustering/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 12:39:34.909125 torchmetrics-1.3.2/src/torchmetrics/functional/detection/
+-rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/functional/detection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/functional/detection/_deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19801 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/functional/detection/_panoptic_quality_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4422 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/functional/detection/ciou.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4424 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/functional/detection/diou.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4423 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/functional/detection/giou.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4263 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/functional/detection/iou.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7896 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/functional/detection/panoptic_qualities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 12:39:34.913125 torchmetrics-1.3.2/src/torchmetrics/functional/image/
+-rw-r--r--   0 runner    (1001) docker     (127)     2572 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/functional/image/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9323 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/functional/image/_deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5678 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/functional/image/d_lambda.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11144 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/functional/image/d_s.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4297 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/functional/image/ergas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2900 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/functional/image/gradients.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16774 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/functional/image/lpips.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 12:39:34.913125 torchmetrics-1.3.2/src/torchmetrics/functional/image/lpips_models/
+-rw-r--r--   0 runner    (1001) docker     (127)     6009 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/functional/image/lpips_models/alex.pth
+-rw-r--r--   0 runner    (1001) docker     (127)    10811 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/functional/image/lpips_models/squeeze.pth
+-rw-r--r--   0 runner    (1001) docker     (127)     7289 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/functional/image/lpips_models/vgg.pth
+-rw-r--r--   0 runner    (1001) docker     (127)    13786 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/functional/image/perceptual_path_length.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5979 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/functional/image/psnr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4527 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/functional/image/psnrb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4018 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/functional/image/rase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5517 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/functional/image/rmse_sw.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4331 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/functional/image/sam.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8698 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/functional/image/scc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21659 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/functional/image/ssim.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2840 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/functional/image/tv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6561 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/functional/image/uqi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5993 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/functional/image/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4795 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/functional/image/vif.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 12:39:34.913125 torchmetrics-1.3.2/src/torchmetrics/functional/multimodal/
+-rw-r--r--   0 runner    (1001) docker     (127)      918 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/functional/multimodal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15553 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/functional/multimodal/clip_iqa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7062 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/functional/multimodal/clip_score.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 12:39:34.917125 torchmetrics-1.3.2/src/torchmetrics/functional/nominal/
+-rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/functional/nominal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7351 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/functional/nominal/cramers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4290 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/functional/nominal/fleiss_kappa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6886 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/functional/nominal/pearson.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7125 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/functional/nominal/theils_u.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7650 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/functional/nominal/tschuprows.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5756 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/functional/nominal/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 12:39:34.917125 torchmetrics-1.3.2/src/torchmetrics/functional/pairwise/
+-rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/functional/pairwise/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3499 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/functional/pairwise/cosine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3449 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/functional/pairwise/euclidean.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2253 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/functional/pairwise/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3176 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/functional/pairwise/linear.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3196 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/functional/pairwise/manhattan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3999 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/functional/pairwise/minkowski.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 12:39:34.921125 torchmetrics-1.3.2/src/torchmetrics/functional/regression/
+-rw-r--r--   0 runner    (1001) docker     (127)     2664 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/functional/regression/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2878 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/functional/regression/concordance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3635 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/functional/regression/cosine_similarity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4862 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/functional/regression/csi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5472 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/functional/regression/explained_variance.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15232 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/functional/regression/kendall.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4399 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/functional/regression/kl_divergence.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3525 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/functional/regression/log_cosh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2599 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/functional/regression/log_mse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2561 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/functional/regression/mae.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3030 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/functional/regression/mape.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3010 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/functional/regression/minkowski.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2900 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/functional/regression/mse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5308 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/functional/regression/pearson.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6639 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/functional/regression/r2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2945 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/functional/regression/rse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5142 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/functional/regression/spearman.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3305 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/functional/regression/symmetric_mape.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6096 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/functional/regression/tweedie_deviance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/functional/regression/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2679 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/functional/regression/wmape.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 12:39:34.921125 torchmetrics-1.3.2/src/torchmetrics/functional/retrieval/
+-rw-r--r--   0 runner    (1001) docker     (127)     1688 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/functional/retrieval/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5417 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/functional/retrieval/_deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2663 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/functional/retrieval/auroc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2605 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/functional/retrieval/average_precision.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2671 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/functional/retrieval/fall_out.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2409 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/functional/retrieval/hit_rate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4328 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/functional/retrieval/ndcg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2745 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/functional/retrieval/precision.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4044 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/functional/retrieval/precision_recall_curve.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2121 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/functional/retrieval/r_precision.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2504 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/functional/retrieval/recall.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2447 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/functional/retrieval/reciprocal_rank.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 12:39:34.921125 torchmetrics-1.3.2/src/torchmetrics/functional/segmentation/
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/functional/segmentation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44776 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/functional/segmentation/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 12:39:34.925125 torchmetrics-1.3.2/src/torchmetrics/functional/text/
+-rw-r--r--   0 runner    (1001) docker     (127)     2067 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/functional/text/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14008 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/functional/text/_deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21062 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/functional/text/bert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7578 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/functional/text/bleu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2983 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/functional/text/cer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26088 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/functional/text/chrf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4779 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/functional/text/edit.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17547 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/functional/text/eed.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16996 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/functional/text/helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11874 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/functional/text/helper_embedding_metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28013 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/functional/text/infolm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3031 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/functional/text/mer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5374 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/functional/text/perplexity.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21903 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/functional/text/rouge.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19053 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/functional/text/sacre_bleu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9888 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/functional/text/squad.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23307 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/functional/text/ter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2974 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/functional/text/wer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3509 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/functional/text/wil.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3513 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/functional/text/wip.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 12:39:34.929125 torchmetrics-1.3.2/src/torchmetrics/image/
+-rw-r--r--   0 runner    (1001) docker     (127)     2828 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/image/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8771 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/image/_deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6107 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/image/d_lambda.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9589 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/image/d_s.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6362 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/image/ergas.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19261 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/image/fid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9093 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/image/inception.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14540 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/image/kid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8075 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/image/lpip.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12652 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/image/mifid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8731 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/image/perceptual_path_length.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8501 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/image/psnr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5624 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/image/psnrb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5078 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/image/rase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5421 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/image/rmse_sw.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6823 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/image/sam.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3295 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/image/scc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17181 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/image/ssim.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5307 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/image/tv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6816 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/image/uqi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3207 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/image/vif.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52260 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/metric.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 12:39:34.929125 torchmetrics-1.3.2/src/torchmetrics/multimodal/
+-rw-r--r--   0 runner    (1001) docker     (127)      888 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/multimodal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11621 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/multimodal/clip_iqa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7460 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/multimodal/clip_score.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 12:39:34.929125 torchmetrics-1.3.2/src/torchmetrics/nominal/
+-rw-r--r--   0 runner    (1001) docker     (127)      986 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/nominal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6253 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/nominal/cramers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5701 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/nominal/fleiss_kappa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6548 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/nominal/pearson.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5783 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/nominal/theils_u.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6319 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/nominal/tschuprows.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 12:39:34.933125 torchmetrics-1.3.2/src/torchmetrics/regression/
+-rw-r--r--   0 runner    (1001) docker     (127)     2345 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/regression/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5420 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/regression/concordance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5208 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/regression/cosine_similarity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4821 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/regression/csi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6921 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/regression/explained_variance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8258 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/regression/kendall.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6454 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/regression/kl_divergence.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5413 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/regression/log_cosh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4687 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/regression/log_mse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4498 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/regression/mae.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5067 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/regression/mape.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4576 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/regression/minkowski.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5582 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/regression/mse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8378 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/regression/pearson.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7333 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/regression/r2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5443 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/regression/rse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5782 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/regression/spearman.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4794 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/regression/symmetric_mape.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5892 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/regression/tweedie_deviance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4860 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/regression/wmape.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 12:39:34.937125 torchmetrics-1.3.2/src/torchmetrics/retrieval/
+-rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/retrieval/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9222 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/retrieval/_deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6974 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/retrieval/auroc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6540 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/retrieval/average_precision.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8020 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/retrieval/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8159 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/retrieval/fall_out.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6511 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/retrieval/hit_rate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6637 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/retrieval/ndcg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6892 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/retrieval/precision.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17854 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/retrieval/precision_recall_curve.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5600 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/retrieval/r_precision.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6489 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/retrieval/recall.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6530 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/retrieval/reciprocal_rank.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 12:39:34.937125 torchmetrics-1.3.2/src/torchmetrics/text/
+-rw-r--r--   0 runner    (1001) docker     (127)     1819 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/text/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8261 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/text/_deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14222 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/text/bert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5857 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/text/bleu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5286 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/text/cer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10476 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/text/chrf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7342 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/text/edit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6359 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/text/eed.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10155 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/text/infolm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5229 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/text/mer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5061 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/text/perplexity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9404 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/text/rouge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6075 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/text/sacre_bleu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6045 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/text/squad.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6745 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/text/ter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5211 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/text/wer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5338 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/text/wil.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5359 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/text/wip.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 12:39:34.941125 torchmetrics-1.3.2/src/torchmetrics/utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34595 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/utilities/checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5136 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/utilities/compute.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8406 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/utilities/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5801 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/utilities/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3712 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/utilities/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)      830 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/utilities/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3132 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/utilities/imports.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12973 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/utilities/plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2382 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/utilities/prints.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 12:39:34.941125 torchmetrics-1.3.2/src/torchmetrics/wrappers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/wrappers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/wrappers/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8771 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/wrappers/bootstrapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10060 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/wrappers/classwise.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5983 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/wrappers/feature_share.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6241 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/wrappers/minmax.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9483 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/wrappers/multioutput.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13694 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/wrappers/multitask.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8335 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/wrappers/running.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14700 2024-03-18 12:39:32.000000 torchmetrics-1.3.2/src/torchmetrics/wrappers/tracker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 12:39:34.941125 torchmetrics-1.3.2/src/torchmetrics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    19911 2024-03-18 12:39:34.000000 torchmetrics-1.3.2/src/torchmetrics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    14588 2024-03-18 12:39:34.000000 torchmetrics-1.3.2/src/torchmetrics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-18 12:39:34.000000 torchmetrics-1.3.2/src/torchmetrics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-18 12:39:34.000000 torchmetrics-1.3.2/src/torchmetrics.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-03-18 12:39:34.000000 torchmetrics-1.3.2/src/torchmetrics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-03-18 12:39:34.000000 torchmetrics-1.3.2/src/torchmetrics.egg-info/top_level.txt
```

### Comparing `torchmetrics-1.3.1/CHANGELOG.md` & `torchmetrics-1.3.2/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -4,14 +4,26 @@
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 **Note: we move fast, but still we preserve 0.1 version (one feature release) back compatibility.**
 
 ---
 
+## [1.3.2] - 2024-03-18
+
+### Fixed
+
+- Fixed negative variance estimates in certain image metrics ([#2378](https://github.com/Lightning-AI/torchmetrics/pull/2378))
+- Fixed dtype being changed by deepspeed for certain regression metrics ([#2379](https://github.com/Lightning-AI/torchmetrics/pull/2379))
+- Fixed plotting of metric collection when prefix/postfix is set ([#2429](https://github.com/Lightning-AI/torchmetrics/pull/2429))
+- Fixed bug when `top_k>1` and `average="macro"` for classification metrics ([#2423](https://github.com/Lightning-AI/torchmetrics/pull/2423))
+- Fixed case where label prediction tensors in classification metrics were not validated correctly ([#2427](https://github.com/Lightning-AI/torchmetrics/pull/2427))
+- Fixed how auc scores are calculated in `PrecisionRecallCurve.plot` methods ([#2437](https://github.com/Lightning-AI/torchmetrics/pull/2437))
+
+
 ## [1.3.1] - 2024-02-12
 
 ### Fixed
 
 - Fixed how backprop is handled in `LPIPS` metric ([#2326](https://github.com/Lightning-AI/torchmetrics/pull/2326))
 - Fixed `MultitaskWrapper` not being able to be logged in lightning when using metric collections ([#2349](https://github.com/Lightning-AI/torchmetrics/pull/2349))
 - Fixed high memory consumption in `Perplexity` metric ([#2346](https://github.com/Lightning-AI/torchmetrics/pull/2346))
```

### Comparing `torchmetrics-1.3.1/CITATION.cff` & `torchmetrics-1.3.2/CITATION.cff`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.3.1/LICENSE` & `torchmetrics-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.3.1/MANIFEST.in` & `torchmetrics-1.3.2/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.3.1/PKG-INFO` & `torchmetrics-1.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchmetrics
-Version: 1.3.1
+Version: 1.3.2
 Summary: PyTorch native Metrics
 Home-page: https://github.com/Lightning-AI/torchmetrics
 Download-URL: https://github.com/Lightning-AI/torchmetrics/archive/master.zip
 Author: Lightning-AI et al.
 Author-email: name@pytorchlightning.ai
 License: Apache-2.0
 Project-URL: Bug Tracker, https://github.com/Lightning-AI/torchmetrics/issues
@@ -27,140 +27,139 @@
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy>1.20.0
 Requires-Dist: packaging>17.1
 Requires-Dist: torch>=1.10.0
-Requires-Dist: torch>=1.10.0
 Requires-Dist: typing-extensions; python_version < "3.9"
 Requires-Dist: lightning-utilities>=0.8.0
 Provides-Extra: audio
-Requires-Dist: pystoi>=0.3.0; extra == "audio"
 Requires-Dist: torchaudio>=0.10.0; extra == "audio"
+Requires-Dist: pystoi>=0.3.0; extra == "audio"
 Provides-Extra: detection
-Requires-Dist: torchvision>=0.8; extra == "detection"
 Requires-Dist: pycocotools>2.0.0; extra == "detection"
+Requires-Dist: torchvision>=0.8; extra == "detection"
 Provides-Extra: image
-Requires-Dist: torchvision>=0.8; extra == "image"
 Requires-Dist: scipy>1.0.0; extra == "image"
 Requires-Dist: torch-fidelity<=0.4.0; extra == "image"
+Requires-Dist: torchvision>=0.8; extra == "image"
 Provides-Extra: multimodal
-Requires-Dist: transformers>=4.10.0; extra == "multimodal"
 Requires-Dist: piq<=0.8.0; extra == "multimodal"
+Requires-Dist: transformers>=4.10.0; extra == "multimodal"
 Provides-Extra: text
-Requires-Dist: transformers>4.4.0; extra == "text"
-Requires-Dist: mecab-python3>=1.0.6; extra == "text"
 Requires-Dist: mecab-ko>=1.0.0; extra == "text"
-Requires-Dist: sentencepiece>=0.1.98; extra == "text"
-Requires-Dist: tqdm>=4.41.0; extra == "text"
-Requires-Dist: nltk>=3.6; extra == "text"
 Requires-Dist: regex>=2021.9.24; extra == "text"
-Requires-Dist: ipadic>=1.0.0; extra == "text"
+Requires-Dist: mecab-python3>=1.0.6; extra == "text"
 Requires-Dist: mecab-ko-dic>=1.0.0; extra == "text"
+Requires-Dist: tqdm>=4.41.0; extra == "text"
+Requires-Dist: ipadic>=1.0.0; extra == "text"
+Requires-Dist: transformers>4.4.0; extra == "text"
+Requires-Dist: sentencepiece>=0.2.0; extra == "text"
+Requires-Dist: nltk>=3.6; extra == "text"
 Provides-Extra: typing
-Requires-Dist: torch==2.2.0; extra == "typing"
-Requires-Dist: types-PyYAML; extra == "typing"
-Requires-Dist: types-emoji; extra == "typing"
-Requires-Dist: types-requests; extra == "typing"
 Requires-Dist: types-setuptools; extra == "typing"
-Requires-Dist: types-six; extra == "typing"
-Requires-Dist: mypy==1.8.0; extra == "typing"
 Requires-Dist: types-tabulate; extra == "typing"
 Requires-Dist: types-protobuf; extra == "typing"
+Requires-Dist: torch==2.2.1; extra == "typing"
+Requires-Dist: types-requests; extra == "typing"
+Requires-Dist: types-PyYAML; extra == "typing"
+Requires-Dist: mypy==1.8.0; extra == "typing"
+Requires-Dist: types-emoji; extra == "typing"
+Requires-Dist: types-six; extra == "typing"
 Provides-Extra: visual
-Requires-Dist: SciencePlots>=2.0.0; extra == "visual"
 Requires-Dist: matplotlib>=3.3.0; extra == "visual"
+Requires-Dist: SciencePlots>=2.0.0; extra == "visual"
 Provides-Extra: all
-Requires-Dist: pystoi>=0.3.0; extra == "all"
 Requires-Dist: torchaudio>=0.10.0; extra == "all"
-Requires-Dist: torchvision>=0.8; extra == "all"
+Requires-Dist: pystoi>=0.3.0; extra == "all"
 Requires-Dist: pycocotools>2.0.0; extra == "all"
 Requires-Dist: torchvision>=0.8; extra == "all"
 Requires-Dist: scipy>1.0.0; extra == "all"
 Requires-Dist: torch-fidelity<=0.4.0; extra == "all"
-Requires-Dist: transformers>=4.10.0; extra == "all"
+Requires-Dist: torchvision>=0.8; extra == "all"
 Requires-Dist: piq<=0.8.0; extra == "all"
-Requires-Dist: transformers>4.4.0; extra == "all"
-Requires-Dist: mecab-python3>=1.0.6; extra == "all"
+Requires-Dist: transformers>=4.10.0; extra == "all"
 Requires-Dist: mecab-ko>=1.0.0; extra == "all"
-Requires-Dist: sentencepiece>=0.1.98; extra == "all"
-Requires-Dist: tqdm>=4.41.0; extra == "all"
-Requires-Dist: nltk>=3.6; extra == "all"
 Requires-Dist: regex>=2021.9.24; extra == "all"
-Requires-Dist: ipadic>=1.0.0; extra == "all"
+Requires-Dist: mecab-python3>=1.0.6; extra == "all"
 Requires-Dist: mecab-ko-dic>=1.0.0; extra == "all"
-Requires-Dist: torch==2.2.0; extra == "all"
-Requires-Dist: types-PyYAML; extra == "all"
-Requires-Dist: types-emoji; extra == "all"
-Requires-Dist: types-requests; extra == "all"
+Requires-Dist: tqdm>=4.41.0; extra == "all"
+Requires-Dist: ipadic>=1.0.0; extra == "all"
+Requires-Dist: transformers>4.4.0; extra == "all"
+Requires-Dist: sentencepiece>=0.2.0; extra == "all"
+Requires-Dist: nltk>=3.6; extra == "all"
 Requires-Dist: types-setuptools; extra == "all"
-Requires-Dist: types-six; extra == "all"
-Requires-Dist: mypy==1.8.0; extra == "all"
 Requires-Dist: types-tabulate; extra == "all"
 Requires-Dist: types-protobuf; extra == "all"
-Requires-Dist: SciencePlots>=2.0.0; extra == "all"
+Requires-Dist: torch==2.2.1; extra == "all"
+Requires-Dist: types-requests; extra == "all"
+Requires-Dist: types-PyYAML; extra == "all"
+Requires-Dist: mypy==1.8.0; extra == "all"
+Requires-Dist: types-emoji; extra == "all"
+Requires-Dist: types-six; extra == "all"
 Requires-Dist: matplotlib>=3.3.0; extra == "all"
+Requires-Dist: SciencePlots>=2.0.0; extra == "all"
 Provides-Extra: dev
-Requires-Dist: pystoi>=0.3.0; extra == "dev"
 Requires-Dist: torchaudio>=0.10.0; extra == "dev"
-Requires-Dist: torchvision>=0.8; extra == "dev"
+Requires-Dist: pystoi>=0.3.0; extra == "dev"
 Requires-Dist: pycocotools>2.0.0; extra == "dev"
 Requires-Dist: torchvision>=0.8; extra == "dev"
 Requires-Dist: scipy>1.0.0; extra == "dev"
 Requires-Dist: torch-fidelity<=0.4.0; extra == "dev"
-Requires-Dist: transformers>=4.10.0; extra == "dev"
+Requires-Dist: torchvision>=0.8; extra == "dev"
 Requires-Dist: piq<=0.8.0; extra == "dev"
-Requires-Dist: transformers>4.4.0; extra == "dev"
-Requires-Dist: mecab-python3>=1.0.6; extra == "dev"
+Requires-Dist: transformers>=4.10.0; extra == "dev"
 Requires-Dist: mecab-ko>=1.0.0; extra == "dev"
-Requires-Dist: sentencepiece>=0.1.98; extra == "dev"
-Requires-Dist: tqdm>=4.41.0; extra == "dev"
-Requires-Dist: nltk>=3.6; extra == "dev"
 Requires-Dist: regex>=2021.9.24; extra == "dev"
-Requires-Dist: ipadic>=1.0.0; extra == "dev"
+Requires-Dist: mecab-python3>=1.0.6; extra == "dev"
 Requires-Dist: mecab-ko-dic>=1.0.0; extra == "dev"
-Requires-Dist: torch==2.2.0; extra == "dev"
-Requires-Dist: types-PyYAML; extra == "dev"
-Requires-Dist: types-emoji; extra == "dev"
-Requires-Dist: types-requests; extra == "dev"
+Requires-Dist: tqdm>=4.41.0; extra == "dev"
+Requires-Dist: ipadic>=1.0.0; extra == "dev"
+Requires-Dist: transformers>4.4.0; extra == "dev"
+Requires-Dist: sentencepiece>=0.2.0; extra == "dev"
+Requires-Dist: nltk>=3.6; extra == "dev"
 Requires-Dist: types-setuptools; extra == "dev"
-Requires-Dist: types-six; extra == "dev"
-Requires-Dist: mypy==1.8.0; extra == "dev"
 Requires-Dist: types-tabulate; extra == "dev"
 Requires-Dist: types-protobuf; extra == "dev"
-Requires-Dist: SciencePlots>=2.0.0; extra == "dev"
+Requires-Dist: torch==2.2.1; extra == "dev"
+Requires-Dist: types-requests; extra == "dev"
+Requires-Dist: types-PyYAML; extra == "dev"
+Requires-Dist: mypy==1.8.0; extra == "dev"
+Requires-Dist: types-emoji; extra == "dev"
+Requires-Dist: types-six; extra == "dev"
 Requires-Dist: matplotlib>=3.3.0; extra == "dev"
-Requires-Dist: statsmodels>0.13.5; extra == "dev"
-Requires-Dist: torch_complex<=0.4.3; extra == "dev"
-Requires-Dist: monai==1.3.0; extra == "dev"
+Requires-Dist: SciencePlots>=2.0.0; extra == "dev"
 Requires-Dist: rouge-score>0.1.0; extra == "dev"
-Requires-Dist: fairlearn; extra == "dev"
+Requires-Dist: mir-eval>=0.6; extra == "dev"
+Requires-Dist: bert_score==0.3.13; extra == "dev"
+Requires-Dist: lpips<=0.1.4; extra == "dev"
 Requires-Dist: scikit-image>=0.19.0; extra == "dev"
+Requires-Dist: monai==1.3.0; extra == "dev"
+Requires-Dist: sewar>=0.4.4; extra == "dev"
 Requires-Dist: jiwer>=2.3.0; extra == "dev"
-Requires-Dist: pandas>=1.4.0; extra == "dev"
-Requires-Dist: fast-bss-eval>=0.1.0; extra == "dev"
-Requires-Dist: kornia>=0.6.7; extra == "dev"
-Requires-Dist: huggingface-hub<0.21; extra == "dev"
+Requires-Dist: dython<=0.7.5; extra == "dev"
+Requires-Dist: netcal>1.0.0; extra == "dev"
+Requires-Dist: torch_complex<=0.4.3; extra == "dev"
 Requires-Dist: numpy<1.25.0; extra == "dev"
-Requires-Dist: bert_score==0.3.13; extra == "dev"
-Requires-Dist: sewar>=0.4.4; extra == "dev"
-Requires-Dist: faster-coco-eval>=1.3.3; extra == "dev"
+Requires-Dist: fairlearn; extra == "dev"
+Requires-Dist: statsmodels>0.13.5; extra == "dev"
 Requires-Dist: scipy>1.0.0; extra == "dev"
-Requires-Dist: netcal>1.0.0; extra == "dev"
-Requires-Dist: dython<=0.7.5; extra == "dev"
-Requires-Dist: pandas>1.0.0; extra == "dev"
-Requires-Dist: lpips<=0.1.4; extra == "dev"
-Requires-Dist: sacrebleu>=2.3.0; extra == "dev"
-Requires-Dist: mir-eval>=0.6; extra == "dev"
+Requires-Dist: kornia>=0.6.7; extra == "dev"
+Requires-Dist: faster-coco-eval>=1.3.3; extra == "dev"
 Requires-Dist: pytorch-msssim==1.0.0; extra == "dev"
+Requires-Dist: sacrebleu>=2.3.0; extra == "dev"
+Requires-Dist: huggingface-hub<0.22; extra == "dev"
+Requires-Dist: fast-bss-eval>=0.1.0; extra == "dev"
+Requires-Dist: pandas>1.0.0; extra == "dev"
+Requires-Dist: pandas>=1.4.0; extra == "dev"
 
 <div align="center">
 
-<img src="https://github.com/Lightning-AI/torchmetrics/raw/v1.3.1/docs/source/_static/images/logo.png" width="400px">
+<img src="https://github.com/Lightning-AI/torchmetrics/raw/v1.3.2/docs/source/_static/images/logo.png" width="400px">
 
 **Machine learning metrics for distributed, scalable PyTorch applications.**
 
 ______________________________________________________________________
 
 <p align="center">
   <a href="#what-is-torchmetrics">What is Torchmetrics</a> •
@@ -177,16 +176,16 @@
 [![PyPI Status](https://badge.fury.io/py/torchmetrics.svg)](https://badge.fury.io/py/torchmetrics)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/torchmetrics)
 ](https://pepy.tech/project/torchmetrics)
 [![Conda](https://img.shields.io/conda/v/conda-forge/torchmetrics?label=conda&color=success)](https://anaconda.org/conda-forge/torchmetrics)
 [![license](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://github.com/Lightning-AI/torchmetrics/blob/master/LICENSE)
 
 [![CI testing | CPU](https://github.com/Lightning-AI/torchmetrics/actions/workflows/ci-tests.yml/badge.svg?event=push)](https://github.com/Lightning-AI/torchmetrics/actions/workflows/ci-tests.yml)
-[![Build Status](https://dev.azure.com/Lightning-AI/Metrics/_apis/build/status%2FTM.unittests?branchName=refs%2Ftags%2Fv1.3.1)](https://dev.azure.com/Lightning-AI/Metrics/_build/latest?definitionId=2&branchName=refs%2Ftags%2Fv1.3.1)
-[![codecov](https://codecov.io/gh/Lightning-AI/torchmetrics/release/v1.3.1/graph/badge.svg?token=NER6LPI3HS)](https://codecov.io/gh/Lightning-AI/torchmetrics)
+[![Build Status](https://dev.azure.com/Lightning-AI/Metrics/_apis/build/status%2FTM.unittests?branchName=refs%2Ftags%2Fv1.3.2)](https://dev.azure.com/Lightning-AI/Metrics/_build/latest?definitionId=2&branchName=refs%2Ftags%2Fv1.3.2)
+[![codecov](https://codecov.io/gh/Lightning-AI/torchmetrics/release/v1.3.2/graph/badge.svg?token=NER6LPI3HS)](https://codecov.io/gh/Lightning-AI/torchmetrics)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/Lightning-AI/torchmetrics/master.svg)](https://results.pre-commit.ci/latest/github/Lightning-AI/torchmetrics/master)
 
 [![Documentation Status](https://readthedocs.org/projects/torchmetrics/badge/?version=latest)](https://torchmetrics.readthedocs.io/en/latest/?badge=latest)
 [![Discord](https://img.shields.io/discord/1077906959069626439?style=plastic)](https://discord.gg/VptPCZkGNa)
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.5844769.svg)](https://doi.org/10.5281/zenodo.5844769)
 [![JOSS status](https://joss.theoj.org/papers/561d9bb59b400158bc8204e2639dca43/status.svg)](https://joss.theoj.org/papers/561d9bb59b400158bc8204e2639dca43)
 
@@ -483,15 +482,15 @@
 values = []
 for i in range(10):
     values.append(acc(preds(i), target(i)))
 fig3, ax3 = acc.plot(values)
 ```
 
 <p align="center">
-  <img src="https://github.com/Lightning-AI/torchmetrics/raw/v1.3.1/docs/source/_static/images/plot_example.png" width="1000">
+  <img src="https://github.com/Lightning-AI/torchmetrics/raw/v1.3.2/docs/source/_static/images/plot_example.png" width="1000">
 </p>
 
 For examples of plotting different metrics try running [this example file](examples/plotting.py).
 
 ## Contribute!
 
 The lightning + TorchMetrics team is hard at work adding even more metrics.
```

### Comparing `torchmetrics-1.3.1/README.md` & `torchmetrics-1.3.2/README.md`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.3.1/requirements/_docs.txt` & `torchmetrics-1.3.2/requirements/_docs.txt`

 * *Files 22% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 sphinxcontrib-mockautodoc
 lai-sphinx-theme  # need to be downloaded from s3://sphinx-packages/
 sphinx-autodoc-typehints ==1.23.0
 sphinx-paramlinks ==0.6.0
 sphinx-togglebutton ==0.3.2
 sphinx-copybutton ==0.5.2
 
-lightning >=1.8.0, <2.2.0
+lightning >=1.8.0, <2.3.0
 lightning-utilities >=0.9.0, <0.11.0
 pydantic > 1.0.0, < 3.0.0
 
 # integrations
 -r _integrate.txt
 -r visual.txt
 -r audio.txt
```

### Comparing `torchmetrics-1.3.1/requirements/_tests.txt` & `torchmetrics-1.3.2/requirements/_tests.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 # NOTE: the upper bound for the package version is only set for CI stability, and it is dropped while installing this package
 #  in case you want to preserve/enforce restrictions on the latest compatible version, add "strict" as an in-line comment
 
-coverage ==7.4.1
-pytest ==7.4.4
+coverage ==7.4.3
+pytest ==8.1.1
 pytest-cov ==4.1.0
-pytest-doctestplus ==1.1.0
+pytest-doctestplus ==1.2.1
 pytest-rerunfailures ==13.0
-pytest-timeout ==2.2.0
+pytest-timeout ==2.3.1
 pytest-xdist ==3.5.0
 phmdoctest ==1.4.0
 
 psutil <5.10.0
-requests <=2.31.0
-fire <=0.5.0
+pyGithub ==2.2.0
+fire <=0.6.0
 
 cloudpickle >1.3, <=3.0.0
 scikit-learn >=1.1.1, <1.4.0
+cachier ==3.0.0
```

### Comparing `torchmetrics-1.3.1/requirements/audio_test.txt` & `torchmetrics-1.3.2/requirements/audio_test.txt`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.3.1/setup.py` & `torchmetrics-1.3.2/setup.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.3.1/src/torchmetrics/__about__.py` & `torchmetrics-1.3.2/src/torchmetrics/__about__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "1.3.1"
+__version__ = "1.3.2"
 __author__ = "Lightning-AI et al."
 __author_email__ = "name@pytorchlightning.ai"
 __license__ = "Apache-2.0"
 __copyright__ = f"Copyright (c) 2020-2023, {__author__}."
 __homepage__ = "https://github.com/Lightning-AI/torchmetrics"
 __docs__ = "PyTorch native Metrics"
 __docs_url__ = "https://lightning.ai/docs/torchmetrics/stable/"
```

### Comparing `torchmetrics-1.3.1/src/torchmetrics/__init__.py` & `torchmetrics-1.3.2/src/torchmetrics/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 r"""Root package info."""
+
 import logging as __logging
 import os
 
 from lightning_utilities.core.imports import package_available
 
 from torchmetrics.__about__ import *  # noqa: F403
```

### Comparing `torchmetrics-1.3.1/src/torchmetrics/aggregation.py` & `torchmetrics-1.3.2/src/torchmetrics/aggregation.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,17 +73,17 @@
         self.state_name = state_name
 
     def _cast_and_nan_check_input(
         self, x: Union[float, Tensor], weight: Optional[Union[float, Tensor]] = None
     ) -> Tuple[Tensor, Tensor]:
         """Convert input ``x`` to a tensor and check for Nans."""
         if not isinstance(x, Tensor):
-            x = torch.as_tensor(x, dtype=torch.float32, device=self.device)
+            x = torch.as_tensor(x, dtype=self.dtype, device=self.device)
         if weight is not None and not isinstance(weight, Tensor):
-            weight = torch.as_tensor(weight, dtype=torch.float32, device=self.device)
+            weight = torch.as_tensor(weight, dtype=self.dtype, device=self.device)
 
         nans = torch.isnan(x)
         if weight is not None:
             nans_weight = torch.isnan(weight)
         else:
             nans_weight = torch.zeros_like(nans).bool()
             weight = torch.ones_like(x)
@@ -97,15 +97,15 @@
                 weight = weight[~(nans | nans_weight)]
             else:
                 if not isinstance(self.nan_strategy, float):
                     raise ValueError(f"`nan_strategy` shall be float but you pass {self.nan_strategy}")
                 x[nans | nans_weight] = self.nan_strategy
                 weight[nans | nans_weight] = self.nan_strategy
 
-        return x.float(), weight.float()
+        return x.to(self.dtype), weight.to(self.dtype)
 
     def update(self, value: Union[float, Tensor]) -> None:
         """Overwrite in child class."""
 
     def compute(self) -> Tensor:
         """Compute the aggregated value."""
         return getattr(self, self.state_name)
@@ -553,17 +553,17 @@
                 the average. Shape of weight should be able to broadcast with
                 the shape of `value`. Default to `1.0` corresponding to simple
                 harmonic average.
 
         """
         # broadcast weight to value shape
         if not isinstance(value, Tensor):
-            value = torch.as_tensor(value, dtype=torch.float32, device=self.device)
+            value = torch.as_tensor(value, dtype=self.dtype, device=self.device)
         if weight is not None and not isinstance(weight, Tensor):
-            weight = torch.as_tensor(weight, dtype=torch.float32, device=self.device)
+            weight = torch.as_tensor(weight, dtype=self.dtype, device=self.device)
         weight = torch.broadcast_to(weight, value.shape)
         value, weight = self._cast_and_nan_check_input(value, weight)
 
         if value.numel() == 0:
             return
         self.mean_value += (value * weight).sum()
         self.weight += weight.sum()
```

### Comparing `torchmetrics-1.3.1/src/torchmetrics/audio/__init__.py` & `torchmetrics-1.3.2/src/torchmetrics/audio/__init__.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.3.1/src/torchmetrics/audio/_deprecated.py` & `torchmetrics-1.3.2/src/torchmetrics/audio/_deprecated.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.3.1/src/torchmetrics/audio/pesq.py` & `torchmetrics-1.3.2/src/torchmetrics/audio/pesq.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.3.1/src/torchmetrics/audio/pit.py` & `torchmetrics-1.3.2/src/torchmetrics/audio/pit.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.3.1/src/torchmetrics/audio/sdr.py` & `torchmetrics-1.3.2/src/torchmetrics/audio/sdr.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.3.1/src/torchmetrics/audio/snr.py` & `torchmetrics-1.3.2/src/torchmetrics/audio/snr.py`

 * *Files 0% similar despite different names*

```diff
@@ -64,14 +64,15 @@
         >>> target = tensor([3.0, -0.5, 2.0, 7.0])
         >>> preds = tensor([2.5, 0.0, 2.0, 8.0])
         >>> snr = SignalNoiseRatio()
         >>> snr(preds, target)
         tensor(16.1805)
 
     """
+
     full_state_update: bool = False
     is_differentiable: bool = True
     higher_is_better: bool = True
     sum_snr: Tensor
     total: Tensor
     plot_lower_bound: Optional[float] = None
     plot_upper_bound: Optional[float] = None
```

### Comparing `torchmetrics-1.3.1/src/torchmetrics/audio/srmr.py` & `torchmetrics-1.3.2/src/torchmetrics/audio/srmr.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.3.1/src/torchmetrics/audio/stoi.py` & `torchmetrics-1.3.2/src/torchmetrics/audio/stoi.py`

 * *Files 0% similar despite different names*

```diff
@@ -69,14 +69,15 @@
         >>> preds = torch.randn(8000)
         >>> target = torch.randn(8000)
         >>> stoi = ShortTimeObjectiveIntelligibility(8000, False)
         >>> stoi(preds, target)
         tensor(-0.0100)
 
     """
+
     sum_stoi: Tensor
     total: Tensor
     full_state_update: bool = False
     is_differentiable: bool = False
     higher_is_better: bool = True
     plot_lower_bound: float = 0.0
     plot_upper_bound: float = 1.0
```

### Comparing `torchmetrics-1.3.1/src/torchmetrics/classification/__init__.py` & `torchmetrics-1.3.2/src/torchmetrics/classification/__init__.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.3.1/src/torchmetrics/classification/accuracy.py` & `torchmetrics-1.3.2/src/torchmetrics/classification/accuracy.py`

 * *Files 1% similar despite different names*

```diff
@@ -89,14 +89,15 @@
         >>> preds = tensor([[[0.59, 0.91], [0.91, 0.99], [0.63, 0.04]],
         ...                 [[0.38, 0.04], [0.86, 0.780], [0.45, 0.37]]])
         >>> metric = BinaryAccuracy(multidim_average='samplewise')
         >>> metric(preds, target)
         tensor([0.3333, 0.1667])
 
     """
+
     is_differentiable: bool = False
     higher_is_better: bool = True
     full_state_update: bool = False
     plot_lower_bound: float = 0.0
     plot_upper_bound: float = 1.0
 
     def compute(self) -> Tensor:
@@ -240,25 +241,28 @@
         tensor([0.5000, 0.2778])
         >>> mca = MulticlassAccuracy(num_classes=3, multidim_average='samplewise', average=None)
         >>> mca(preds, target)
         tensor([[1.0000, 0.0000, 0.5000],
                 [0.0000, 0.3333, 0.5000]])
 
     """
+
     is_differentiable: bool = False
     higher_is_better: bool = True
     full_state_update: bool = False
     plot_lower_bound: float = 0.0
     plot_upper_bound: float = 1.0
     plot_legend_name: str = "Class"
 
     def compute(self) -> Tensor:
         """Compute accuracy based on inputs passed in to ``update`` previously."""
         tp, fp, tn, fn = self._final_state()
-        return _accuracy_reduce(tp, fp, tn, fn, average=self.average, multidim_average=self.multidim_average)
+        return _accuracy_reduce(
+            tp, fp, tn, fn, average=self.average, multidim_average=self.multidim_average, top_k=self.top_k
+        )
 
     def plot(
         self, val: Optional[Union[Tensor, Sequence[Tensor]]] = None, ax: Optional[_AX_TYPE] = None
     ) -> _PLOT_OUT_TYPE:
         """Plot a single or multiple values from the metric.
 
         Args:
@@ -392,14 +396,15 @@
         tensor([0.3333, 0.1667])
         >>> mla = MultilabelAccuracy(num_labels=3, multidim_average='samplewise', average=None)
         >>> mla(preds, target)
         tensor([[0.5000, 0.5000, 0.0000],
                 [0.0000, 0.0000, 0.5000]])
 
     """
+
     is_differentiable: bool = False
     higher_is_better: bool = True
     full_state_update: bool = False
     plot_lower_bound: float = 0.0
     plot_upper_bound: float = 1.0
     plot_legend_name: str = "Label"
 
@@ -495,17 +500,19 @@
         ignore_index: Optional[int] = None,
         validate_args: bool = True,
         **kwargs: Any,
     ) -> Metric:
         """Initialize task metric."""
         task = ClassificationTask.from_str(task)
 
-        kwargs.update(
-            {"multidim_average": multidim_average, "ignore_index": ignore_index, "validate_args": validate_args}
-        )
+        kwargs.update({
+            "multidim_average": multidim_average,
+            "ignore_index": ignore_index,
+            "validate_args": validate_args,
+        })
 
         if task == ClassificationTask.BINARY:
             return BinaryAccuracy(threshold, **kwargs)
         if task == ClassificationTask.MULTICLASS:
             if not isinstance(num_classes, int):
                 raise ValueError(
                     f"Optional arg `num_classes` must be type `int` when task is {task}. Got {type(num_classes)}"
```

### Comparing `torchmetrics-1.3.1/src/torchmetrics/classification/auroc.py` & `torchmetrics-1.3.2/src/torchmetrics/classification/auroc.py`

 * *Files 0% similar despite different names*

```diff
@@ -94,14 +94,15 @@
         >>> metric(preds, target)
         tensor(0.5000)
         >>> b_auroc = BinaryAUROC(thresholds=5)
         >>> b_auroc(preds, target)
         tensor(0.5000)
 
     """
+
     is_differentiable: bool = False
     higher_is_better: bool = True
     full_state_update: bool = False
     plot_lower_bound: float = 0.0
     plot_upper_bound: float = 1.0
 
     def __init__(
@@ -269,15 +270,18 @@
         self.average = average  # type: ignore[assignment]
         self.validate_args = validate_args
 
     def compute(self) -> Tensor:  # type: ignore[override]
         """Compute metric."""
         state = (dim_zero_cat(self.preds), dim_zero_cat(self.target)) if self.thresholds is None else self.confmat
         return _multiclass_auroc_compute(
-            state, self.num_classes, self.average, self.thresholds  # type: ignore[arg-type]
+            state,
+            self.num_classes,
+            self.average,  # type: ignore[arg-type]
+            self.thresholds,
         )
 
     def plot(  # type: ignore[override]
         self, val: Optional[Union[Tensor, Sequence[Tensor]]] = None, ax: Optional[_AX_TYPE] = None
     ) -> _PLOT_OUT_TYPE:
         """Plot a single or multiple values from the metric.
 
@@ -392,14 +396,15 @@
         >>> ml_auroc(preds, target)
         tensor(0.6528)
         >>> ml_auroc = MultilabelAUROC(num_labels=3, average=None, thresholds=5)
         >>> ml_auroc(preds, target)
         tensor([0.6250, 0.5000, 0.8333])
 
     """
+
     is_differentiable: bool = False
     higher_is_better: bool = True
     full_state_update: bool = False
     plot_lower_bound: float = 0.0
     plot_upper_bound: float = 1.0
     plot_legend_name: str = "Label"
```

### Comparing `torchmetrics-1.3.1/src/torchmetrics/classification/average_precision.py` & `torchmetrics-1.3.2/src/torchmetrics/classification/average_precision.py`

 * *Files 1% similar despite different names*

```diff
@@ -101,14 +101,15 @@
         >>> metric(preds, target)
         tensor(0.5833)
         >>> bap = BinaryAveragePrecision(thresholds=5)
         >>> bap(preds, target)
         tensor(0.6667)
 
     """
+
     is_differentiable: bool = False
     higher_is_better: bool = True
     full_state_update: bool = False
     plot_lower_bound: float = 0.0
     plot_upper_bound: float = 1.0
 
     def compute(self) -> Tensor:  # type: ignore[override]
@@ -267,15 +268,18 @@
         self.average = average  # type: ignore[assignment]
         self.validate_args = validate_args
 
     def compute(self) -> Tensor:  # type: ignore[override]
         """Compute metric."""
         state = (dim_zero_cat(self.preds), dim_zero_cat(self.target)) if self.thresholds is None else self.confmat
         return _multiclass_average_precision_compute(
-            state, self.num_classes, self.average, self.thresholds  # type: ignore[arg-type]
+            state,
+            self.num_classes,
+            self.average,  # type: ignore[arg-type]
+            self.thresholds,
         )
 
     def plot(  # type: ignore[override]
         self, val: Optional[Union[Tensor, Sequence[Tensor]]] = None, ax: Optional[_AX_TYPE] = None
     ) -> _PLOT_OUT_TYPE:
         """Plot a single or multiple values from the metric.
 
@@ -395,14 +399,15 @@
         >>> mlap(preds, target)
         tensor(0.7778)
         >>> mlap = MultilabelAveragePrecision(num_labels=3, average=None, thresholds=5)
         >>> mlap(preds, target)
         tensor([0.7500, 0.6667, 0.9167])
 
     """
+
     is_differentiable: bool = False
     higher_is_better: bool = True
     full_state_update: bool = False
     plot_lower_bound: float = 0.0
     plot_upper_bound: float = 1.0
     plot_legend_name: str = "Label"
```

### Comparing `torchmetrics-1.3.1/src/torchmetrics/classification/base.py` & `torchmetrics-1.3.2/src/torchmetrics/classification/base.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.3.1/src/torchmetrics/classification/calibration_error.py` & `torchmetrics-1.3.2/src/torchmetrics/classification/calibration_error.py`

 * *Files 0% similar despite different names*

```diff
@@ -94,14 +94,15 @@
         >>> bce(preds, target)
         tensor(0.2918)
         >>> bce = BinaryCalibrationError(n_bins=2, norm='max')
         >>> bce(preds, target)
         tensor(0.3167)
 
     """
+
     is_differentiable: bool = False
     higher_is_better: bool = False
     full_state_update: bool = False
     plot_lower_bound: float = 0.0
     plot_upper_bound: float = 1.0
 
     confidences: List[Tensor]
@@ -245,14 +246,15 @@
         >>> mcce(preds, target)
         tensor(0.2082)
         >>> mcce = MulticlassCalibrationError(num_classes=3, n_bins=3, norm='max')
         >>> mcce(preds, target)
         tensor(0.2333)
 
     """
+
     is_differentiable: bool = False
     higher_is_better: bool = False
     full_state_update: bool = False
     plot_lower_bound: float = 0.0
     plot_upper_bound: float = 1.0
     plot_legend_name: str = "Class"
```

### Comparing `torchmetrics-1.3.1/src/torchmetrics/classification/cohen_kappa.py` & `torchmetrics-1.3.2/src/torchmetrics/classification/cohen_kappa.py`

 * *Files 0% similar despite different names*

```diff
@@ -85,14 +85,15 @@
         >>> target = tensor([1, 1, 0, 0])
         >>> preds = tensor([0.35, 0.85, 0.48, 0.01])
         >>> metric = BinaryCohenKappa()
         >>> metric(preds, target)
         tensor(0.5000)
 
     """
+
     is_differentiable: bool = False
     higher_is_better: bool = True
     full_state_update: bool = False
     plot_lower_bound: float = 0.0
     plot_upper_bound: float = 1.0
 
     def __init__(
@@ -212,14 +213,15 @@
         ...                 [0.71, 0.09, 0.20],
         ...                 [0.05, 0.82, 0.13]])
         >>> metric = MulticlassCohenKappa(num_classes=3)
         >>> metric(preds, target)
         tensor(0.6364)
 
     """
+
     is_differentiable: bool = False
     higher_is_better: bool = True
     full_state_update: bool = False
     plot_lower_bound: float = 0.0
     plot_upper_bound: float = 1.0
     plot_legend_name: str = "Class"
```

### Comparing `torchmetrics-1.3.1/src/torchmetrics/classification/confusion_matrix.py` & `torchmetrics-1.3.2/src/torchmetrics/classification/confusion_matrix.py`

 * *Files 0% similar despite different names*

```diff
@@ -104,14 +104,15 @@
         >>> preds = torch.tensor([0.35, 0.85, 0.48, 0.01])
         >>> bcm = BinaryConfusionMatrix()
         >>> bcm(preds, target)
         tensor([[2, 0],
                 [1, 1]])
 
     """
+
     is_differentiable: bool = False
     higher_is_better: Optional[bool] = None
     full_state_update: bool = False
 
     confmat: Tensor
 
     def __init__(
@@ -244,14 +245,15 @@
         >>> metric = MulticlassConfusionMatrix(num_classes=3)
         >>> metric(preds, target)
         tensor([[1, 1, 0],
                 [0, 1, 0],
                 [0, 0, 1]])
 
     """
+
     is_differentiable: bool = False
     higher_is_better: Optional[bool] = None
     full_state_update: bool = False
 
     confmat: Tensor
 
     def __init__(
@@ -383,14 +385,15 @@
         >>> metric = MultilabelConfusionMatrix(num_labels=3)
         >>> metric(preds, target)
         tensor([[[1, 0], [0, 1]],
                 [[1, 0], [1, 0]],
                 [[0, 1], [0, 1]]])
 
     """
+
     is_differentiable: bool = False
     higher_is_better: Optional[bool] = None
     full_state_update: bool = False
 
     confmat: Tensor
 
     def __init__(
```

### Comparing `torchmetrics-1.3.1/src/torchmetrics/classification/dice.py` & `torchmetrics-1.3.2/src/torchmetrics/classification/dice.py`

 * *Files 0% similar despite different names*

```diff
@@ -130,14 +130,15 @@
         >>> preds  = tensor([2, 0, 2, 1])
         >>> target = tensor([1, 1, 2, 0])
         >>> dice = Dice(average='micro')
         >>> dice(preds, target)
         tensor(0.2500)
 
     """
+
     is_differentiable: bool = False
     higher_is_better: bool = True
     full_state_update: bool = False
     plot_lower_bound: float = 0.0
     plot_upper_bound: float = 1.0
     plot_legend_name: str = "Class"
```

### Comparing `torchmetrics-1.3.1/src/torchmetrics/classification/exact_match.py` & `torchmetrics-1.3.2/src/torchmetrics/classification/exact_match.py`

 * *Files 0% similar despite different names*

```diff
@@ -92,14 +92,15 @@
         >>> target = tensor([[[0, 1], [2, 1], [0, 2]], [[1, 1], [2, 0], [1, 2]]])
         >>> preds = tensor([[[0, 1], [2, 1], [0, 2]], [[2, 2], [2, 1], [1, 0]]])
         >>> metric = MulticlassExactMatch(num_classes=3, multidim_average='samplewise')
         >>> metric(preds, target)
         tensor([1., 0.])
 
     """
+
     is_differentiable: bool = False
     higher_is_better: bool = True
     full_state_update: bool = False
     plot_lower_bound: float = 0.0
     plot_upper_bound: float = 1.0
     plot_legend_name: str = "Class"
 
@@ -401,17 +402,19 @@
         multidim_average: Literal["global", "samplewise"] = "global",
         ignore_index: Optional[int] = None,
         validate_args: bool = True,
         **kwargs: Any,
     ) -> Metric:
         """Initialize task metric."""
         task = ClassificationTaskNoBinary.from_str(task)
-        kwargs.update(
-            {"multidim_average": multidim_average, "ignore_index": ignore_index, "validate_args": validate_args}
-        )
+        kwargs.update({
+            "multidim_average": multidim_average,
+            "ignore_index": ignore_index,
+            "validate_args": validate_args,
+        })
         if task == ClassificationTaskNoBinary.MULTICLASS:
             if not isinstance(num_classes, int):
                 raise ValueError(f"`num_classes` is expected to be `int` but `{type(num_classes)} was passed.`")
             return MulticlassExactMatch(num_classes, **kwargs)
         if task == ClassificationTaskNoBinary.MULTILABEL:
             if not isinstance(num_labels, int):
                 raise ValueError(f"`num_labels` is expected to be `int` but `{type(num_labels)} was passed.`")
```

### Comparing `torchmetrics-1.3.1/src/torchmetrics/classification/f_beta.py` & `torchmetrics-1.3.2/src/torchmetrics/classification/f_beta.py`

 * *Files 0% similar despite different names*

```diff
@@ -107,14 +107,15 @@
         >>> preds = tensor([[[0.59, 0.91], [0.91, 0.99],  [0.63, 0.04]],
         ...                 [[0.38, 0.04], [0.86, 0.780], [0.45, 0.37]]])
         >>> metric = BinaryFBetaScore(beta=2.0, multidim_average='samplewise')
         >>> metric(preds, target)
         tensor([0.5882, 0.0000])
 
     """
+
     is_differentiable: bool = False
     higher_is_better: Optional[bool] = True
     full_state_update: bool = False
     plot_lower_bound: float = 0.0
     plot_upper_bound: float = 1.0
 
     def __init__(
@@ -284,14 +285,15 @@
         tensor([0.4697, 0.2706])
         >>> mcfbs = MulticlassFBetaScore(beta=2.0, num_classes=3, multidim_average='samplewise', average=None)
         >>> mcfbs(preds, target)
         tensor([[0.9091, 0.0000, 0.5000],
                 [0.0000, 0.3571, 0.4545]])
 
     """
+
     is_differentiable: bool = False
     higher_is_better: Optional[bool] = True
     full_state_update: bool = False
     plot_lower_bound: float = 0.0
     plot_upper_bound: float = 1.0
     plot_legend_name: str = "Class"
 
@@ -462,14 +464,15 @@
         tensor([0.5556, 0.0000])
         >>> mlfbs = MultilabelFBetaScore(num_labels=3, beta=2.0, multidim_average='samplewise', average=None)
         >>> mlfbs(preds, target)
         tensor([[0.8333, 0.8333, 0.0000],
                 [0.0000, 0.0000, 0.0000]])
 
     """
+
     is_differentiable: bool = False
     higher_is_better: Optional[bool] = True
     full_state_update: bool = False
     plot_lower_bound: float = 0.0
     plot_upper_bound: float = 1.0
     plot_legend_name: str = "Label"
 
@@ -613,14 +616,15 @@
         >>> preds = tensor([[[0.59, 0.91], [0.91, 0.99],  [0.63, 0.04]],
         ...                 [[0.38, 0.04], [0.86, 0.780], [0.45, 0.37]]])
         >>> metric = BinaryF1Score(multidim_average='samplewise')
         >>> metric(preds, target)
         tensor([0.5000, 0.0000])
 
     """
+
     is_differentiable: bool = False
     higher_is_better: Optional[bool] = True
     full_state_update: bool = False
     plot_lower_bound: float = 0.0
     plot_upper_bound: float = 1.0
 
     def __init__(
@@ -780,14 +784,15 @@
         tensor([0.4333, 0.2667])
         >>> mcf1s = MulticlassF1Score(num_classes=3, multidim_average='samplewise', average=None)
         >>> mcf1s(preds, target)
         tensor([[0.8000, 0.0000, 0.5000],
                 [0.0000, 0.4000, 0.4000]])
 
     """
+
     is_differentiable: bool = False
     higher_is_better: Optional[bool] = True
     full_state_update: bool = False
     plot_lower_bound: float = 0.0
     plot_upper_bound: float = 1.0
     plot_legend_name: str = "Class"
 
@@ -948,14 +953,15 @@
         tensor([0.4444, 0.0000])
         >>> mlf1s = MultilabelF1Score(num_labels=3, multidim_average='samplewise', average=None)
         >>> mlf1s(preds, target)
         tensor([[0.6667, 0.6667, 0.0000],
                 [0.0000, 0.0000, 0.0000]])
 
     """
+
     is_differentiable: bool = False
     higher_is_better: Optional[bool] = True
     full_state_update: bool = False
     plot_lower_bound: float = 0.0
     plot_upper_bound: float = 1.0
     plot_legend_name: str = "Label"
 
@@ -1065,17 +1071,19 @@
         ignore_index: Optional[int] = None,
         validate_args: bool = True,
         **kwargs: Any,
     ) -> Metric:
         """Initialize task metric."""
         task = ClassificationTask.from_str(task)
         assert multidim_average is not None  # noqa: S101  # needed for mypy
-        kwargs.update(
-            {"multidim_average": multidim_average, "ignore_index": ignore_index, "validate_args": validate_args}
-        )
+        kwargs.update({
+            "multidim_average": multidim_average,
+            "ignore_index": ignore_index,
+            "validate_args": validate_args,
+        })
         if task == ClassificationTask.BINARY:
             return BinaryFBetaScore(beta, threshold, **kwargs)
         if task == ClassificationTask.MULTICLASS:
             if not isinstance(num_classes, int):
                 raise ValueError(f"`num_classes` is expected to be `int` but `{type(num_classes)} was passed.`")
             if not isinstance(top_k, int):
                 raise ValueError(f"`top_k` is expected to be `int` but `{type(top_k)} was passed.`")
@@ -1126,17 +1134,19 @@
         ignore_index: Optional[int] = None,
         validate_args: bool = True,
         **kwargs: Any,
     ) -> Metric:
         """Initialize task metric."""
         task = ClassificationTask.from_str(task)
         assert multidim_average is not None  # noqa: S101  # needed for mypy
-        kwargs.update(
-            {"multidim_average": multidim_average, "ignore_index": ignore_index, "validate_args": validate_args}
-        )
+        kwargs.update({
+            "multidim_average": multidim_average,
+            "ignore_index": ignore_index,
+            "validate_args": validate_args,
+        })
         if task == ClassificationTask.BINARY:
             return BinaryF1Score(threshold, **kwargs)
         if task == ClassificationTask.MULTICLASS:
             if not isinstance(num_classes, int):
                 raise ValueError(f"`num_classes` is expected to be `int` but `{type(num_classes)} was passed.`")
             if not isinstance(top_k, int):
                 raise ValueError(f"`top_k` is expected to be `int` but `{type(top_k)} was passed.`")
```

### Comparing `torchmetrics-1.3.1/src/torchmetrics/classification/group_fairness.py` & `torchmetrics-1.3.2/src/torchmetrics/classification/group_fairness.py`

 * *Files 0% similar despite different names*

```diff
@@ -97,14 +97,15 @@
         >>> preds = torch.tensor([0.11, 0.84, 0.22, 0.73, 0.33, 0.92])
         >>> groups = torch.tensor([0, 1, 0, 1, 0, 1])
         >>> metric = BinaryGroupStatRates(num_groups=2)
         >>> metric(preds, target, groups)
         {'group_0': tensor([0., 0., 1., 0.]), 'group_1': tensor([1., 0., 0., 0.])}
 
     """
+
     is_differentiable: bool = False
     higher_is_better: bool = False
     full_state_update: bool = False
     plot_lower_bound: float = 0.0
     plot_upper_bound: float = 1.0
 
     def __init__(
@@ -203,14 +204,15 @@
         >>> preds = torch.tensor([0.11, 0.84, 0.22, 0.73, 0.33, 0.92])
         >>> groups = torch.tensor([0, 1, 0, 1, 0, 1])
         >>> metric = BinaryFairness(2)
         >>> metric(preds, target, groups)
         {'DP_0_1': tensor(0.), 'EO_0_1': tensor(0.)}
 
     """
+
     is_differentiable: bool = False
     higher_is_better: bool = False
     full_state_update: bool = False
     plot_lower_bound: float = 0.0
     plot_upper_bound: float = 1.0
 
     def __init__(
```

### Comparing `torchmetrics-1.3.1/src/torchmetrics/classification/hamming.py` & `torchmetrics-1.3.2/src/torchmetrics/classification/hamming.py`

 * *Files 0% similar despite different names*

```diff
@@ -504,17 +504,19 @@
         ignore_index: Optional[int] = None,
         validate_args: bool = True,
         **kwargs: Any,
     ) -> Metric:
         """Initialize task metric."""
         task = ClassificationTask.from_str(task)
         assert multidim_average is not None  # noqa: S101  # needed for mypy
-        kwargs.update(
-            {"multidim_average": multidim_average, "ignore_index": ignore_index, "validate_args": validate_args}
-        )
+        kwargs.update({
+            "multidim_average": multidim_average,
+            "ignore_index": ignore_index,
+            "validate_args": validate_args,
+        })
         if task == ClassificationTask.BINARY:
             return BinaryHammingDistance(threshold, **kwargs)
         if task == ClassificationTask.MULTICLASS:
             if not isinstance(num_classes, int):
                 raise ValueError(f"`num_classes` is expected to be `int` but `{type(num_classes)} was passed.`")
             if not isinstance(top_k, int):
                 raise ValueError(f"`top_k` is expected to be `int` but `{type(top_k)} was passed.`")
```

### Comparing `torchmetrics-1.3.1/src/torchmetrics/classification/hinge.py` & `torchmetrics-1.3.2/src/torchmetrics/classification/hinge.py`

 * *Files 0% similar despite different names*

```diff
@@ -79,14 +79,15 @@
         >>> bhl(preds, target)
         tensor(0.6900)
         >>> bhl = BinaryHingeLoss(squared=True)
         >>> bhl(preds, target)
         tensor(0.6905)
 
     """
+
     is_differentiable: bool = True
     higher_is_better: bool = False
     full_state_update: bool = False
     plot_lower_bound: float = 0.0
     plot_upper_bound: float = 1.0
 
     measures: Tensor
@@ -221,14 +222,15 @@
         >>> mchl(preds, target)
         tensor(1.1131)
         >>> mchl = MulticlassHingeLoss(num_classes=3, multiclass_mode='one-vs-all')
         >>> mchl(preds, target)
         tensor([0.8750, 1.1250, 1.1000])
 
     """
+
     is_differentiable: bool = True
     higher_is_better: bool = False
     full_state_update: bool = False
     plot_lower_bound: float = 0.0
     plot_upper_bound: float = 1.0
     plot_legend_name: str = "Class"
```

### Comparing `torchmetrics-1.3.1/src/torchmetrics/classification/jaccard.py` & `torchmetrics-1.3.2/src/torchmetrics/classification/jaccard.py`

 * *Files 0% similar despite different names*

```diff
@@ -81,14 +81,15 @@
         >>> target = tensor([1, 1, 0, 0])
         >>> preds = tensor([0.35, 0.85, 0.48, 0.01])
         >>> metric = BinaryJaccardIndex()
         >>> metric(preds, target)
         tensor(0.5000)
 
     """
+
     is_differentiable: bool = False
     higher_is_better: bool = True
     full_state_update: bool = False
     plot_lower_bound: float = 0.0
     plot_upper_bound: float = 1.0
 
     def __init__(
@@ -205,14 +206,15 @@
         ...                 [0.71, 0.09, 0.20],
         ...                 [0.05, 0.82, 0.13]])
         >>> metric = MulticlassJaccardIndex(num_classes=3)
         >>> metric(preds, target)
         tensor(0.6667)
 
     """
+
     is_differentiable: bool = False
     higher_is_better: bool = True
     full_state_update: bool = False
     plot_lower_bound: float = 0.0
     plot_upper_bound: float = 1.0
     plot_legend_name: str = "Class"
```

### Comparing `torchmetrics-1.3.1/src/torchmetrics/classification/matthews_corrcoef.py` & `torchmetrics-1.3.2/src/torchmetrics/classification/matthews_corrcoef.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.3.1/src/torchmetrics/classification/precision_fixed_recall.py` & `torchmetrics-1.3.2/src/torchmetrics/classification/precision_fixed_recall.py`

 * *Files 0% similar despite different names*

```diff
@@ -101,14 +101,15 @@
         >>> metric(preds, target)
         (tensor(0.6667), tensor(0.5000))
         >>> metric = BinaryPrecisionAtFixedRecall(min_recall=0.5, thresholds=5)
         >>> metric(preds, target)
         (tensor(0.6667), tensor(0.5000))
 
     """
+
     is_differentiable: bool = False
     higher_is_better: Optional[bool] = None
     full_state_update: bool = False
     plot_lower_bound: float = 0.0
     plot_upper_bound: float = 1.0
 
     def __init__(
@@ -241,14 +242,15 @@
          tensor([7.5000e-01, 7.5000e-01, 5.0000e-02, 5.0000e-02, 1.0000e+06]))
         >>> mcrafp = MulticlassPrecisionAtFixedRecall(num_classes=5, min_recall=0.5, thresholds=5)
         >>> mcrafp(preds, target)  # doctest: +NORMALIZE_WHITESPACE
         (tensor([1.0000, 1.0000, 0.2500, 0.2500, 0.0000]),
          tensor([7.5000e-01, 7.5000e-01, 0.0000e+00, 0.0000e+00, 1.0000e+06]))
 
     """
+
     is_differentiable: bool = False
     higher_is_better: Optional[bool] = None
     full_state_update: bool = False
     plot_lower_bound: float = 0.0
     plot_upper_bound: float = 1.0
     plot_legend_name: str = "Class"
 
@@ -386,14 +388,15 @@
         >>> metric(preds, target)
         (tensor([1.0000, 0.6667, 1.0000]), tensor([0.7500, 0.5500, 0.3500]))
         >>> mlrafp = MultilabelPrecisionAtFixedRecall(num_labels=3, min_recall=0.5, thresholds=5)
         >>> mlrafp(preds, target)
         (tensor([1.0000, 0.6667, 1.0000]), tensor([0.7500, 0.5000, 0.2500]))
 
     """
+
     is_differentiable: bool = False
     higher_is_better: Optional[bool] = None
     full_state_update: bool = False
     plot_lower_bound: float = 0.0
     plot_upper_bound: float = 1.0
     plot_legend_name: str = "Label"
```

### Comparing `torchmetrics-1.3.1/src/torchmetrics/classification/precision_recall.py` & `torchmetrics-1.3.2/src/torchmetrics/classification/precision_recall.py`

 * *Files 1% similar despite different names*

```diff
@@ -97,14 +97,15 @@
         >>> preds = tensor([[[0.59, 0.91], [0.91, 0.99],  [0.63, 0.04]],
         ...                 [[0.38, 0.04], [0.86, 0.780], [0.45, 0.37]]])
         >>> metric = BinaryPrecision(multidim_average='samplewise')
         >>> metric(preds, target)
         tensor([0.4000, 0.0000])
 
     """
+
     is_differentiable: bool = False
     higher_is_better: Optional[bool] = True
     full_state_update: bool = False
     plot_lower_bound: float = 0.0
     plot_upper_bound: float = 1.0
 
     def compute(self) -> Tensor:
@@ -252,26 +253,27 @@
         tensor([0.3889, 0.2778])
         >>> mcp = MulticlassPrecision(num_classes=3, multidim_average='samplewise', average=None)
         >>> mcp(preds, target)
         tensor([[0.6667, 0.0000, 0.5000],
                 [0.0000, 0.5000, 0.3333]])
 
     """
+
     is_differentiable: bool = False
     higher_is_better: Optional[bool] = True
     full_state_update: bool = False
     plot_lower_bound: float = 0.0
     plot_upper_bound: float = 1.0
     plot_legend_name: str = "Class"
 
     def compute(self) -> Tensor:
         """Compute metric."""
         tp, fp, tn, fn = self._final_state()
         return _precision_recall_reduce(
-            "precision", tp, fp, tn, fn, average=self.average, multidim_average=self.multidim_average
+            "precision", tp, fp, tn, fn, average=self.average, multidim_average=self.multidim_average, top_k=self.top_k
         )
 
     def plot(
         self, val: Optional[Union[Tensor, Sequence[Tensor]]] = None, ax: Optional[_AX_TYPE] = None
     ) -> _PLOT_OUT_TYPE:
         """Plot a single or multiple values from the metric.
 
@@ -405,14 +407,15 @@
         tensor([0.3333, 0.0000])
         >>> mlp = MultilabelPrecision(num_labels=3, multidim_average='samplewise', average=None)
         >>> mlp(preds, target)
         tensor([[0.5000, 0.5000, 0.0000],
                 [0.0000, 0.0000, 0.0000]])
 
     """
+
     is_differentiable: bool = False
     higher_is_better: Optional[bool] = True
     full_state_update: bool = False
     plot_lower_bound: float = 0.0
     plot_upper_bound: float = 1.0
     plot_legend_name: str = "Label"
 
@@ -528,14 +531,15 @@
         >>> preds = tensor([[[0.59, 0.91], [0.91, 0.99],  [0.63, 0.04]],
         ...                 [[0.38, 0.04], [0.86, 0.780], [0.45, 0.37]]])
         >>> metric = BinaryRecall(multidim_average='samplewise')
         >>> metric(preds, target)
         tensor([0.6667, 0.0000])
 
     """
+
     is_differentiable: bool = False
     higher_is_better: Optional[bool] = True
     full_state_update: bool = False
     plot_lower_bound: float = 0.0
     plot_upper_bound: float = 1.0
 
     def compute(self) -> Tensor:
@@ -682,26 +686,27 @@
         tensor([0.5000, 0.2778])
         >>> mcr = MulticlassRecall(num_classes=3, multidim_average='samplewise', average=None)
         >>> mcr(preds, target)
         tensor([[1.0000, 0.0000, 0.5000],
                 [0.0000, 0.3333, 0.5000]])
 
     """
+
     is_differentiable: bool = False
     higher_is_better: Optional[bool] = True
     full_state_update: bool = False
     plot_lower_bound: float = 0.0
     plot_upper_bound: float = 1.0
     plot_legend_name: str = "Class"
 
     def compute(self) -> Tensor:
         """Compute metric."""
         tp, fp, tn, fn = self._final_state()
         return _precision_recall_reduce(
-            "recall", tp, fp, tn, fn, average=self.average, multidim_average=self.multidim_average
+            "recall", tp, fp, tn, fn, average=self.average, multidim_average=self.multidim_average, top_k=self.top_k
         )
 
     def plot(
         self, val: Optional[Union[Tensor, Sequence[Tensor]]] = None, ax: Optional[_AX_TYPE] = None
     ) -> _PLOT_OUT_TYPE:
         """Plot a single or multiple values from the metric.
 
@@ -834,14 +839,15 @@
         tensor([0.6667, 0.0000])
         >>> mlr = MultilabelRecall(num_labels=3, multidim_average='samplewise', average=None)
         >>> mlr(preds, target)
         tensor([[1., 1., 0.],
                 [0., 0., 0.]])
 
     """
+
     is_differentiable: bool = False
     higher_is_better: Optional[bool] = True
     full_state_update: bool = False
     plot_lower_bound: float = 0.0
     plot_upper_bound: float = 1.0
     plot_legend_name: str = "Label"
 
@@ -935,17 +941,19 @@
         top_k: Optional[int] = 1,
         ignore_index: Optional[int] = None,
         validate_args: bool = True,
         **kwargs: Any,
     ) -> Metric:
         """Initialize task metric."""
         assert multidim_average is not None  # noqa: S101  # needed for mypy
-        kwargs.update(
-            {"multidim_average": multidim_average, "ignore_index": ignore_index, "validate_args": validate_args}
-        )
+        kwargs.update({
+            "multidim_average": multidim_average,
+            "ignore_index": ignore_index,
+            "validate_args": validate_args,
+        })
         task = ClassificationTask.from_str(task)
         if task == ClassificationTask.BINARY:
             return BinaryPrecision(threshold, **kwargs)
         if task == ClassificationTask.MULTICLASS:
             if not isinstance(num_classes, int):
                 raise ValueError(f"`num_classes` is expected to be `int` but `{type(num_classes)} was passed.`")
             if not isinstance(top_k, int):
@@ -999,17 +1007,19 @@
         ignore_index: Optional[int] = None,
         validate_args: bool = True,
         **kwargs: Any,
     ) -> Metric:
         """Initialize task metric."""
         task = ClassificationTask.from_str(task)
         assert multidim_average is not None  # noqa: S101  # needed for mypy
-        kwargs.update(
-            {"multidim_average": multidim_average, "ignore_index": ignore_index, "validate_args": validate_args}
-        )
+        kwargs.update({
+            "multidim_average": multidim_average,
+            "ignore_index": ignore_index,
+            "validate_args": validate_args,
+        })
         if task == ClassificationTask.BINARY:
             return BinaryRecall(threshold, **kwargs)
         if task == ClassificationTask.MULTICLASS:
             if not isinstance(num_classes, int):
                 raise ValueError(f"`num_classes` is expected to be `int` but `{type(num_classes)} was passed.`")
             if not isinstance(top_k, int):
                 raise ValueError(f"`top_k` is expected to be `int` but `{type(top_k)} was passed.`")
```

### Comparing `torchmetrics-1.3.1/src/torchmetrics/classification/precision_recall_curve.py` & `torchmetrics-1.3.2/src/torchmetrics/classification/precision_recall_curve.py`

 * *Files 2% similar despite different names*

```diff
@@ -121,14 +121,15 @@
         >>> bprc = BinaryPrecisionRecallCurve(thresholds=5)
         >>> bprc(preds, target)  # doctest: +NORMALIZE_WHITESPACE
         (tensor([0.5000, 0.6667, 0.6667, 0.0000, 0.0000, 1.0000]),
          tensor([1., 1., 1., 0., 0., 0.]),
          tensor([0.0000, 0.2500, 0.5000, 0.7500, 1.0000]))
 
     """
+
     is_differentiable: bool = False
     higher_is_better: Optional[bool] = None
     full_state_update: bool = False
 
     preds: List[Tensor]
     target: List[Tensor]
     confmat: Tensor
@@ -183,15 +184,16 @@
     ) -> _PLOT_OUT_TYPE:
         """Plot a single curve from the metric.
 
         Args:
             curve: the output of either `metric.compute` or `metric.forward`. If no value is provided, will
                 automatically call `metric.compute` and plot that result.
             score: Provide a area-under-the-curve score to be displayed on the plot. If `True` and no curve is provided,
-                will automatically compute the score.
+                will automatically compute the score. The score is computed by using the trapezoidal rule to compute the
+                area under the curve.
             ax: An matplotlib axis object. If provided will add plot to that axis
 
         Returns:
             Figure and Axes object
 
         Raises:
             ModuleNotFoundError:
@@ -210,15 +212,15 @@
 
         """
         curve_computed = curve or self.compute()
         # switch order as the standard way is recall along x-axis and precision along y-axis
         curve_computed = (curve_computed[1], curve_computed[0], curve_computed[2])
 
         score = (
-            _auc_compute_without_check(curve_computed[0], curve_computed[1], 1.0)
+            _auc_compute_without_check(curve_computed[0], curve_computed[1], direction=-1.0)
             if not curve and score is True
             else None
         )
         return plot_curve(
             curve_computed, score=score, ax=ax, label_names=("Recall", "Precision"), name=self.__class__.__name__
         )
 
@@ -312,14 +314,15 @@
                  [1., 1., 1., 1., 0., 0.],
                  [1., 0., 0., 0., 0., 0.],
                  [1., 0., 0., 0., 0., 0.],
                  [0., 0., 0., 0., 0., 0.]]),
          tensor([0.0000, 0.2500, 0.5000, 0.7500, 1.0000]))
 
     """
+
     is_differentiable: bool = False
     higher_is_better: Optional[bool] = None
     full_state_update: bool = False
 
     preds: List[Tensor]
     target: List[Tensor]
     confmat: Tensor
@@ -384,15 +387,16 @@
     ) -> _PLOT_OUT_TYPE:
         """Plot a single or multiple values from the metric.
 
         Args:
             curve: the output of either `metric.compute` or `metric.forward`. If no value is provided, will
                 automatically call `metric.compute` and plot that result.
             score: Provide a area-under-the-curve score to be displayed on the plot. If `True` and no curve is provided,
-                will automatically compute the score.
+                will automatically compute the score. The score is computed by using the trapezoidal rule to compute the
+                area under the curve.
             ax: An matplotlib axis object. If provided will add plot to that axis
 
         Returns:
             Figure and Axes object
 
         Raises:
             ModuleNotFoundError:
@@ -410,15 +414,17 @@
             >>> fig_, ax_ = metric.plot(score=True)
 
         """
         curve_computed = curve or self.compute()
         # switch order as the standard way is recall along x-axis and precision along y-axis
         curve_computed = (curve_computed[1], curve_computed[0], curve_computed[2])
         score = (
-            _reduce_auroc(curve_computed[0], curve_computed[1], average=None) if not curve and score is True else None
+            _reduce_auroc(curve_computed[0], curve_computed[1], average=None, direction=-1.0)
+            if not curve and score is True
+            else None
         )
         return plot_curve(
             curve_computed, score=score, ax=ax, label_names=("Recall", "Precision"), name=self.__class__.__name__
         )
 
 
 class MultilabelPrecisionRecallCurve(Metric):
@@ -508,14 +514,15 @@
                  [0.7500, 1.0000, 1.0000, 1.0000, 0.0000, 1.0000]]),
          tensor([[1.0000, 0.5000, 0.5000, 0.5000, 0.0000, 0.0000],
                  [1.0000, 1.0000, 1.0000, 0.0000, 0.0000, 0.0000],
                  [1.0000, 0.6667, 0.3333, 0.3333, 0.0000, 0.0000]]),
          tensor([0.0000, 0.2500, 0.5000, 0.7500, 1.0000]))
 
     """
+
     is_differentiable: bool = False
     higher_is_better: Optional[bool] = None
     full_state_update: bool = False
 
     preds: List[Tensor]
     target: List[Tensor]
     confmat: Tensor
@@ -576,15 +583,16 @@
     ) -> _PLOT_OUT_TYPE:
         """Plot a single or multiple values from the metric.
 
         Args:
             curve: the output of either `metric.compute` or `metric.forward`. If no value is provided, will
                 automatically call `metric.compute` and plot that result.
             score: Provide a area-under-the-curve score to be displayed on the plot. If `True` and no curve is provided,
-                will automatically compute the score.
+                will automatically compute the score. The score is computed by using the trapezoidal rule to compute the
+                area under the curve.
             ax: An matplotlib axis object. If provided will add plot to that axis
 
         Returns:
             Figure and Axes object
 
         Raises:
             ModuleNotFoundError:
@@ -602,15 +610,17 @@
             >>> fig_, ax_ = metric.plot(score=True)
 
         """
         curve_computed = curve or self.compute()
         # switch order as the standard way is recall along x-axis and precision along y-axis
         curve_computed = (curve_computed[1], curve_computed[0], curve_computed[2])
         score = (
-            _reduce_auroc(curve_computed[0], curve_computed[1], average=None) if not curve and score is True else None
+            _reduce_auroc(curve_computed[0], curve_computed[1], average=None, direction=-1.0)
+            if not curve and score is True
+            else None
         )
         return plot_curve(
             curve_computed, score=score, ax=ax, label_names=("Recall", "Precision"), name=self.__class__.__name__
         )
 
 
 class PrecisionRecallCurve(_ClassificationTaskWrapper):
```

### Comparing `torchmetrics-1.3.1/src/torchmetrics/classification/ranking.py` & `torchmetrics-1.3.2/src/torchmetrics/classification/ranking.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.3.1/src/torchmetrics/classification/recall_fixed_precision.py` & `torchmetrics-1.3.2/src/torchmetrics/classification/recall_fixed_precision.py`

 * *Files 0% similar despite different names*

```diff
@@ -100,14 +100,15 @@
         >>> metric(preds, target)
         (tensor(1.), tensor(0.5000))
         >>> metric = BinaryRecallAtFixedPrecision(min_precision=0.5, thresholds=5)
         >>> metric(preds, target)
         (tensor(1.), tensor(0.5000))
 
     """
+
     is_differentiable: bool = False
     higher_is_better: Optional[bool] = None
     full_state_update: bool = False
     plot_lower_bound: float = 0.0
     plot_upper_bound: float = 1.0
 
     def __init__(
@@ -240,14 +241,15 @@
         >>> metric(preds, target)
         (tensor([1., 1., 0., 0., 0.]), tensor([7.5000e-01, 7.5000e-01, 1.0000e+06, 1.0000e+06, 1.0000e+06]))
         >>> mcrafp = MulticlassRecallAtFixedPrecision(num_classes=5, min_precision=0.5, thresholds=5)
         >>> mcrafp(preds, target)
         (tensor([1., 1., 0., 0., 0.]), tensor([7.5000e-01, 7.5000e-01, 1.0000e+06, 1.0000e+06, 1.0000e+06]))
 
     """
+
     is_differentiable: bool = False
     higher_is_better: Optional[bool] = None
     full_state_update: bool = False
     plot_lower_bound: float = 0.0
     plot_upper_bound: float = 1.0
     plot_legend_name: str = "Class"
 
@@ -385,14 +387,15 @@
         >>> metric(preds, target)
         (tensor([1., 1., 1.]), tensor([0.0500, 0.5500, 0.0500]))
         >>> mlrafp = MultilabelRecallAtFixedPrecision(num_labels=3, min_precision=0.5, thresholds=5)
         >>> mlrafp(preds, target)
         (tensor([1., 1., 1.]), tensor([0.0000, 0.5000, 0.0000]))
 
     """
+
     is_differentiable: bool = False
     higher_is_better: Optional[bool] = None
     full_state_update: bool = False
     plot_lower_bound: float = 0.0
     plot_upper_bound: float = 1.0
     plot_legend_name: str = "Label"
```

### Comparing `torchmetrics-1.3.1/src/torchmetrics/classification/roc.py` & `torchmetrics-1.3.2/src/torchmetrics/classification/roc.py`

 * *Files 2% similar despite different names*

```diff
@@ -106,14 +106,15 @@
         >>> broc = BinaryROC(thresholds=5)
         >>> broc(preds, target)  # doctest: +NORMALIZE_WHITESPACE
         (tensor([0.0000, 0.5000, 0.5000, 0.5000, 1.0000]),
          tensor([0., 0., 1., 1., 1.]),
          tensor([1.0000, 0.7500, 0.5000, 0.2500, 0.0000]))
 
     """
+
     is_differentiable: bool = False
     higher_is_better: Optional[bool] = None
     full_state_update: bool = False
     plot_lower_bound: float = 0.0
     plot_upper_bound: float = 1.0
 
     def compute(self) -> Tuple[Tensor, Tensor, Tensor]:
@@ -129,15 +130,16 @@
     ) -> _PLOT_OUT_TYPE:
         """Plot a single or multiple values from the metric.
 
         Args:
             curve: the output of either `metric.compute` or `metric.forward`. If no value is provided, will
                 automatically call `metric.compute` and plot that result.
             score: Provide a area-under-the-curve score to be displayed on the plot. If `True` and no curve is provided,
-                will automatically compute the score.
+                will automatically compute the score. The score is computed by using the trapezoidal rule to compute the
+                area under the curve.
             ax: An matplotlib axis object. If provided will add plot to that axis
 
         Returns:
             Figure and Axes object
 
         Raises:
             ModuleNotFoundError:
@@ -273,14 +275,15 @@
                  [0., 1., 1., 1., 1.],
                  [0., 0., 0., 0., 1.],
                  [0., 0., 0., 0., 1.],
                  [0., 0., 0., 0., 0.]]),
          tensor([1.0000, 0.7500, 0.5000, 0.2500, 0.0000]))
 
     """
+
     is_differentiable: bool = False
     higher_is_better: Optional[bool] = None
     full_state_update: bool = False
     plot_lower_bound: float = 0.0
     plot_upper_bound: float = 1.0
     plot_legend_name: str = "Class"
 
@@ -297,15 +300,16 @@
     ) -> _PLOT_OUT_TYPE:
         """Plot a single or multiple values from the metric.
 
         Args:
             curve: the output of either `metric.compute` or `metric.forward`. If no value is provided, will
                 automatically call `metric.compute` and plot that result.
             score: Provide a area-under-the-curve score to be displayed on the plot. If `True` and no curve is provided,
-                will automatically compute the score.
+                will automatically compute the score. The score is computed by using the trapezoidal rule to compute the
+                area under the curve.
             ax: An matplotlib axis object. If provided will add plot to that axis
 
         Returns:
             Figure and Axes object
 
         Raises:
             ModuleNotFoundError:
@@ -430,14 +434,15 @@
                  [0.0000, 0.0000, 0.0000, 0.0000, 1.0000]]),
          tensor([[0.0000, 0.5000, 0.5000, 0.5000, 1.0000],
                  [0.0000, 0.0000, 1.0000, 1.0000, 1.0000],
                  [0.0000, 0.3333, 0.3333, 0.6667, 1.0000]]),
          tensor([1.0000, 0.7500, 0.5000, 0.2500, 0.0000]))
 
     """
+
     is_differentiable: bool = False
     higher_is_better: Optional[bool] = None
     full_state_update: bool = False
     plot_lower_bound: float = 0.0
     plot_upper_bound: float = 1.0
     plot_legend_name: str = "Label"
 
@@ -454,15 +459,16 @@
     ) -> _PLOT_OUT_TYPE:
         """Plot a single or multiple values from the metric.
 
         Args:
             curve: the output of either `metric.compute` or `metric.forward`. If no value is provided, will
                 automatically call `metric.compute` and plot that result.
             score: Provide a area-under-the-curve score to be displayed on the plot. If `True` and no curve is provided,
-                will automatically compute the score.
+                will automatically compute the score. The score is computed by using the trapezoidal rule to compute the
+                area under the curve.
             ax: An matplotlib axis object. If provided will add plot to that axis
 
         Returns:
             Figure and Axes object
 
         Raises:
             ModuleNotFoundError:
```

### Comparing `torchmetrics-1.3.1/src/torchmetrics/classification/specificity.py` & `torchmetrics-1.3.2/src/torchmetrics/classification/specificity.py`

 * *Files 0% similar despite different names*

```diff
@@ -90,14 +90,15 @@
         >>> preds = tensor([[[0.59, 0.91], [0.91, 0.99],  [0.63, 0.04]],
         ...                 [[0.38, 0.04], [0.86, 0.780], [0.45, 0.37]]])
         >>> metric = BinarySpecificity(multidim_average='samplewise')
         >>> metric(preds, target)
         tensor([0.0000, 0.3333])
 
     """
+
     plot_lower_bound: float = 0.0
     plot_upper_bound: float = 1.0
 
     def compute(self) -> Tensor:
         """Compute metric."""
         tp, fp, tn, fn = self._final_state()
         return _specificity_reduce(tp, fp, tn, fn, average="binary", multidim_average=self.multidim_average)
@@ -240,14 +241,15 @@
         tensor([0.7500, 0.6556])
         >>> mcs = MulticlassSpecificity(num_classes=3, multidim_average='samplewise', average=None)
         >>> mcs(preds, target)
         tensor([[0.7500, 0.7500, 0.7500],
                 [0.8000, 0.6667, 0.5000]])
 
     """
+
     plot_lower_bound: float = 0.0
     plot_upper_bound: float = 1.0
     plot_legend_name: str = "Class"
 
     def compute(self) -> Tensor:
         """Compute metric."""
         tp, fp, tn, fn = self._final_state()
@@ -386,14 +388,15 @@
         tensor([0.0000, 0.3333])
         >>> mls = MultilabelSpecificity(num_labels=3, multidim_average='samplewise', average=None)
         >>> mls(preds, target)
         tensor([[0., 0., 0.],
                 [0., 0., 1.]])
 
     """
+
     plot_lower_bound: float = 0.0
     plot_upper_bound: float = 1.0
     plot_legend_name: str = "Label"
 
     def compute(self) -> Tensor:
         """Compute metric."""
         tp, fp, tn, fn = self._final_state()
@@ -485,17 +488,19 @@
         ignore_index: Optional[int] = None,
         validate_args: bool = True,
         **kwargs: Any,
     ) -> Metric:
         """Initialize task metric."""
         task = ClassificationTask.from_str(task)
         assert multidim_average is not None  # noqa: S101  # needed for mypy
-        kwargs.update(
-            {"multidim_average": multidim_average, "ignore_index": ignore_index, "validate_args": validate_args}
-        )
+        kwargs.update({
+            "multidim_average": multidim_average,
+            "ignore_index": ignore_index,
+            "validate_args": validate_args,
+        })
         if task == ClassificationTask.BINARY:
             return BinarySpecificity(threshold, **kwargs)
         if task == ClassificationTask.MULTICLASS:
             if not isinstance(num_classes, int):
                 raise ValueError(f"`num_classes` is expected to be `int` but `{type(num_classes)} was passed.`")
             if not isinstance(top_k, int):
                 raise ValueError(f"`top_k` is expected to be `int` but `{type(top_k)} was passed.`")
```

### Comparing `torchmetrics-1.3.1/src/torchmetrics/classification/specificity_sensitivity.py` & `torchmetrics-1.3.2/src/torchmetrics/classification/specificity_sensitivity.py`

 * *Files 0% similar despite different names*

```diff
@@ -97,14 +97,15 @@
         >>> metric(preds, target)
         (tensor(1.), tensor(0.4000))
         >>> metric = BinarySpecificityAtSensitivity(min_sensitivity=0.5, thresholds=5)
         >>> metric(preds, target)
         (tensor(1.), tensor(0.2500))
 
     """
+
     is_differentiable: bool = False
     higher_is_better: Optional[bool] = None
     full_state_update: bool = False
     plot_lower_bound: float = 0.0
     plot_upper_bound: float = 1.0
 
     def __init__(
@@ -191,14 +192,15 @@
         >>> metric(preds, target)
         (tensor([1., 1., 0., 0., 0.]), tensor([7.5000e-01, 7.5000e-01, 5.0000e-02, 5.0000e-02, 1.0000e+06]))
         >>> metric = MulticlassSpecificityAtSensitivity(num_classes=5, min_sensitivity=0.5, thresholds=5)
         >>> metric(preds, target)
         (tensor([1., 1., 0., 0., 0.]), tensor([7.5000e-01, 7.5000e-01, 0.0000e+00, 0.0000e+00, 1.0000e+06]))
 
     """
+
     is_differentiable: bool = False
     higher_is_better: Optional[bool] = None
     full_state_update: bool = False
     plot_lower_bound: float = 0.0
     plot_upper_bound: float = 1.0
     plot_legend_name: str = "Class"
 
@@ -291,14 +293,15 @@
         >>> metric(preds, target)
         (tensor([1.0000, 0.5000, 1.0000]), tensor([0.7500, 0.6500, 0.3500]))
         >>> metric = MultilabelSpecificityAtSensitivity(num_labels=3, min_sensitivity=0.5, thresholds=5)
         >>> metric(preds, target)
         (tensor([1.0000, 0.5000, 1.0000]), tensor([0.7500, 0.5000, 0.2500]))
 
     """
+
     is_differentiable: bool = False
     higher_is_better: Optional[bool] = None
     full_state_update: bool = False
     plot_lower_bound: float = 0.0
     plot_upper_bound: float = 1.0
     plot_legend_name: str = "Label"
```

### Comparing `torchmetrics-1.3.1/src/torchmetrics/classification/stat_scores.py` & `torchmetrics-1.3.2/src/torchmetrics/classification/stat_scores.py`

 * *Files 1% similar despite different names*

```diff
@@ -152,14 +152,15 @@
         ...                 [[0.38, 0.04], [0.86, 0.780], [0.45, 0.37]]])
         >>> metric = BinaryStatScores(multidim_average='samplewise')
         >>> metric(preds, target)
         tensor([[2, 3, 0, 1, 3],
                 [0, 2, 1, 3, 3]])
 
     """
+
     is_differentiable: bool = False
     higher_is_better: Optional[bool] = None
     full_state_update: bool = False
 
     def __init__(
         self,
         threshold: float = 0.5,
@@ -293,14 +294,15 @@
                  [0, 1, 3, 2, 2],
                  [1, 1, 3, 1, 2]],
                 [[0, 1, 4, 1, 1],
                  [1, 1, 2, 2, 3],
                  [1, 2, 2, 1, 2]]])
 
     """
+
     is_differentiable: bool = False
     higher_is_better: Optional[bool] = None
     full_state_update: bool = False
 
     def __init__(
         self,
         num_classes: int,
@@ -440,14 +442,15 @@
                  [1, 1, 0, 0, 1],
                  [0, 1, 0, 1, 1]],
                 [[0, 0, 0, 2, 2],
                  [0, 2, 0, 0, 0],
                  [0, 0, 1, 1, 1]]])
 
     """
+
     is_differentiable: bool = False
     higher_is_better: Optional[bool] = None
     full_state_update: bool = False
 
     def __init__(
         self,
         num_labels: int,
@@ -524,17 +527,19 @@
         ignore_index: Optional[int] = None,
         validate_args: bool = True,
         **kwargs: Any,
     ) -> Metric:
         """Initialize task metric."""
         task = ClassificationTask.from_str(task)
         assert multidim_average is not None  # noqa: S101  # needed for mypy
-        kwargs.update(
-            {"multidim_average": multidim_average, "ignore_index": ignore_index, "validate_args": validate_args}
-        )
+        kwargs.update({
+            "multidim_average": multidim_average,
+            "ignore_index": ignore_index,
+            "validate_args": validate_args,
+        })
         if task == ClassificationTask.BINARY:
             return BinaryStatScores(threshold, **kwargs)
         if task == ClassificationTask.MULTICLASS:
             if not isinstance(num_classes, int):
                 raise ValueError(f"`num_classes` is expected to be `int` but `{type(num_classes)} was passed.`")
             if not isinstance(top_k, int):
                 raise ValueError(f"`top_k` is expected to be `int` but `{type(top_k)} was passed.`")
```

### Comparing `torchmetrics-1.3.1/src/torchmetrics/clustering/__init__.py` & `torchmetrics-1.3.2/src/torchmetrics/clustering/__init__.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.3.1/src/torchmetrics/clustering/adjusted_mutual_info_score.py` & `torchmetrics-1.3.2/src/torchmetrics/clustering/adjusted_mutual_info_score.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.3.1/src/torchmetrics/clustering/adjusted_rand_score.py` & `torchmetrics-1.3.2/src/torchmetrics/clustering/adjusted_rand_score.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.3.1/src/torchmetrics/clustering/calinski_harabasz_score.py` & `torchmetrics-1.3.2/src/torchmetrics/clustering/calinski_harabasz_score.py`

 * *Files 0% similar despite different names*

```diff
@@ -60,14 +60,15 @@
         >>> data = torch.randn(10, 3)
         >>> labels = torch.randint(3, (10,))
         >>> metric = CalinskiHarabaszScore()
         >>> metric(data, labels)
         tensor(3.0053)
 
     """
+
     is_differentiable: bool = True
     higher_is_better: bool = True
     full_state_update: bool = False
     plot_lower_bound: float = 0.0
     data: List[Tensor]
     labels: List[Tensor]
```

### Comparing `torchmetrics-1.3.1/src/torchmetrics/clustering/davies_bouldin_score.py` & `torchmetrics-1.3.2/src/torchmetrics/clustering/davies_bouldin_score.py`

 * *Files 0% similar despite different names*

```diff
@@ -70,14 +70,15 @@
         >>> data = torch.randn(10, 3)
         >>> labels = torch.randint(3, (10,))
         >>> metric = DaviesBouldinScore()
         >>> metric(data, labels)
         tensor(1.2540)
 
     """
+
     is_differentiable: bool = True
     higher_is_better: bool = True
     full_state_update: bool = False
     plot_lower_bound: float = 0.0
     data: List[Tensor]
     labels: List[Tensor]
```

### Comparing `torchmetrics-1.3.1/src/torchmetrics/clustering/dunn_index.py` & `torchmetrics-1.3.2/src/torchmetrics/clustering/dunn_index.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.3.1/src/torchmetrics/clustering/fowlkes_mallows_index.py` & `torchmetrics-1.3.2/src/torchmetrics/clustering/fowlkes_mallows_index.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.3.1/src/torchmetrics/clustering/homogeneity_completeness_v_measure.py` & `torchmetrics-1.3.2/src/torchmetrics/clustering/homogeneity_completeness_v_measure.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.3.1/src/torchmetrics/clustering/mutual_info_score.py` & `torchmetrics-1.3.2/src/torchmetrics/clustering/mutual_info_score.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.3.1/src/torchmetrics/clustering/normalized_mutual_info_score.py` & `torchmetrics-1.3.2/src/torchmetrics/clustering/normalized_mutual_info_score.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.3.1/src/torchmetrics/clustering/rand_score.py` & `torchmetrics-1.3.2/src/torchmetrics/clustering/rand_score.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.3.1/src/torchmetrics/collections.py` & `torchmetrics-1.3.2/src/torchmetrics/collections.py`

 * *Files 0% similar despite different names*

```diff
@@ -643,19 +643,18 @@
             if not together and not (
                 isinstance(ax, Sequence) and all(isinstance(a, _AX_TYPE) for a in ax) and len(ax) == len(self)
             ):
                 raise ValueError(
                     f"Expected argument `ax` to be a sequence of matplotlib axis objects with the same length as the "
                     f"number of metrics in the collection, but got {type(ax)} with len {len(ax)} when `together=False`"
                 )
-
         val = val or self.compute()
         if together:
             return plot_single_or_multi_val(val, ax=ax)
         fig_axs = []
-        for i, (k, m) in enumerate(self.items(keep_base=True, copy_state=False)):
+        for i, (k, m) in enumerate(self.items(keep_base=False, copy_state=False)):
             if isinstance(val, dict):
                 f, a = m.plot(val[k], ax=ax[i] if ax is not None else ax)
             elif isinstance(val, Sequence):
                 f, a = m.plot([v[k] for v in val], ax=ax[i] if ax is not None else ax)
             fig_axs.append((f, a))
         return fig_axs
```

### Comparing `torchmetrics-1.3.1/src/torchmetrics/detection/__init__.py` & `torchmetrics-1.3.2/src/torchmetrics/detection/__init__.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.3.1/src/torchmetrics/detection/_deprecated.py` & `torchmetrics-1.3.2/src/torchmetrics/detection/_deprecated.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.3.1/src/torchmetrics/detection/_mean_ap.py` & `torchmetrics-1.3.2/src/torchmetrics/detection/_mean_ap.py`

 * *Files 0% similar despite different names*

```diff
@@ -294,14 +294,15 @@
          'mar_100': tensor(0.6000),
          'mar_100_per_class': tensor(-1.),
          'mar_large': tensor(0.6000),
          'mar_medium': tensor(-1.),
          'mar_small': tensor(-1.)}
 
     """
+
     is_differentiable: bool = False
     higher_is_better: Optional[bool] = True
     full_state_update: bool = True
     plot_lower_bound: float = 0.0
     plot_upper_bound: float = 1.0
 
     detections: List[Tensor]
```

### Comparing `torchmetrics-1.3.1/src/torchmetrics/detection/ciou.py` & `torchmetrics-1.3.2/src/torchmetrics/detection/ciou.py`

 * *Files 0% similar despite different names*

```diff
@@ -90,14 +90,15 @@
         {'ciou': tensor(0.8611)}
 
     Raises:
         ModuleNotFoundError:
             If torchvision is not installed with version 0.13.0 or newer.
 
     """
+
     is_differentiable: bool = False
     higher_is_better: Optional[bool] = True
     full_state_update: bool = True
 
     _iou_type: str = "ciou"
     _invalid_val: float = -2.0  # unsure, min val could be just -1.5 as well
```

### Comparing `torchmetrics-1.3.1/src/torchmetrics/detection/diou.py` & `torchmetrics-1.3.2/src/torchmetrics/detection/diou.py`

 * *Files 0% similar despite different names*

```diff
@@ -90,14 +90,15 @@
         {'diou': tensor(0.8611)}
 
     Raises:
         ModuleNotFoundError:
             If torchvision is not installed with version 0.13.0 or newer.
 
     """
+
     is_differentiable: bool = False
     higher_is_better: Optional[bool] = True
     full_state_update: bool = True
 
     _iou_type: str = "diou"
     _invalid_val: float = -1.0
```

### Comparing `torchmetrics-1.3.1/src/torchmetrics/detection/giou.py` & `torchmetrics-1.3.2/src/torchmetrics/detection/giou.py`

 * *Files 0% similar despite different names*

```diff
@@ -90,14 +90,15 @@
         {'giou': tensor(0.8613)}
 
     Raises:
         ModuleNotFoundError:
             If torchvision is not installed with version 0.8.0 or newer.
 
     """
+
     is_differentiable: bool = False
     higher_is_better: Optional[bool] = True
     full_state_update: bool = True
 
     _iou_type: str = "giou"
     _invalid_val: float = -1.0
```

### Comparing `torchmetrics-1.3.1/src/torchmetrics/detection/helpers.py` & `torchmetrics-1.3.2/src/torchmetrics/detection/helpers.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.3.1/src/torchmetrics/detection/iou.py` & `torchmetrics-1.3.2/src/torchmetrics/detection/iou.py`

 * *Files 0% similar despite different names*

```diff
@@ -122,14 +122,15 @@
         {'iou': tensor(0.7756), 'iou/cl_4': tensor(0.6898), 'iou/cl_5': tensor(0.8614)}
 
     Raises:
         ModuleNotFoundError:
             If torchvision is not installed with version 0.8.0 or newer.
 
     """
+
     is_differentiable: bool = False
     higher_is_better: Optional[bool] = True
     full_state_update: bool = True
 
     groundtruth_labels: List[Tensor]
     iou_matrix: List[Tensor]
     _iou_type: str = "iou"
```

### Comparing `torchmetrics-1.3.1/src/torchmetrics/detection/mean_ap.py` & `torchmetrics-1.3.2/src/torchmetrics/detection/mean_ap.py`

 * *Files 0% similar despite different names*

```diff
@@ -325,14 +325,15 @@
          'mar_100': tensor(0.2000),
          'mar_100_per_class': tensor(-1.),
          'mar_large': tensor(-1.),
          'mar_medium': tensor(-1.),
          'mar_small': tensor(0.2000)}
 
     """
+
     is_differentiable: bool = False
     higher_is_better: Optional[bool] = True
     full_state_update: bool = True
     plot_lower_bound: float = 0.0
     plot_upper_bound: float = 1.0
 
     detection_box: List[Tensor]
```

### Comparing `torchmetrics-1.3.1/src/torchmetrics/detection/panoptic_qualities.py` & `torchmetrics-1.3.2/src/torchmetrics/detection/panoptic_qualities.py`

 * *Files 0% similar despite different names*

```diff
@@ -77,14 +77,15 @@
         ...                   [[0, 1], [7, 0], [1, 0], [1, 0]],
         ...                   [[0, 1], [7, 0], [7, 0], [7, 0]]]])
         >>> panoptic_quality = PanopticQuality(things = {0, 1}, stuffs = {6, 7})
         >>> panoptic_quality(preds, target)
         tensor(0.5463, dtype=torch.float64)
 
     """
+
     is_differentiable: bool = False
     higher_is_better: bool = True
     full_state_update: bool = False
     plot_lower_bound: float = 0.0
     plot_upper_bound: float = 1.0
 
     iou_sum: Tensor
@@ -255,14 +256,15 @@
         >>> preds = tensor([[[0, 0], [0, 1], [6, 0], [7, 0], [0, 2], [1, 0]]])
         >>> target = tensor([[[0, 1], [0, 0], [6, 0], [7, 0], [6, 0], [255, 0]]])
         >>> pq_modified = ModifiedPanopticQuality(things = {0, 1}, stuffs = {6, 7})
         >>> pq_modified(preds, target)
         tensor(0.7667, dtype=torch.float64)
 
     """
+
     is_differentiable: bool = False
     higher_is_better: bool = True
     full_state_update: bool = False
     plot_lower_bound: float = 0.0
     plot_upper_bound: float = 1.0
 
     iou_sum: Tensor
```

### Comparing `torchmetrics-1.3.1/src/torchmetrics/functional/__init__.py` & `torchmetrics-1.3.2/src/torchmetrics/functional/__init__.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.3.1/src/torchmetrics/functional/audio/__init__.py` & `torchmetrics-1.3.2/src/torchmetrics/functional/audio/__init__.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.3.1/src/torchmetrics/functional/audio/_deprecated.py` & `torchmetrics-1.3.2/src/torchmetrics/functional/audio/_deprecated.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 def _permutation_invariant_training(
     preds: Tensor,
     target: Tensor,
     metric_func: Callable,
     mode: Literal["speaker-wise", "permutation-wise"] = "speaker-wise",
     eval_func: Literal["max", "min"] = "max",
-    **kwargs: Any
+    **kwargs: Any,
 ) -> Tuple[Tensor, Tensor]:
     """Wrapper for deprecated import.
 
     >>> from torch import tensor
     >>> preds = tensor([[[-0.0579,  0.3560, -0.9604], [-0.1719,  0.3205,  0.2951]]])
     >>> target = tensor([[[ 1.0958, -0.1648,  0.5228], [-0.4100,  1.1942, -0.5103]]])
     >>> best_metric, best_perm = _permutation_invariant_training(
```

### Comparing `torchmetrics-1.3.1/src/torchmetrics/functional/audio/pesq.py` & `torchmetrics-1.3.2/src/torchmetrics/functional/audio/pesq.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.3.1/src/torchmetrics/functional/audio/pit.py` & `torchmetrics-1.3.2/src/torchmetrics/functional/audio/pit.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.3.1/src/torchmetrics/functional/audio/sdr.py` & `torchmetrics-1.3.2/src/torchmetrics/functional/audio/sdr.py`

 * *Files 0% similar despite different names*

```diff
@@ -226,17 +226,15 @@
     _check_same_shape(preds, target)
     eps = torch.finfo(preds.dtype).eps
 
     if zero_mean:
         target = target - torch.mean(target, dim=-1, keepdim=True)
         preds = preds - torch.mean(preds, dim=-1, keepdim=True)
 
-    alpha = (torch.sum(preds * target, dim=-1, keepdim=True) + eps) / (
-        torch.sum(target**2, dim=-1, keepdim=True) + eps
-    )
+    alpha = (torch.sum(preds * target, dim=-1, keepdim=True) + eps) / (torch.sum(target**2, dim=-1, keepdim=True) + eps)
     target_scaled = alpha * target
 
     noise = target_scaled - preds
 
     val = (torch.sum(target_scaled**2, dim=-1) + eps) / (torch.sum(noise**2, dim=-1) + eps)
     return 10 * torch.log10(val)
```

### Comparing `torchmetrics-1.3.1/src/torchmetrics/functional/audio/snr.py` & `torchmetrics-1.3.2/src/torchmetrics/functional/audio/snr.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.3.1/src/torchmetrics/functional/audio/srmr.py` & `torchmetrics-1.3.2/src/torchmetrics/functional/audio/srmr.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.3.1/src/torchmetrics/functional/audio/stoi.py` & `torchmetrics-1.3.2/src/torchmetrics/functional/audio/stoi.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.3.1/src/torchmetrics/functional/classification/__init__.py` & `torchmetrics-1.3.2/src/torchmetrics/functional/classification/__init__.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.3.1/src/torchmetrics/functional/classification/accuracy.py` & `torchmetrics-1.3.2/src/torchmetrics/functional/classification/accuracy.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,14 +38,15 @@
     tp: Tensor,
     fp: Tensor,
     tn: Tensor,
     fn: Tensor,
     average: Optional[Literal["binary", "micro", "macro", "weighted", "none"]],
     multidim_average: Literal["global", "samplewise"] = "global",
     multilabel: bool = False,
+    top_k: int = 1,
 ) -> Tensor:
     """Reduce classification statistics into accuracy score.
 
     Args:
         tp: number of true positives
         fp: number of false positives
         tn: number of true negatives
@@ -62,14 +63,15 @@
         multidim_average:
             Defines how additionally dimensions ``...`` should be handled. Should be one of the following:
 
             - ``global``: Additional dimensions are flatted along the batch dimension
             - ``samplewise``: Statistic will be calculated independently for each sample on the ``N`` axis.
 
         multilabel: If input is multilabel or not
+        top_k: value for top-k accuracy, else 1
 
     Returns:
         Accuracy score
 
     """
     if average == "binary":
         return _safe_divide(tp + tn, tp + tn + fp + fn)
@@ -79,15 +81,15 @@
         if multilabel:
             fp = fp.sum(dim=0 if multidim_average == "global" else 1)
             tn = tn.sum(dim=0 if multidim_average == "global" else 1)
             return _safe_divide(tp + tn, tp + tn + fp + fn)
         return _safe_divide(tp, tp + fn)
 
     score = _safe_divide(tp + tn, tp + tn + fp + fn) if multilabel else _safe_divide(tp, tp + fn)
-    return _adjust_weights_safe_divide(score, average, multilabel, tp, fp, fn)
+    return _adjust_weights_safe_divide(score, average, multilabel, tp, fp, fn, top_k)
 
 
 def binary_accuracy(
     preds: Tensor,
     target: Tensor,
     threshold: float = 0.5,
     multidim_average: Literal["global", "samplewise"] = "global",
@@ -262,15 +264,15 @@
     if validate_args:
         _multiclass_stat_scores_arg_validation(num_classes, top_k, average, multidim_average, ignore_index)
         _multiclass_stat_scores_tensor_validation(preds, target, num_classes, multidim_average, ignore_index)
     preds, target = _multiclass_stat_scores_format(preds, target, top_k)
     tp, fp, tn, fn = _multiclass_stat_scores_update(
         preds, target, num_classes, top_k, average, multidim_average, ignore_index
     )
-    return _accuracy_reduce(tp, fp, tn, fn, average=average, multidim_average=multidim_average)
+    return _accuracy_reduce(tp, fp, tn, fn, average=average, multidim_average=multidim_average, top_k=top_k)
 
 
 def multilabel_accuracy(
     preds: Tensor,
     target: Tensor,
     num_labels: int,
     threshold: float = 0.5,
```

### Comparing `torchmetrics-1.3.1/src/torchmetrics/functional/classification/auroc.py` & `torchmetrics-1.3.2/src/torchmetrics/functional/classification/auroc.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,20 +43,21 @@
 
 
 def _reduce_auroc(
     fpr: Union[Tensor, List[Tensor]],
     tpr: Union[Tensor, List[Tensor]],
     average: Optional[Literal["macro", "weighted", "none"]] = "macro",
     weights: Optional[Tensor] = None,
+    direction: float = 1.0,
 ) -> Tensor:
     """Reduce multiple average precision score into one number."""
     if isinstance(fpr, Tensor) and isinstance(tpr, Tensor):
-        res = _auc_compute_without_check(fpr, tpr, 1.0, axis=1)
+        res = _auc_compute_without_check(fpr, tpr, direction=direction, axis=1)
     else:
-        res = torch.stack([_auc_compute_without_check(x, y, 1.0) for x, y in zip(fpr, tpr)])
+        res = torch.stack([_auc_compute_without_check(x, y, direction=direction) for x, y in zip(fpr, tpr)])
     if average is None or average == "none":
         return res
     if torch.isnan(res).any():
         rank_zero_warn(
             f"Average precision score for one or more classes was `nan`. Ignoring these classes in {average}-average",
             UserWarning,
         )
```

### Comparing `torchmetrics-1.3.1/src/torchmetrics/functional/classification/average_precision.py` & `torchmetrics-1.3.2/src/torchmetrics/functional/classification/average_precision.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.3.1/src/torchmetrics/functional/classification/calibration_error.py` & `torchmetrics-1.3.2/src/torchmetrics/functional/classification/calibration_error.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.3.1/src/torchmetrics/functional/classification/cohen_kappa.py` & `torchmetrics-1.3.2/src/torchmetrics/functional/classification/cohen_kappa.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.3.1/src/torchmetrics/functional/classification/confusion_matrix.py` & `torchmetrics-1.3.2/src/torchmetrics/functional/classification/confusion_matrix.py`

 * *Files 4% similar despite different names*

```diff
@@ -281,29 +281,21 @@
             )
     else:
         raise ValueError(
             "Either `preds` and `target` both should have the (same) shape (N, ...), or `target` should be (N, ...)"
             " and `preds` should be (N, C, ...)."
         )
 
-    num_unique_values = len(torch.unique(target))
-    check = num_unique_values > num_classes if ignore_index is None else num_unique_values > num_classes + 1
-    if check:
-        raise RuntimeError(
-            "Detected more unique values in `target` than `num_classes`. Expected only "
-            f"{num_classes if ignore_index is None else num_classes + 1} but found "
-            f"{num_unique_values} in `target`."
-        )
-
-    if not preds.is_floating_point():
-        num_unique_values = len(torch.unique(preds))
-        if num_unique_values > num_classes:
+    check_value = num_classes if ignore_index is None else num_classes + 1
+    for t, name in ((target, "target"),) + ((preds, "preds"),) if not preds.is_floating_point() else ():  # noqa: RUF005
+        num_unique_values = len(torch.unique(t))
+        if num_unique_values > check_value:
             raise RuntimeError(
-                "Detected more unique values in `preds` than `num_classes`. Expected only "
-                f"{num_classes} but found {num_unique_values} in `preds`."
+                f"Detected more unique values in `{name}` than expected. Expected only {check_value} but found"
+                f" {num_unique_values} in `target`."
             )
 
 
 def _multiclass_confusion_matrix_format(
     preds: Tensor,
     target: Tensor,
     ignore_index: Optional[int] = None,
```

### Comparing `torchmetrics-1.3.1/src/torchmetrics/functional/classification/dice.py` & `torchmetrics-1.3.2/src/torchmetrics/functional/classification/dice.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.3.1/src/torchmetrics/functional/classification/exact_match.py` & `torchmetrics-1.3.2/src/torchmetrics/functional/classification/exact_match.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.3.1/src/torchmetrics/functional/classification/f_beta.py` & `torchmetrics-1.3.2/src/torchmetrics/functional/classification/f_beta.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.3.1/src/torchmetrics/functional/classification/group_fairness.py` & `torchmetrics-1.3.2/src/torchmetrics/functional/classification/group_fairness.py`

 * *Files 0% similar despite different names*

```diff
@@ -80,22 +80,22 @@
     group_preds = list(torch.split(preds, split_sizes, dim=0))
     group_target = list(torch.split(target, split_sizes, dim=0))
 
     return [_binary_stat_scores_update(group_p, group_t) for group_p, group_t in zip(group_preds, group_target)]
 
 
 def _groups_reduce(
-    group_stats: List[Tuple[torch.Tensor, torch.Tensor, torch.Tensor, torch.Tensor]]
+    group_stats: List[Tuple[torch.Tensor, torch.Tensor, torch.Tensor, torch.Tensor]],
 ) -> Dict[str, torch.Tensor]:
     """Compute rates for all the group statistics."""
     return {f"group_{group}": torch.stack(stats) / torch.stack(stats).sum() for group, stats in enumerate(group_stats)}
 
 
 def _groups_stat_transform(
-    group_stats: List[Tuple[torch.Tensor, torch.Tensor, torch.Tensor, torch.Tensor]]
+    group_stats: List[Tuple[torch.Tensor, torch.Tensor, torch.Tensor, torch.Tensor]],
 ) -> Dict[str, torch.Tensor]:
     """Transform group statistics by creating a tensor for each statistic."""
     return {
         "tp": torch.stack([stat[0] for stat in group_stats]),
         "fp": torch.stack([stat[1] for stat in group_stats]),
         "tn": torch.stack([stat[2] for stat in group_stats]),
         "fn": torch.stack([stat[3] for stat in group_stats]),
```

### Comparing `torchmetrics-1.3.1/src/torchmetrics/functional/classification/hamming.py` & `torchmetrics-1.3.2/src/torchmetrics/functional/classification/hamming.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.3.1/src/torchmetrics/functional/classification/hinge.py` & `torchmetrics-1.3.2/src/torchmetrics/functional/classification/hinge.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.3.1/src/torchmetrics/functional/classification/jaccard.py` & `torchmetrics-1.3.2/src/torchmetrics/functional/classification/jaccard.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.3.1/src/torchmetrics/functional/classification/matthews_corrcoef.py` & `torchmetrics-1.3.2/src/torchmetrics/functional/classification/matthews_corrcoef.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.3.1/src/torchmetrics/functional/classification/precision_fixed_recall.py` & `torchmetrics-1.3.2/src/torchmetrics/functional/classification/precision_fixed_recall.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.3.1/src/torchmetrics/functional/classification/precision_recall.py` & `torchmetrics-1.3.2/src/torchmetrics/functional/classification/precision_recall.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,26 +39,27 @@
     tp: Tensor,
     fp: Tensor,
     tn: Tensor,
     fn: Tensor,
     average: Optional[Literal["binary", "micro", "macro", "weighted", "none"]],
     multidim_average: Literal["global", "samplewise"] = "global",
     multilabel: bool = False,
+    top_k: int = 1,
 ) -> Tensor:
     different_stat = fp if stat == "precision" else fn  # this is what differs between the two scores
     if average == "binary":
         return _safe_divide(tp, tp + different_stat)
     if average == "micro":
         tp = tp.sum(dim=0 if multidim_average == "global" else 1)
         fn = fn.sum(dim=0 if multidim_average == "global" else 1)
         different_stat = different_stat.sum(dim=0 if multidim_average == "global" else 1)
         return _safe_divide(tp, tp + different_stat)
 
     score = _safe_divide(tp, tp + different_stat)
-    return _adjust_weights_safe_divide(score, average, multilabel, tp, fp, fn)
+    return _adjust_weights_safe_divide(score, average, multilabel, tp, fp, fn, top_k=top_k)
 
 
 def binary_precision(
     preds: Tensor,
     target: Tensor,
     threshold: float = 0.5,
     multidim_average: Literal["global", "samplewise"] = "global",
@@ -231,15 +232,17 @@
     if validate_args:
         _multiclass_stat_scores_arg_validation(num_classes, top_k, average, multidim_average, ignore_index)
         _multiclass_stat_scores_tensor_validation(preds, target, num_classes, multidim_average, ignore_index)
     preds, target = _multiclass_stat_scores_format(preds, target, top_k)
     tp, fp, tn, fn = _multiclass_stat_scores_update(
         preds, target, num_classes, top_k, average, multidim_average, ignore_index
     )
-    return _precision_recall_reduce("precision", tp, fp, tn, fn, average=average, multidim_average=multidim_average)
+    return _precision_recall_reduce(
+        "precision", tp, fp, tn, fn, average=average, multidim_average=multidim_average, top_k=top_k
+    )
 
 
 def multilabel_precision(
     preds: Tensor,
     target: Tensor,
     num_labels: int,
     threshold: float = 0.5,
@@ -515,15 +518,17 @@
     if validate_args:
         _multiclass_stat_scores_arg_validation(num_classes, top_k, average, multidim_average, ignore_index)
         _multiclass_stat_scores_tensor_validation(preds, target, num_classes, multidim_average, ignore_index)
     preds, target = _multiclass_stat_scores_format(preds, target, top_k)
     tp, fp, tn, fn = _multiclass_stat_scores_update(
         preds, target, num_classes, top_k, average, multidim_average, ignore_index
     )
-    return _precision_recall_reduce("recall", tp, fp, tn, fn, average=average, multidim_average=multidim_average)
+    return _precision_recall_reduce(
+        "recall", tp, fp, tn, fn, average=average, multidim_average=multidim_average, top_k=top_k
+    )
 
 
 def multilabel_recall(
     preds: Tensor,
     target: Tensor,
     num_labels: int,
     threshold: float = 0.5,
```

### Comparing `torchmetrics-1.3.1/src/torchmetrics/functional/classification/precision_recall_curve.py` & `torchmetrics-1.3.2/src/torchmetrics/functional/classification/precision_recall_curve.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.3.1/src/torchmetrics/functional/classification/ranking.py` & `torchmetrics-1.3.2/src/torchmetrics/functional/classification/ranking.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.3.1/src/torchmetrics/functional/classification/recall_fixed_precision.py` & `torchmetrics-1.3.2/src/torchmetrics/functional/classification/recall_fixed_precision.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.3.1/src/torchmetrics/functional/classification/roc.py` & `torchmetrics-1.3.2/src/torchmetrics/functional/classification/roc.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.3.1/src/torchmetrics/functional/classification/specificity.py` & `torchmetrics-1.3.2/src/torchmetrics/functional/classification/specificity.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.3.1/src/torchmetrics/functional/classification/specificity_sensitivity.py` & `torchmetrics-1.3.2/src/torchmetrics/functional/classification/specificity_sensitivity.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.3.1/src/torchmetrics/functional/classification/stat_scores.py` & `torchmetrics-1.3.2/src/torchmetrics/functional/classification/stat_scores.py`

 * *Files 0% similar despite different names*

```diff
@@ -300,29 +300,21 @@
             )
     else:
         raise ValueError(
             "Either `preds` and `target` both should have the (same) shape (N, ...), or `target` should be (N, ...)"
             " and `preds` should be (N, C, ...)."
         )
 
-    num_unique_values = len(torch.unique(target))
-    check = num_unique_values > num_classes if ignore_index is None else num_unique_values > num_classes + 1
-    if check:
-        raise RuntimeError(
-            "Detected more unique values in `target` than `num_classes`. Expected only"
-            f" {num_classes if ignore_index is None else num_classes + 1} but found"
-            f" {num_unique_values} in `target`."
-        )
-
-    if not preds.is_floating_point():
-        unique_values = torch.unique(preds)
-        if len(unique_values) > num_classes:
+    check_value = num_classes if ignore_index is None else num_classes + 1
+    for t, name in ((target, "target"),) + ((preds, "preds"),) if not preds.is_floating_point() else ():  # noqa: RUF005
+        num_unique_values = len(torch.unique(t))
+        if num_unique_values > check_value:
             raise RuntimeError(
-                "Detected more unique values in `preds` than `num_classes`. Expected only"
-                f" {num_classes} but found {len(unique_values)} in `preds`."
+                f"Detected more unique values in `{name}` than expected. Expected only {check_value} but found"
+                f" {num_unique_values} in `target`."
             )
 
 
 def _multiclass_stat_scores_format(
     preds: Tensor,
     target: Tensor,
     top_k: int = 1,
```

### Comparing `torchmetrics-1.3.1/src/torchmetrics/functional/clustering/__init__.py` & `torchmetrics-1.3.2/src/torchmetrics/functional/clustering/__init__.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.3.1/src/torchmetrics/functional/clustering/adjusted_mutual_info_score.py` & `torchmetrics-1.3.2/src/torchmetrics/functional/clustering/adjusted_mutual_info_score.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.3.1/src/torchmetrics/functional/clustering/adjusted_rand_score.py` & `torchmetrics-1.3.2/src/torchmetrics/functional/clustering/adjusted_rand_score.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.3.1/src/torchmetrics/functional/clustering/calinski_harabasz_score.py` & `torchmetrics-1.3.2/src/torchmetrics/functional/clustering/calinski_harabasz_score.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.3.1/src/torchmetrics/functional/clustering/davies_bouldin_score.py` & `torchmetrics-1.3.2/src/torchmetrics/functional/clustering/davies_bouldin_score.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.3.1/src/torchmetrics/functional/clustering/dunn_index.py` & `torchmetrics-1.3.2/src/torchmetrics/functional/clustering/dunn_index.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,17 +35,17 @@
     clusters = [data[inverse_indices == label_idx] for label_idx in range(len(unique_labels))]
     centroids = [c.mean(dim=0) for c in clusters]
 
     intercluster_distance = torch.linalg.norm(
         torch.stack([a - b for a, b in combinations(centroids, 2)], dim=0), ord=p, dim=1
     )
 
-    max_intracluster_distance = torch.stack(
-        [torch.linalg.norm(ci - mu, ord=p, dim=1).max() for ci, mu in zip(clusters, centroids)]
-    )
+    max_intracluster_distance = torch.stack([
+        torch.linalg.norm(ci - mu, ord=p, dim=1).max() for ci, mu in zip(clusters, centroids)
+    ])
 
     return intercluster_distance, max_intracluster_distance
 
 
 def _dunn_index_compute(intercluster_distance: Tensor, max_intracluster_distance: Tensor) -> Tensor:
     """Compute the Dunn index based on updated state.
```

### Comparing `torchmetrics-1.3.1/src/torchmetrics/functional/clustering/fowlkes_mallows_index.py` & `torchmetrics-1.3.2/src/torchmetrics/functional/clustering/fowlkes_mallows_index.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.3.1/src/torchmetrics/functional/clustering/homogeneity_completeness_v_measure.py` & `torchmetrics-1.3.2/src/torchmetrics/functional/clustering/homogeneity_completeness_v_measure.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.3.1/src/torchmetrics/functional/clustering/mutual_info_score.py` & `torchmetrics-1.3.2/src/torchmetrics/functional/clustering/mutual_info_score.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.3.1/src/torchmetrics/functional/clustering/normalized_mutual_info_score.py` & `torchmetrics-1.3.2/src/torchmetrics/functional/clustering/normalized_mutual_info_score.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.3.1/src/torchmetrics/functional/clustering/rand_score.py` & `torchmetrics-1.3.2/src/torchmetrics/functional/clustering/rand_score.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.3.1/src/torchmetrics/functional/clustering/utils.py` & `torchmetrics-1.3.2/src/torchmetrics/functional/clustering/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         Boolean tensor indicating if all values are nonnegative
 
     """
     return torch.logical_or(x > 0.0, torch.abs(x) < atol).all()
 
 
 def _validate_average_method_arg(
-    average_method: Literal["min", "geometric", "arithmetic", "max"] = "arithmetic"
+    average_method: Literal["min", "geometric", "arithmetic", "max"] = "arithmetic",
 ) -> None:
     if average_method not in ("min", "geometric", "arithmetic", "max"):
         raise ValueError(
             "Expected argument `average_method` to be one of  `min`, `geometric`, `arithmetic`, `max`,"
             f"but got {average_method}"
         )
 
@@ -150,20 +150,18 @@
     preds_classes, preds_idx = torch.unique(preds, return_inverse=True)
     target_classes, target_idx = torch.unique(target, return_inverse=True)
 
     num_classes_preds = preds_classes.size(0)
     num_classes_target = target_classes.size(0)
 
     contingency = torch.sparse_coo_tensor(
-        torch.stack(
-            (
-                target_idx,
-                preds_idx,
-            )
-        ),
+        torch.stack((
+            target_idx,
+            preds_idx,
+        )),
         torch.ones(target_idx.shape[0], dtype=preds_idx.dtype, device=preds_idx.device),
         (
             num_classes_target,
             num_classes_preds,
         ),
     )
```

### Comparing `torchmetrics-1.3.1/src/torchmetrics/functional/detection/__init__.py` & `torchmetrics-1.3.2/src/torchmetrics/functional/detection/__init__.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.3.1/src/torchmetrics/functional/detection/_deprecated.py` & `torchmetrics-1.3.2/src/torchmetrics/functional/detection/_deprecated.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.3.1/src/torchmetrics/functional/detection/_panoptic_quality_common.py` & `torchmetrics-1.3.2/src/torchmetrics/functional/detection/_panoptic_quality_common.py`

 * *Files 0% similar despite different names*

```diff
@@ -201,15 +201,15 @@
     out = torch.flatten(out, 1, -2)
     mask_stuffs = _isin(out[:, :, 0], list(stuffs))
     mask_things = _isin(out[:, :, 0], list(things))
     # reset instance IDs of stuffs
     mask_stuffs_instance = torch.stack([torch.zeros_like(mask_stuffs), mask_stuffs], dim=-1)
     out[mask_stuffs_instance] = 0
     if not allow_unknown_category and not torch.all(mask_things | mask_stuffs):
-        raise ValueError(f"Unknown categories found: {out[~(mask_things|mask_stuffs)]}")
+        raise ValueError(f"Unknown categories found: {out[~(mask_things | mask_stuffs)]}")
     # set unknown categories to void color
     out[~(mask_things | mask_stuffs)] = out.new(void_color)
     return out
 
 
 def _calculate_iou(
     pred_color: _Color,
```

### Comparing `torchmetrics-1.3.1/src/torchmetrics/functional/detection/ciou.py` & `torchmetrics-1.3.2/src/torchmetrics/functional/detection/ciou.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.3.1/src/torchmetrics/functional/detection/diou.py` & `torchmetrics-1.3.2/src/torchmetrics/functional/detection/diou.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.3.1/src/torchmetrics/functional/detection/giou.py` & `torchmetrics-1.3.2/src/torchmetrics/functional/detection/giou.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.3.1/src/torchmetrics/functional/detection/iou.py` & `torchmetrics-1.3.2/src/torchmetrics/functional/detection/iou.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.3.1/src/torchmetrics/functional/detection/panoptic_qualities.py` & `torchmetrics-1.3.2/src/torchmetrics/functional/detection/panoptic_qualities.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.3.1/src/torchmetrics/functional/image/__init__.py` & `torchmetrics-1.3.2/src/torchmetrics/functional/image/__init__.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.3.1/src/torchmetrics/functional/image/_deprecated.py` & `torchmetrics-1.3.2/src/torchmetrics/functional/image/_deprecated.py`

 * *Files 0% similar despite different names*

```diff
@@ -106,15 +106,15 @@
     """Wrapper for deprecated import.
 
     >>> import torch
     >>> gen = torch.manual_seed(22)
     >>> preds = torch.rand(4, 3, 16, 16, generator=gen)
     >>> target = torch.rand(4, 3, 16, 16, generator=gen)
     >>> _relative_average_spectral_error(preds, target)
-    tensor(5114.6641)
+    tensor(5114.66...)
 
     """
     _deprecated_root_import_func("relative_average_spectral_error", "image")
     return relative_average_spectral_error(preds=preds, target=target, window_size=window_size)
 
 
 def _root_mean_squared_error_using_sliding_window(
```

### Comparing `torchmetrics-1.3.1/src/torchmetrics/functional/image/d_lambda.py` & `torchmetrics-1.3.2/src/torchmetrics/functional/image/d_lambda.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.3.1/src/torchmetrics/functional/image/d_s.py` & `torchmetrics-1.3.2/src/torchmetrics/functional/image/d_s.py`

 * *Files 1% similar despite different names*

```diff
@@ -181,15 +181,15 @@
         if not _TORCHVISION_AVAILABLE:
             raise ValueError(
                 "When `pan_lr` is not provided as input to metric Spatial distortion index, torchvision should be "
                 "installed. Please install with `pip install torchvision` or `pip install torchmetrics[image]`."
             )
         from torchvision.transforms.functional import resize
 
-        from torchmetrics.functional.image.helper import _uniform_filter
+        from torchmetrics.functional.image.utils import _uniform_filter
 
         pan_degraded = _uniform_filter(pan, window_size=window_size)
         pan_degraded = resize(pan_degraded, size=ms.shape[-2:], antialias=False)
     else:
         pan_degraded = pan_lr
 
     m1 = torch.zeros(length, device=preds.device)
```

### Comparing `torchmetrics-1.3.1/src/torchmetrics/functional/image/ergas.py` & `torchmetrics-1.3.2/src/torchmetrics/functional/image/ergas.py`

 * *Files 8% similar despite different names*

```diff
@@ -85,15 +85,15 @@
 
 def error_relative_global_dimensionless_synthesis(
     preds: Tensor,
     target: Tensor,
     ratio: float = 4,
     reduction: Literal["elementwise_mean", "sum", "none", None] = "elementwise_mean",
 ) -> Tensor:
-    """Erreur Relative Globale Adimensionnelle de Synthèse.
+    """Calculates `Error relative global dimensionless synthesis`_ (ERGAS) metric.
 
     Args:
         preds: estimated image
         target: ground truth image
         ratio: ratio of high resolution to low resolution
         reduction: a method to reduce metric score over labels.
 
@@ -115,15 +115,10 @@
         >>> gen = torch.manual_seed(42)
         >>> preds = torch.rand([16, 1, 16, 16], generator=gen)
         >>> target = preds * 0.75
         >>> ergds = error_relative_global_dimensionless_synthesis(preds, target)
         >>> torch.round(ergds)
         tensor(154.)
 
-    References:
-        [1] Qian Du; Nicholas H. Younan; Roger King; Vijay P. Shah, "On the Performance Evaluation of
-        Pan-Sharpening Techniques" in IEEE Geoscience and Remote Sensing Letters, vol. 4, no. 4, pp. 518-522,
-        15 October 2007, doi: 10.1109/LGRS.2007.896328.
-
     """
     preds, target = _ergas_update(preds, target)
     return _ergas_compute(preds, target, ratio, reduction)
```

### Comparing `torchmetrics-1.3.1/src/torchmetrics/functional/image/gradients.py` & `torchmetrics-1.3.2/src/torchmetrics/functional/image/gradients.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.3.1/src/torchmetrics/functional/image/helper.py` & `torchmetrics-1.3.2/src/torchmetrics/functional/image/utils.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.3.1/src/torchmetrics/functional/image/lpips.py` & `torchmetrics-1.3.2/src/torchmetrics/functional/image/lpips.py`

 * *Files 0% similar despite different names*

```diff
@@ -382,15 +382,15 @@
 
 def _lpips_update(img1: Tensor, img2: Tensor, net: nn.Module, normalize: bool) -> Tuple[Tensor, Union[int, Tensor]]:
     if not (_valid_img(img1, normalize) and _valid_img(img2, normalize)):
         raise ValueError(
             "Expected both input arguments to be normalized tensors with shape [N, 3, H, W]."
             f" Got input with shape {img1.shape} and {img2.shape} and values in range"
             f" {[img1.min(), img1.max()]} and {[img2.min(), img2.max()]} when all values are"
-            f" expected to be in the {[0,1] if normalize else [-1,1]} range."
+            f" expected to be in the {[0, 1] if normalize else [-1, 1]} range."
         )
     loss = net(img1, img2, normalize=normalize).squeeze()
     return loss, img1.shape[0]
 
 
 def _lpips_compute(sum_scores: Tensor, total: Union[Tensor, int], reduction: Literal["sum", "mean"] = "mean") -> Tensor:
     return sum_scores / total if reduction == "mean" else sum_scores
```

### Comparing `torchmetrics-1.3.1/src/torchmetrics/functional/image/lpips_models/alex.pth` & `torchmetrics-1.3.2/src/torchmetrics/functional/image/lpips_models/alex.pth`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.3.1/src/torchmetrics/functional/image/lpips_models/squeeze.pth` & `torchmetrics-1.3.2/src/torchmetrics/functional/image/lpips_models/squeeze.pth`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.3.1/src/torchmetrics/functional/image/lpips_models/vgg.pth` & `torchmetrics-1.3.2/src/torchmetrics/functional/image/lpips_models/vgg.pth`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.3.1/src/torchmetrics/functional/image/perceptual_path_length.py` & `torchmetrics-1.3.2/src/torchmetrics/functional/image/perceptual_path_length.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.3.1/src/torchmetrics/functional/image/psnr.py` & `torchmetrics-1.3.2/src/torchmetrics/functional/image/psnr.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.3.1/src/torchmetrics/functional/image/psnrb.py` & `torchmetrics-1.3.2/src/torchmetrics/functional/image/psnrb.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.3.1/src/torchmetrics/functional/image/rase.py` & `torchmetrics-1.3.2/src/torchmetrics/functional/image/rase.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,16 +13,16 @@
 # limitations under the License.
 
 from typing import Tuple
 
 import torch
 from torch import Tensor
 
-from torchmetrics.functional.image.helper import _uniform_filter
 from torchmetrics.functional.image.rmse_sw import _rmse_sw_compute, _rmse_sw_update
+from torchmetrics.functional.image.utils import _uniform_filter
 
 
 def _rase_update(
     preds: Tensor, target: Tensor, window_size: int, rmse_map: Tensor, target_sum: Tensor, total_images: Tensor
 ) -> Tuple[Tensor, Tensor, Tensor]:
     """Calculate the sum of RMSE map values for the batch of examples and update intermediate states.
 
@@ -81,15 +81,15 @@
 
     Example:
         >>> from torchmetrics.functional.image import relative_average_spectral_error
         >>> g = torch.manual_seed(22)
         >>> preds = torch.rand(4, 3, 16, 16)
         >>> target = torch.rand(4, 3, 16, 16)
         >>> relative_average_spectral_error(preds, target)
-        tensor(5114.6641)
+        tensor(5114.66...)
 
     Raises:
         ValueError: If ``window_size`` is not a positive integer.
 
     """
     if not isinstance(window_size, int) or isinstance(window_size, int) and window_size < 1:
         raise ValueError("Argument `window_size` is expected to be a positive integer.")
```

### Comparing `torchmetrics-1.3.1/src/torchmetrics/functional/image/rmse_sw.py` & `torchmetrics-1.3.2/src/torchmetrics/functional/image/rmse_sw.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # limitations under the License.
 
 from typing import Optional, Tuple, Union
 
 import torch
 from torch import Tensor
 
-from torchmetrics.functional.image.helper import _uniform_filter
+from torchmetrics.functional.image.utils import _uniform_filter
 from torchmetrics.utilities.checks import _check_same_shape
 
 
 def _rmse_sw_update(
     preds: Tensor,
     target: Tensor,
     window_size: int,
```

### Comparing `torchmetrics-1.3.1/src/torchmetrics/functional/image/sam.py` & `torchmetrics-1.3.2/src/torchmetrics/functional/image/sam.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.3.1/src/torchmetrics/functional/image/scc.py` & `torchmetrics-1.3.2/src/torchmetrics/functional/image/scc.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.3.1/src/torchmetrics/functional/image/ssim.py` & `torchmetrics-1.3.2/src/torchmetrics/functional/image/ssim.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from typing import List, Optional, Sequence, Tuple, Union
 
 import torch
 from torch import Tensor
 from torch.nn import functional as F  # noqa: N812
 from typing_extensions import Literal
 
-from torchmetrics.functional.image.helper import _gaussian_kernel_2d, _gaussian_kernel_3d, _reflection_pad_3d
+from torchmetrics.functional.image.utils import _gaussian_kernel_2d, _gaussian_kernel_3d, _reflection_pad_3d
 from torchmetrics.utilities.checks import _check_same_shape
 from torchmetrics.utilities.distributed import reduce
 
 
 def _ssim_check_inputs(preds: Tensor, target: Tensor) -> Tuple[Tensor, Tensor]:
     """Update and returns variables required to compute Structural Similarity Index Measure.
 
@@ -150,16 +150,17 @@
 
     output_list = outputs.split(preds.shape[0])
 
     mu_pred_sq = output_list[0].pow(2)
     mu_target_sq = output_list[1].pow(2)
     mu_pred_target = output_list[0] * output_list[1]
 
-    sigma_pred_sq = output_list[2] - mu_pred_sq
-    sigma_target_sq = output_list[3] - mu_target_sq
+    # Calculate the variance of the predicted and target images, should be non-negative
+    sigma_pred_sq = torch.clamp(output_list[2] - mu_pred_sq, min=0.0)
+    sigma_target_sq = torch.clamp(output_list[3] - mu_target_sq, min=0.0)
     sigma_pred_target = output_list[4] - mu_pred_target
 
     upper = 2 * sigma_pred_target.to(dtype) + c2
     lower = (sigma_pred_sq + sigma_target_sq).to(dtype) + c2
 
     ssim_idx_full_image = ((2 * mu_pred_target + c1) * upper) / ((mu_pred_sq + mu_target_sq + c1) * lower)
```

### Comparing `torchmetrics-1.3.1/src/torchmetrics/functional/image/tv.py` & `torchmetrics-1.3.2/src/torchmetrics/functional/image/tv.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.3.1/src/torchmetrics/functional/image/uqi.py` & `torchmetrics-1.3.2/src/torchmetrics/functional/image/uqi.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # limitations under the License.
 from typing import Optional, Sequence, Tuple
 
 import torch
 from torch import Tensor, nn
 from typing_extensions import Literal
 
-from torchmetrics.functional.image.helper import _gaussian_kernel_2d
+from torchmetrics.functional.image.utils import _gaussian_kernel_2d
 from torchmetrics.utilities.checks import _check_same_shape
 from torchmetrics.utilities.distributed import reduce
 
 
 def _uqi_update(preds: Tensor, target: Tensor) -> Tuple[Tensor, Tensor]:
     """Update and returns variables required to compute Universal Image Quality Index.
 
@@ -98,16 +98,17 @@
     outputs = nn.functional.conv2d(input_list, kernel, groups=channel)
     output_list = outputs.split(preds.shape[0])
 
     mu_pred_sq = output_list[0].pow(2)
     mu_target_sq = output_list[1].pow(2)
     mu_pred_target = output_list[0] * output_list[1]
 
-    sigma_pred_sq = output_list[2] - mu_pred_sq
-    sigma_target_sq = output_list[3] - mu_target_sq
+    # Calculate the variance of the predicted and target images, should be non-negative
+    sigma_pred_sq = torch.clamp(output_list[2] - mu_pred_sq, min=0.0)
+    sigma_target_sq = torch.clamp(output_list[3] - mu_target_sq, min=0.0)
     sigma_pred_target = output_list[4] - mu_pred_target
 
     upper = 2 * sigma_pred_target
     lower = sigma_pred_sq + sigma_target_sq
     eps = torch.finfo(sigma_pred_sq.dtype).eps
     uqi_idx = ((2 * mu_pred_target) * upper) / ((mu_pred_sq + mu_target_sq) * lower + eps)
     uqi_idx = uqi_idx[..., pad_h:-pad_h, pad_w:-pad_w]
```

### Comparing `torchmetrics-1.3.1/src/torchmetrics/functional/image/vif.py` & `torchmetrics-1.3.2/src/torchmetrics/functional/image/vif.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.3.1/src/torchmetrics/functional/multimodal/__init__.py` & `torchmetrics-1.3.2/src/torchmetrics/functional/multimodal/__init__.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.3.1/src/torchmetrics/functional/multimodal/clip_iqa.py` & `torchmetrics-1.3.2/src/torchmetrics/functional/multimodal/clip_iqa.py`

 * *Files 0% similar despite different names*

```diff
@@ -63,15 +63,15 @@
 def _get_clip_iqa_model_and_processor(
     model_name_or_path: Literal[
         "clip_iqa",
         "openai/clip-vit-base-patch16",
         "openai/clip-vit-base-patch32",
         "openai/clip-vit-large-patch14-336",
         "openai/clip-vit-large-patch14",
-    ]
+    ],
 ) -> Tuple["_CLIPModel", "_CLIPProcessor"]:
     """Extract the CLIP model and processor from the model name or path."""
     from transformers import CLIPProcessor as _CLIPProcessor
 
     if model_name_or_path == "clip_iqa":
         if not _PIQ_GREATER_EQUAL_0_8:
             raise ValueError(
```

### Comparing `torchmetrics-1.3.1/src/torchmetrics/functional/multimodal/clip_score.py` & `torchmetrics-1.3.2/src/torchmetrics/functional/multimodal/clip_score.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.3.1/src/torchmetrics/functional/nominal/__init__.py` & `torchmetrics-1.3.2/src/torchmetrics/functional/nominal/__init__.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.3.1/src/torchmetrics/functional/nominal/cramers.py` & `torchmetrics-1.3.2/src/torchmetrics/functional/nominal/cramers.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.3.1/src/torchmetrics/functional/nominal/fleiss_kappa.py` & `torchmetrics-1.3.2/src/torchmetrics/functional/nominal/fleiss_kappa.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.3.1/src/torchmetrics/functional/nominal/pearson.py` & `torchmetrics-1.3.2/src/torchmetrics/functional/nominal/pearson.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.3.1/src/torchmetrics/functional/nominal/theils_u.py` & `torchmetrics-1.3.2/src/torchmetrics/functional/nominal/theils_u.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.3.1/src/torchmetrics/functional/nominal/tschuprows.py` & `torchmetrics-1.3.2/src/torchmetrics/functional/nominal/tschuprows.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.3.1/src/torchmetrics/functional/nominal/utils.py` & `torchmetrics-1.3.2/src/torchmetrics/functional/nominal/utils.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.3.1/src/torchmetrics/functional/pairwise/__init__.py` & `torchmetrics-1.3.2/src/torchmetrics/functional/pairwise/__init__.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.3.1/src/torchmetrics/functional/pairwise/cosine.py` & `torchmetrics-1.3.2/src/torchmetrics/functional/pairwise/cosine.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.3.1/src/torchmetrics/functional/pairwise/euclidean.py` & `torchmetrics-1.3.2/src/torchmetrics/functional/pairwise/euclidean.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.3.1/src/torchmetrics/functional/pairwise/helpers.py` & `torchmetrics-1.3.2/src/torchmetrics/functional/pairwise/helpers.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.3.1/src/torchmetrics/functional/pairwise/linear.py` & `torchmetrics-1.3.2/src/torchmetrics/functional/pairwise/linear.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.3.1/src/torchmetrics/functional/pairwise/manhattan.py` & `torchmetrics-1.3.2/src/torchmetrics/functional/pairwise/manhattan.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.3.1/src/torchmetrics/functional/pairwise/minkowski.py` & `torchmetrics-1.3.2/src/torchmetrics/functional/pairwise/minkowski.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.3.1/src/torchmetrics/functional/regression/__init__.py` & `torchmetrics-1.3.2/src/torchmetrics/functional/regression/__init__.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.3.1/src/torchmetrics/functional/regression/concordance.py` & `torchmetrics-1.3.2/src/torchmetrics/functional/regression/concordance.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.3.1/src/torchmetrics/functional/regression/cosine_similarity.py` & `torchmetrics-1.3.2/src/torchmetrics/functional/regression/cosine_similarity.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.3.1/src/torchmetrics/functional/regression/csi.py` & `torchmetrics-1.3.2/src/torchmetrics/functional/regression/csi.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.3.1/src/torchmetrics/functional/regression/explained_variance.py` & `torchmetrics-1.3.2/src/torchmetrics/functional/regression/explained_variance.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.3.1/src/torchmetrics/functional/regression/kendall.py` & `torchmetrics-1.3.2/src/torchmetrics/functional/regression/kendall.py`

 * *Files 0% similar despite different names*

```diff
@@ -401,13 +401,16 @@
     _variant = _MetricVariant.from_str(str(variant))
     _alternative = _TestAlternative.from_str(str(alternative)) if t_test else None
 
     _preds, _target = _kendall_corrcoef_update(
         preds, target, [], [], num_outputs=1 if preds.ndim == 1 else preds.shape[-1]
     )
     tau, p_value = _kendall_corrcoef_compute(
-        dim_zero_cat(_preds), dim_zero_cat(_target), _variant, _alternative  # type: ignore[arg-type]  # todo
+        dim_zero_cat(_preds),
+        dim_zero_cat(_target),
+        _variant,  # type: ignore[arg-type]  # todo
+        _alternative,  # type: ignore[arg-type]  # todo
     )
 
     if p_value is not None:
         return tau, p_value
     return tau
```

### Comparing `torchmetrics-1.3.1/src/torchmetrics/functional/regression/kl_divergence.py` & `torchmetrics-1.3.2/src/torchmetrics/functional/regression/kl_divergence.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.3.1/src/torchmetrics/functional/regression/log_cosh.py` & `torchmetrics-1.3.2/src/torchmetrics/functional/regression/log_cosh.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.3.1/src/torchmetrics/functional/regression/log_mse.py` & `torchmetrics-1.3.2/src/torchmetrics/functional/regression/log_mse.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.3.1/src/torchmetrics/functional/regression/mae.py` & `torchmetrics-1.3.2/src/torchmetrics/functional/regression/mae.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.3.1/src/torchmetrics/functional/regression/mape.py` & `torchmetrics-1.3.2/src/torchmetrics/functional/regression/mape.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.3.1/src/torchmetrics/functional/regression/minkowski.py` & `torchmetrics-1.3.2/src/torchmetrics/functional/regression/minkowski.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.3.1/src/torchmetrics/functional/regression/mse.py` & `torchmetrics-1.3.2/src/torchmetrics/functional/regression/mse.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.3.1/src/torchmetrics/functional/regression/pearson.py` & `torchmetrics-1.3.2/src/torchmetrics/functional/regression/pearson.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,16 +55,16 @@
     num_obs = preds.shape[0]
     cond = num_prior.mean() > 0 or num_obs == 1
 
     if cond:
         mx_new = (num_prior * mean_x + preds.sum(0)) / (num_prior + num_obs)
         my_new = (num_prior * mean_y + target.sum(0)) / (num_prior + num_obs)
     else:
-        mx_new = preds.mean(0)
-        my_new = target.mean(0)
+        mx_new = preds.mean(0).to(mean_x.dtype)
+        my_new = target.mean(0).to(mean_y.dtype)
 
     num_prior += num_obs
 
     if cond:
         var_x += ((preds - mx_new) * (preds - mean_x)).sum(0)
         var_y += ((target - my_new) * (target - mean_y)).sum(0)
     else:
```

### Comparing `torchmetrics-1.3.1/src/torchmetrics/functional/regression/r2.py` & `torchmetrics-1.3.2/src/torchmetrics/functional/regression/r2.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.3.1/src/torchmetrics/functional/regression/rse.py` & `torchmetrics-1.3.2/src/torchmetrics/functional/regression/rse.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.3.1/src/torchmetrics/functional/regression/spearman.py` & `torchmetrics-1.3.2/src/torchmetrics/functional/regression/spearman.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.3.1/src/torchmetrics/functional/regression/symmetric_mape.py` & `torchmetrics-1.3.2/src/torchmetrics/functional/regression/symmetric_mape.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.3.1/src/torchmetrics/functional/regression/tweedie_deviance.py` & `torchmetrics-1.3.2/src/torchmetrics/functional/regression/tweedie_deviance.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.3.1/src/torchmetrics/functional/regression/utils.py` & `torchmetrics-1.3.2/src/torchmetrics/functional/regression/utils.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.3.1/src/torchmetrics/functional/regression/wmape.py` & `torchmetrics-1.3.2/src/torchmetrics/functional/regression/wmape.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.3.1/src/torchmetrics/functional/retrieval/__init__.py` & `torchmetrics-1.3.2/src/torchmetrics/functional/retrieval/__init__.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.3.1/src/torchmetrics/functional/retrieval/_deprecated.py` & `torchmetrics-1.3.2/src/torchmetrics/functional/retrieval/_deprecated.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.3.1/src/torchmetrics/functional/retrieval/auroc.py` & `torchmetrics-1.3.2/src/torchmetrics/functional/retrieval/auroc.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.3.1/src/torchmetrics/functional/retrieval/average_precision.py` & `torchmetrics-1.3.2/src/torchmetrics/functional/retrieval/average_precision.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.3.1/src/torchmetrics/functional/retrieval/fall_out.py` & `torchmetrics-1.3.2/src/torchmetrics/functional/retrieval/fall_out.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.3.1/src/torchmetrics/functional/retrieval/hit_rate.py` & `torchmetrics-1.3.2/src/torchmetrics/functional/retrieval/hit_rate.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.3.1/src/torchmetrics/functional/retrieval/ndcg.py` & `torchmetrics-1.3.2/src/torchmetrics/functional/retrieval/ndcg.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.3.1/src/torchmetrics/functional/retrieval/precision.py` & `torchmetrics-1.3.2/src/torchmetrics/functional/retrieval/precision.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.3.1/src/torchmetrics/functional/retrieval/precision_recall_curve.py` & `torchmetrics-1.3.2/src/torchmetrics/functional/retrieval/precision_recall_curve.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.3.1/src/torchmetrics/functional/retrieval/r_precision.py` & `torchmetrics-1.3.2/src/torchmetrics/functional/retrieval/r_precision.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.3.1/src/torchmetrics/functional/retrieval/recall.py` & `torchmetrics-1.3.2/src/torchmetrics/functional/retrieval/recall.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.3.1/src/torchmetrics/functional/retrieval/reciprocal_rank.py` & `torchmetrics-1.3.2/src/torchmetrics/functional/retrieval/reciprocal_rank.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.3.1/src/torchmetrics/functional/segmentation/__init__.py` & `torchmetrics-1.3.2/src/torchmetrics/functional/segmentation/__init__.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.3.1/src/torchmetrics/functional/segmentation/utils.py` & `torchmetrics-1.3.2/src/torchmetrics/functional/segmentation/utils.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.3.1/src/torchmetrics/functional/text/__init__.py` & `torchmetrics-1.3.2/src/torchmetrics/functional/text/__init__.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.3.1/src/torchmetrics/functional/text/_deprecated.py` & `torchmetrics-1.3.2/src/torchmetrics/functional/text/_deprecated.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.3.1/src/torchmetrics/functional/text/bert.py` & `torchmetrics-1.3.2/src/torchmetrics/functional/text/bert.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.3.1/src/torchmetrics/functional/text/bleu.py` & `torchmetrics-1.3.2/src/torchmetrics/functional/text/bleu.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.3.1/src/torchmetrics/functional/text/cer.py` & `torchmetrics-1.3.2/src/torchmetrics/functional/text/cer.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.3.1/src/torchmetrics/functional/text/chrf.py` & `torchmetrics-1.3.2/src/torchmetrics/functional/text/chrf.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 from collections import defaultdict
+from itertools import chain
 from typing import Dict, List, Optional, Sequence, Tuple, Union
 
 import torch
 from torch import Tensor, tensor
 
 from torchmetrics.functional.text.helper import _validate_inputs
 
@@ -123,15 +124,15 @@
     Args:
         sentence: An input sentence to split
 
     Return:
         An aggregated list of separated words and punctuations.
 
     """
-    return sum((_separate_word_and_punctuation(word) for word in sentence.strip().split()), [])
+    return list(chain.from_iterable(_separate_word_and_punctuation(word) for word in sentence.strip().split()))
 
 
 def _ngram_counts(char_or_word_list: List[str], n_gram_order: int) -> Dict[int, Dict[Tuple[str, ...], Tensor]]:
     """Calculate n-gram counts.
 
     Args:
         char_or_word_list: A list of characters of words
```

### Comparing `torchmetrics-1.3.1/src/torchmetrics/functional/text/edit.py` & `torchmetrics-1.3.2/src/torchmetrics/functional/text/edit.py`

 * *Files 5% similar despite different names*

```diff
@@ -34,15 +34,16 @@
         raise ValueError(f"Expected all values in argument `target` to be string type, but got {target}")
     if len(preds) != len(target):
         raise ValueError(
             f"Expected argument `preds` and `target` to have same length, but got {len(preds)} and {len(target)}"
         )
 
     distance = [
-        _LE_distance(t, op_substitute=substitution_cost)(p)[0] for p, t in zip(preds, target)  # type: ignore[arg-type]
+        _LE_distance(t, op_substitute=substitution_cost)(p)[0]  # type: ignore[arg-type]
+        for p, t in zip(preds, target)
     ]
     return torch.tensor(distance, dtype=torch.int)
 
 
 def _edit_distance_compute(
     edit_scores: Tensor,
     num_elements: Union[Tensor, int],
```

### Comparing `torchmetrics-1.3.1/src/torchmetrics/functional/text/eed.py` & `torchmetrics-1.3.2/src/torchmetrics/functional/text/eed.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.3.1/src/torchmetrics/functional/text/helper.py` & `torchmetrics-1.3.2/src/torchmetrics/functional/text/helper.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.3.1/src/torchmetrics/functional/text/helper_embedding_metric.py` & `torchmetrics-1.3.2/src/torchmetrics/functional/text/helper_embedding_metric.py`

 * *Files 0% similar despite different names*

```diff
@@ -245,17 +245,17 @@
 
         """
         token_counter: Counter = Counter()
         for tokens in map(self._set_of_tokens, self.text["input_ids"]):
             token_counter.update(tokens)
 
         tokens_idf: Dict[int, float] = defaultdict(self._get_tokens_idf_default_value)
-        tokens_idf.update(
-            {idx: math.log((self.num_sentences + 1) / (occurrence + 1)) for idx, occurrence in token_counter.items()}
-        )
+        tokens_idf.update({
+            idx: math.log((self.num_sentences + 1) / (occurrence + 1)) for idx, occurrence in token_counter.items()
+        })
         return tokens_idf
 
     def _get_tokens_idf_default_value(self) -> float:
         """Ensure `defaultdict` can be pickled."""
         return math.log((self.num_sentences + 1) / 1)
 
     @staticmethod
```

### Comparing `torchmetrics-1.3.1/src/torchmetrics/functional/text/infolm.py` & `torchmetrics-1.3.2/src/torchmetrics/functional/text/infolm.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.3.1/src/torchmetrics/functional/text/mer.py` & `torchmetrics-1.3.2/src/torchmetrics/functional/text/mer.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.3.1/src/torchmetrics/functional/text/perplexity.py` & `torchmetrics-1.3.2/src/torchmetrics/functional/text/perplexity.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.3.1/src/torchmetrics/functional/text/rouge.py` & `torchmetrics-1.3.2/src/torchmetrics/functional/text/rouge.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.3.1/src/torchmetrics/functional/text/sacre_bleu.py` & `torchmetrics-1.3.2/src/torchmetrics/functional/text/sacre_bleu.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.3.1/src/torchmetrics/functional/text/squad.py` & `torchmetrics-1.3.2/src/torchmetrics/functional/text/squad.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.3.1/src/torchmetrics/functional/text/ter.py` & `torchmetrics-1.3.2/src/torchmetrics/functional/text/ter.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.3.1/src/torchmetrics/functional/text/wer.py` & `torchmetrics-1.3.2/src/torchmetrics/functional/text/wer.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.3.1/src/torchmetrics/functional/text/wil.py` & `torchmetrics-1.3.2/src/torchmetrics/functional/text/wil.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.3.1/src/torchmetrics/functional/text/wip.py` & `torchmetrics-1.3.2/src/torchmetrics/functional/text/wip.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.3.1/src/torchmetrics/image/__init__.py` & `torchmetrics-1.3.2/src/torchmetrics/image/__init__.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.3.1/src/torchmetrics/image/_deprecated.py` & `torchmetrics-1.3.2/src/torchmetrics/image/_deprecated.py`

 * *Files 0% similar despite different names*

```diff
@@ -105,15 +105,15 @@
 
     >>> import torch
     >>> g = torch.manual_seed(22)
     >>> preds = torch.rand(4, 3, 16, 16)
     >>> target = torch.rand(4, 3, 16, 16)
     >>> rase = _RelativeAverageSpectralError()
     >>> rase(preds, target)
-    tensor(5114.6641)
+    tensor(5114.66...)
 
     """
 
     def __init__(
         self,
         window_size: int = 8,
         **kwargs: Dict[str, Any],
```

### Comparing `torchmetrics-1.3.1/src/torchmetrics/image/d_lambda.py` & `torchmetrics-1.3.2/src/torchmetrics/image/d_lambda.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.3.1/src/torchmetrics/image/d_s.py` & `torchmetrics-1.3.2/src/torchmetrics/image/d_s.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,17 +28,28 @@
     __doctest_skip__ = ["SpatialDistortionIndex.plot"]
 
 if not _TORCHVISION_AVAILABLE:
     __doctest_skip__ = ["SpatialDistortionIndex", "SpatialDistortionIndex.plot"]
 
 
 class SpatialDistortionIndex(Metric):
-    """Compute Spatial Distortion Index (SpatialDistortionIndex_) also now as D_s.
+    r"""Compute Spatial Distortion Index (SpatialDistortionIndex_) also now as D_s.
 
-    The metric is used to compare the spatial distortion between two images.
+    The metric is used to compare the spatial distortion between two images. A value of 0 indicates no distortion
+    (optimal value) and corresponds to the case where the high resolution panchromatic image is equal to the low
+    resolution panchromatic image. The metric is defined as:
+
+    .. math::
+        D_s = \\sqrt[q]{\frac{1}{L}\\sum_{l=1}^L|Q(\\hat{G_l}, P) - Q(\tilde{G}, \tilde{P})|^q}
+
+    where :math:`Q` is the universal image quality index (see this
+    :class:`~torchmetrics.image.UniversalImageQualityIndex` for more info), :math:`\\hat{G_l}` is the l-th band of the
+    high resolution multispectral image, :math:`\tilde{G}` is the high resolution panchromatic image, :math:`P` is the
+    high resolution panchromatic image, :math:`\tilde{P}` is the low resolution panchromatic image, :math:`L` is the
+    number of bands and :math:`q` is the order of the norm applied on the difference.
 
     As input to ``forward`` and ``update`` the metric accepts the following input
 
     - ``preds`` (:class:`~torch.Tensor`): High resolution multispectral image of shape ``(N,C,H,W)``.
     - ``target`` (:class:`~Dict`): A dictionary containing the following keys:
         - ``ms`` (:class:`~torch.Tensor`): Low resolution multispectral image of shape ``(N,C,H',W')``.
         - ``pan`` (:class:`~torch.Tensor`): High resolution panchromatic image of shape ``(N,C,H,W)``.
@@ -73,15 +84,15 @@
         ... }
         >>> sdi = SpatialDistortionIndex()
         >>> sdi(preds, target)
         tensor(0.0090)
 
     """
 
-    higher_is_better: bool = True
+    higher_is_better: bool = False
     is_differentiable: bool = True
     full_state_update: bool = False
     plot_lower_bound: float = 0.0
     plot_upper_bound: float = 1.0
 
     preds: List[Tensor]
     ms: List[Tensor]
@@ -135,15 +146,15 @@
         """
         if "ms" not in target:
             raise ValueError(f"Expected `target` to have key `ms`. Got target: {target.keys()}.")
         if "pan" not in target:
             raise ValueError(f"Expected `target` to have key `pan`. Got target: {target.keys()}.")
         ms = target["ms"]
         pan = target["pan"]
-        pan_lr = target["pan_lr"] if "pan_lr" in target else None
+        pan_lr = target.get("pan_lr")
         preds, ms, pan, pan_lr = _spatial_distortion_index_update(preds, ms, pan, pan_lr)
         self.preds.append(preds)
         self.ms.append(target["ms"])
         self.pan.append(target["pan"])
         if "pan_lr" in target:
             self.pan_lr.append(target["pan_lr"])
```

### Comparing `torchmetrics-1.3.1/src/torchmetrics/image/ergas.py` & `torchmetrics-1.3.2/src/torchmetrics/image/ergas.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,31 +25,39 @@
 from torchmetrics.utilities.plot import _AX_TYPE, _PLOT_OUT_TYPE
 
 if not _MATPLOTLIB_AVAILABLE:
     __doctest_skip__ = ["ErrorRelativeGlobalDimensionlessSynthesis.plot"]
 
 
 class ErrorRelativeGlobalDimensionlessSynthesis(Metric):
-    """Calculate `Relative dimensionless global error synthesis`_ (ERGAS).
+    r"""Calculate the `Error relative global dimensionless synthesis`_  (ERGAS) metric.
 
     This metric is used to calculate the accuracy of Pan sharpened image considering normalized average error of each
-    band of the result image.
+    band of the result image. It is defined as:
+
+    .. math::
+        ERGAS = 100 * \frac{h}{l} \\sqrt{\frac{1}{N} \\sum_{k=1}^{N} \frac{RMSE(B_k)^2}{\\mu_k^2}}
+
+    where :math:`h` and :math:`l` denote the spatial resolution (pixel size) of the high and low resolution images,
+    often shorted to the ratio between them :math:`r=h/l`. :math:`N` is the number of spectral bands, :math:`RMSE(B_k)`
+    is the root mean square error of the k-th band between low and high resolution images, and :math:`\\mu_k` is the
+    mean value of the k-th band of the reference image.
 
     As input to ``forward`` and ``update`` the metric accepts the following input
 
     - ``preds`` (:class:`~torch.Tensor`): Predictions from model
     - ``target`` (:class:`~torch.Tensor`): Ground truth values
 
     As output of `forward` and `compute` the metric returns the following output
 
     - ``ergas`` (:class:`~torch.Tensor`): if ``reduction!='none'`` returns float scalar tensor with average ERGAS
       value over sample else returns tensor of shape ``(N,)`` with ERGAS values per sample
 
     Args:
-        ratio: ratio of high resolution to low resolution
+        ratio: ratio of high resolution to low resolution.
         reduction: a method to reduce metric score over labels.
 
             - ``'elementwise_mean'``: takes the mean (default)
             - ``'sum'``: takes the sum
             - ``'none'`` or ``None``: no reduction will be applied
 
         kwargs: Additional keyword arguments, see :ref:`Metric kwargs` for more info.
```

### Comparing `torchmetrics-1.3.1/src/torchmetrics/image/fid.py` & `torchmetrics-1.3.2/src/torchmetrics/image/fid.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.3.1/src/torchmetrics/image/inception.py` & `torchmetrics-1.3.2/src/torchmetrics/image/inception.py`

 * *Files 0% similar despite different names*

```diff
@@ -89,14 +89,15 @@
         >>> # generate some images
         >>> imgs = torch.randint(0, 255, (100, 3, 299, 299), dtype=torch.uint8)
         >>> inception.update(imgs)
         >>> inception.compute()
         (tensor(1.0544), tensor(0.0117))
 
     """
+
     is_differentiable: bool = False
     higher_is_better: bool = True
     full_state_update: bool = False
     plot_lower_bound: float = 0.0
 
     features: List
     inception: Module
```

### Comparing `torchmetrics-1.3.1/src/torchmetrics/image/kid.py` & `torchmetrics-1.3.2/src/torchmetrics/image/kid.py`

 * *Files 0% similar despite different names*

```diff
@@ -151,14 +151,15 @@
         >>> imgs_dist2 = torch.randint(100, 255, (100, 3, 299, 299), dtype=torch.uint8)
         >>> kid.update(imgs_dist1, real=True)
         >>> kid.update(imgs_dist2, real=False)
         >>> kid.compute()
         (tensor(0.0337), tensor(0.0023))
 
     """
+
     higher_is_better: bool = False
     is_differentiable: bool = False
     full_state_update: bool = False
     plot_lower_bound: float = 0.0
     plot_upper_bound: float = 1.0
 
     real_features: List[Tensor]
```

### Comparing `torchmetrics-1.3.1/src/torchmetrics/image/lpip.py` & `torchmetrics-1.3.2/src/torchmetrics/image/lpip.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.3.1/src/torchmetrics/image/mifid.py` & `torchmetrics-1.3.2/src/torchmetrics/image/mifid.py`

 * *Files 0% similar despite different names*

```diff
@@ -138,14 +138,15 @@
         >>> imgs_dist2 = torch.randint(100, 255, (100, 3, 299, 299), dtype=torch.uint8)
         >>> mifid.update(imgs_dist1, real=True)
         >>> mifid.update(imgs_dist2, real=False)
         >>> mifid.compute()
         tensor(3003.3691)
 
     """
+
     higher_is_better: bool = False
     is_differentiable: bool = False
     full_state_update: bool = False
 
     real_features: List[Tensor]
     fake_features: List[Tensor]
```

### Comparing `torchmetrics-1.3.1/src/torchmetrics/image/perceptual_path_length.py` & `torchmetrics-1.3.2/src/torchmetrics/image/perceptual_path_length.py`

 * *Files 0% similar despite different names*

```diff
@@ -114,14 +114,15 @@
         >>> ppl = PerceptualPathLength(num_samples=10)
         >>> ppl(generator)  # doctest: +SKIP
         (tensor(0.2371),
         tensor(0.1763),
         tensor([0.3502, 0.1362, 0.2535, 0.0902, 0.1784, 0.0769, 0.5871, 0.0691, 0.3921]))
 
     """
+
     is_differentiable: bool = False
     higher_is_better: Optional[bool] = True
     full_state_update: bool = True
 
     net: nn.Module
     feature_network: str = "net"
```

### Comparing `torchmetrics-1.3.1/src/torchmetrics/image/psnr.py` & `torchmetrics-1.3.2/src/torchmetrics/image/psnr.py`

 * *Files 0% similar despite different names*

```diff
@@ -71,14 +71,15 @@
         >>> psnr = PeakSignalNoiseRatio()
         >>> preds = torch.tensor([[0.0, 1.0], [2.0, 3.0]])
         >>> target = torch.tensor([[3.0, 2.0], [1.0, 0.0]])
         >>> psnr(preds, target)
         tensor(2.5527)
 
     """
+
     is_differentiable: bool = True
     higher_is_better: bool = True
     full_state_update: bool = False
     plot_lower_bound: float = 0.0
 
     min_target: Tensor
     max_target: Tensor
```

### Comparing `torchmetrics-1.3.1/src/torchmetrics/image/psnrb.py` & `torchmetrics-1.3.2/src/torchmetrics/image/psnrb.py`

 * *Files 0% similar despite different names*

```diff
@@ -57,14 +57,15 @@
         >>> _ = torch.manual_seed(42)
         >>> preds = torch.rand(2, 1, 10, 10)
         >>> target = torch.rand(2, 1, 10, 10)
         >>> metric(preds, target)
         tensor(7.2893)
 
     """
+
     is_differentiable: bool = True
     higher_is_better: bool = True
     full_state_update: bool = False
 
     sum_squared_error: Tensor
     total: Tensor
     bef: Tensor
```

### Comparing `torchmetrics-1.3.1/src/torchmetrics/image/rase.py` & `torchmetrics-1.3.2/src/torchmetrics/image/rase.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,15 +49,15 @@
         >>> import torch
         >>> from torchmetrics.image import RelativeAverageSpectralError
         >>> g = torch.manual_seed(22)
         >>> preds = torch.rand(4, 3, 16, 16)
         >>> target = torch.rand(4, 3, 16, 16)
         >>> rase = RelativeAverageSpectralError()
         >>> rase(preds, target)
-        tensor(5114.6641)
+        tensor(5114.66...)
 
     Raises:
         ValueError: If ``window_size`` is not a positive integer.
 
     """
 
     higher_is_better: bool = False
```

### Comparing `torchmetrics-1.3.1/src/torchmetrics/image/rmse_sw.py` & `torchmetrics-1.3.2/src/torchmetrics/image/rmse_sw.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.3.1/src/torchmetrics/image/sam.py` & `torchmetrics-1.3.2/src/torchmetrics/image/sam.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.3.1/src/torchmetrics/image/scc.py` & `torchmetrics-1.3.2/src/torchmetrics/image/scc.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.3.1/src/torchmetrics/image/ssim.py` & `torchmetrics-1.3.2/src/torchmetrics/image/ssim.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.3.1/src/torchmetrics/image/tv.py` & `torchmetrics-1.3.2/src/torchmetrics/image/tv.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.3.1/src/torchmetrics/image/uqi.py` & `torchmetrics-1.3.2/src/torchmetrics/image/uqi.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.3.1/src/torchmetrics/image/vif.py` & `torchmetrics-1.3.2/src/torchmetrics/image/vif.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.3.1/src/torchmetrics/metric.py` & `torchmetrics-1.3.2/src/torchmetrics/metric.py`

 * *Files 1% similar despite different names*

```diff
@@ -104,14 +104,15 @@
         super().__init__()
 
         # see (https://github.com/pytorch/pytorch/blob/3e6bb5233f9ca2c5aa55d9cda22a7ee85439aa6e/
         # torch/nn/modules/module.py#L227)
         torch._C._log_api_usage_once(f"torchmetrics.metric.{self.__class__.__name__}")
 
         self._device = torch.device("cpu")
+        self._dtype = torch.get_default_dtype()
 
         self.compute_on_cpu = kwargs.pop("compute_on_cpu", False)
         if not isinstance(self.compute_on_cpu, bool):
             raise ValueError(
                 f"Expected keyword argument `compute_on_cpu` to be an `bool` but got {self.compute_on_cpu}"
             )
 
@@ -725,23 +726,28 @@
         super().__setattr__(name, value)
 
     @property
     def device(self) -> "torch.device":
         """Return the device of the metric."""
         return self._device
 
-    def type(self, dst_type: Union[str, torch.dtype]) -> "Metric":  # noqa: A003
+    @property
+    def dtype(self) -> "torch.dtype":
+        """Return the default dtype of the metric."""
+        return self._dtype
+
+    def type(self, dst_type: Union[str, torch.dtype]) -> "Metric":
         """Override default and prevent dtype casting.
 
         Please use :meth:`Metric.set_dtype` instead.
 
         """
         return self
 
-    def float(self) -> "Metric":  # noqa: A003
+    def float(self) -> "Metric":
         """Override default and prevent dtype casting.
 
         Please use :meth:`Metric.set_dtype` instead.
 
         """
         return self
 
@@ -809,15 +815,17 @@
             else:
                 raise TypeError(
                     f"Expected metric state to be either a Tensor or a list of Tensor, but encountered {current_val}"
                 )
 
         # make sure to update the device attribute
         # if the dummy tensor moves device by fn function we should also update the attribute
-        self._device = fn(torch.zeros(1, device=self.device)).device
+        _dummy_tensor = fn(torch.zeros(1, device=self.device))
+        self._device = _dummy_tensor.device
+        self._dtype = _dummy_tensor.dtype
 
         # Additional apply to forward cache and computed attributes (may be nested)
         if this._computed is not None:
             this._computed = apply_to_collection(this._computed, Tensor, fn)
         if this._forward_cache is not None:
             this._forward_cache = apply_to_collection(this._forward_cache, Tensor, fn)
 
@@ -841,15 +849,17 @@
                 the same object is returned. Otherwise, an ``OrderedDict`` will be created and returned.
             prefix: optional string, a prefix added to parameter and buffer names to compose the keys in state_dict.
             keep_vars: by default the :class:`~torch.Tensor` returned in the state dict are detached from autograd.
                 If set to ``True``, detaching will not be performed.
 
         """
         destination: Dict[str, Union[torch.Tensor, List, Any]] = super().state_dict(
-            destination=destination, prefix=prefix, keep_vars=keep_vars  # type: ignore[arg-type]
+            destination=destination,  # type: ignore[arg-type]
+            prefix=prefix,
+            keep_vars=keep_vars,
         )
         # Register metric states to be part of the state_dict
         for key in self._defaults:
             if not self._persistent[key]:
                 continue
             current_val = getattr(self, key)
             if not keep_vars:
```

### Comparing `torchmetrics-1.3.1/src/torchmetrics/multimodal/__init__.py` & `torchmetrics-1.3.2/src/torchmetrics/multimodal/__init__.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.3.1/src/torchmetrics/multimodal/clip_iqa.py` & `torchmetrics-1.3.2/src/torchmetrics/multimodal/clip_iqa.py`

 * *Files 0% similar despite different names*

```diff
@@ -177,15 +177,15 @@
             "openai/clip-vit-base-patch16",
             "openai/clip-vit-base-patch32",
             "openai/clip-vit-large-patch14-336",
             "openai/clip-vit-large-patch14",
         ] = "clip_iqa",
         data_range: float = 1.0,
         prompts: Tuple[Union[str, Tuple[str, str]]] = ("quality",),
-        **kwargs: Any
+        **kwargs: Any,
     ) -> None:
         super().__init__(**kwargs)
         if not (isinstance(data_range, (int, float)) and data_range > 0):
             raise ValueError("Argument `data_range` should be a positive number.")
         self.data_range = data_range
 
         prompts_list, prompts_name = _clip_iqa_format_prompts(prompts)
```

### Comparing `torchmetrics-1.3.1/src/torchmetrics/multimodal/clip_score.py` & `torchmetrics-1.3.2/src/torchmetrics/multimodal/clip_score.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.3.1/src/torchmetrics/nominal/__init__.py` & `torchmetrics-1.3.2/src/torchmetrics/nominal/__init__.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.3.1/src/torchmetrics/nominal/cramers.py` & `torchmetrics-1.3.2/src/torchmetrics/nominal/cramers.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.3.1/src/torchmetrics/nominal/fleiss_kappa.py` & `torchmetrics-1.3.2/src/torchmetrics/nominal/fleiss_kappa.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.3.1/src/torchmetrics/nominal/pearson.py` & `torchmetrics-1.3.2/src/torchmetrics/nominal/pearson.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.3.1/src/torchmetrics/nominal/theils_u.py` & `torchmetrics-1.3.2/src/torchmetrics/nominal/theils_u.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.3.1/src/torchmetrics/nominal/tschuprows.py` & `torchmetrics-1.3.2/src/torchmetrics/nominal/tschuprows.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.3.1/src/torchmetrics/regression/__init__.py` & `torchmetrics-1.3.2/src/torchmetrics/regression/__init__.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.3.1/src/torchmetrics/regression/concordance.py` & `torchmetrics-1.3.2/src/torchmetrics/regression/concordance.py`

 * *Files 0% similar despite different names*

```diff
@@ -63,14 +63,15 @@
         >>> target = tensor([[3, -0.5], [2, 7]])
         >>> preds = tensor([[2.5, 0.0], [2, 8]])
         >>> concordance = ConcordanceCorrCoef(num_outputs=2)
         >>> concordance(preds, target)
         tensor([0.7273, 0.9887])
 
     """
+
     is_differentiable: bool = True
     higher_is_better: bool = True
     full_state_update: bool = True
 
     plot_lower_bound: float = -1.0
     plot_upper_bound: float = 1.0
```

### Comparing `torchmetrics-1.3.1/src/torchmetrics/regression/cosine_similarity.py` & `torchmetrics-1.3.2/src/torchmetrics/regression/cosine_similarity.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,14 +54,15 @@
         >>> target = tensor([[0, 1], [1, 1]])
         >>> preds = tensor([[0, 1], [0, 1]])
         >>> cosine_similarity = CosineSimilarity(reduction = 'mean')
         >>> cosine_similarity(preds, target)
         tensor(0.8536)
 
     """
+
     is_differentiable: bool = True
     higher_is_better: bool = True
     full_state_update: bool = False
     plot_lower_bound: float = 0.0
     plot_upper_bound: float = 1.0
 
     preds: List[Tensor]
```

### Comparing `torchmetrics-1.3.1/src/torchmetrics/regression/csi.py` & `torchmetrics-1.3.2/src/torchmetrics/regression/csi.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.3.1/src/torchmetrics/regression/explained_variance.py` & `torchmetrics-1.3.2/src/torchmetrics/regression/explained_variance.py`

 * *Files 0% similar despite different names*

```diff
@@ -77,14 +77,15 @@
         >>> target = tensor([[0.5, 1], [-1, 1], [7, -6]])
         >>> preds = tensor([[0, 2], [-1, 2], [8, -5]])
         >>> explained_variance = ExplainedVariance(multioutput='raw_values')
         >>> explained_variance(preds, target)
         tensor([0.9677, 1.0000])
 
     """
+
     is_differentiable: bool = True
     higher_is_better: bool = True
     full_state_update: bool = False
     plot_lower_bound: float = 0.0
     plot_upper_bound: float = 1.0
 
     num_obs: Tensor
```

### Comparing `torchmetrics-1.3.1/src/torchmetrics/regression/kendall.py` & `torchmetrics-1.3.2/src/torchmetrics/regression/kendall.py`

 * *Files 2% similar despite different names*

```diff
@@ -108,14 +108,15 @@
         >>> preds = tensor([[2.5, 0.0], [2, 8]])
         >>> target = tensor([[3, -0.5], [2, 1]])
         >>> kendall = KendallRankCorrCoef(t_test=True, alternative='two-sided', num_outputs=2)
         >>> kendall(preds, target)
         (tensor([1., 1.]), tensor([nan, nan]))
 
     """
+
     is_differentiable = False
     higher_is_better = None
     full_state_update = True
     plot_lower_bound: float = 0.0
     plot_upper_bound: float = 1.0
 
     preds: List[Tensor]
@@ -153,15 +154,18 @@
         )
 
     def compute(self) -> Union[Tensor, Tuple[Tensor, Tensor]]:
         """Compute Kendall rank correlation coefficient, and optionally p-value of corresponding statistical test."""
         preds = dim_zero_cat(self.preds)
         target = dim_zero_cat(self.target)
         tau, p_value = _kendall_corrcoef_compute(
-            preds, target, self.variant, self.alternative  # type: ignore[arg-type]  # todo
+            preds,
+            target,
+            self.variant,  # type: ignore[arg-type]  # todo
+            self.alternative,  # type: ignore[arg-type]  # todo
         )
 
         if p_value is not None:
             return tau, p_value
         return tau
 
     def plot(
```

### Comparing `torchmetrics-1.3.1/src/torchmetrics/regression/kl_divergence.py` & `torchmetrics-1.3.2/src/torchmetrics/regression/kl_divergence.py`

 * *Files 0% similar despite different names*

```diff
@@ -73,14 +73,15 @@
         >>> p = tensor([[0.36, 0.48, 0.16]])
         >>> q = tensor([[1/3, 1/3, 1/3]])
         >>> kl_divergence = KLDivergence()
         >>> kl_divergence(p, q)
         tensor(0.0853)
 
     """
+
     is_differentiable: bool = True
     higher_is_better: bool = False
     full_state_update: bool = False
     plot_lower_bound: float = 0.0
 
     total: Tensor
     # FIXME: Apply once minimal torch is 1.10. For torch<=1.9, jit does not support Union types
```

### Comparing `torchmetrics-1.3.1/src/torchmetrics/regression/log_cosh.py` & `torchmetrics-1.3.2/src/torchmetrics/regression/log_cosh.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.3.1/src/torchmetrics/regression/log_mse.py` & `torchmetrics-1.3.2/src/torchmetrics/regression/log_mse.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,14 +52,15 @@
         >>> mean_squared_log_error(preds, target)
         tensor(0.0397)
 
     .. note::
         Half precision is only support on GPU for this metric
 
     """
+
     is_differentiable: bool = True
     higher_is_better: bool = False
     full_state_update: bool = False
     plot_lower_bound: float = 0.0
 
     sum_squared_log_error: Tensor
     total: Tensor
```

### Comparing `torchmetrics-1.3.1/src/torchmetrics/regression/mae.py` & `torchmetrics-1.3.2/src/torchmetrics/regression/mae.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,14 +49,15 @@
         >>> target = tensor([3.0, -0.5, 2.0, 7.0])
         >>> preds = tensor([2.5, 0.0, 2.0, 8.0])
         >>> mean_absolute_error = MeanAbsoluteError()
         >>> mean_absolute_error(preds, target)
         tensor(0.5000)
 
     """
+
     is_differentiable: bool = True
     higher_is_better: bool = False
     full_state_update: bool = False
     plot_lower_bound: float = 0.0
 
     sum_abs_error: Tensor
     total: Tensor
```

### Comparing `torchmetrics-1.3.1/src/torchmetrics/regression/mape.py` & `torchmetrics-1.3.2/src/torchmetrics/regression/mape.py`

 * *Files 0% similar despite different names*

```diff
@@ -58,14 +58,15 @@
         >>> target = tensor([1, 10, 1e6])
         >>> preds = tensor([0.9, 15, 1.2e6])
         >>> mean_abs_percentage_error = MeanAbsolutePercentageError()
         >>> mean_abs_percentage_error(preds, target)
         tensor(0.2667)
 
     """
+
     is_differentiable: bool = True
     higher_is_better: bool = False
     full_state_update: bool = False
     plot_lower_bound: float = 0.0
 
     sum_abs_per_error: Tensor
     total: Tensor
```

### Comparing `torchmetrics-1.3.1/src/torchmetrics/regression/minkowski.py` & `torchmetrics-1.3.2/src/torchmetrics/regression/minkowski.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.3.1/src/torchmetrics/regression/mse.py` & `torchmetrics-1.3.2/src/torchmetrics/regression/mse.py`

 * *Files 0% similar despite different names*

```diff
@@ -65,14 +65,15 @@
         >>> target = tensor([[0.0, 0.0, 0.0], [0.0, 0.0, 0.0]])
         >>> preds = tensor([[1.0, 2.0, 3.0], [1.0, 2.0, 3.0]])
         >>> mean_squared_error = MeanSquaredError(num_outputs=3)
         >>> mean_squared_error(preds, target)
         tensor([1., 4., 9.])
 
     """
+
     is_differentiable = True
     higher_is_better = False
     full_state_update = False
     plot_lower_bound: float = 0.0
 
     sum_squared_error: Tensor
     total: Tensor
```

### Comparing `torchmetrics-1.3.1/src/torchmetrics/regression/pearson.py` & `torchmetrics-1.3.2/src/torchmetrics/regression/pearson.py`

 * *Files 0% similar despite different names*

```diff
@@ -106,14 +106,15 @@
         >>> target = torch.tensor([[3, -0.5], [2, 7]])
         >>> preds = torch.tensor([[2.5, 0.0], [2, 8]])
         >>> pearson = PearsonCorrCoef(num_outputs=2)
         >>> pearson(preds, target)
         tensor([1., 1.])
 
     """
+
     is_differentiable: bool = True
     higher_is_better: Optional[bool] = None  # both -1 and 1 are optimal
     full_state_update: bool = True
     plot_lower_bound: float = -1.0
     plot_upper_bound: float = 1.0
     preds: List[Tensor]
     target: List[Tensor]
```

### Comparing `torchmetrics-1.3.1/src/torchmetrics/regression/r2.py` & `torchmetrics-1.3.2/src/torchmetrics/regression/r2.py`

 * *Files 0% similar despite different names*

```diff
@@ -82,14 +82,15 @@
         >>> target = torch.tensor([[0.5, 1], [-1, 1], [7, -6]])
         >>> preds = torch.tensor([[0, 2], [-1, 2], [8, -5]])
         >>> r2score = R2Score(num_outputs=2, multioutput='raw_values')
         >>> r2score(preds, target)
         tensor([0.9654, 0.9082])
 
     """
+
     is_differentiable: bool = True
     higher_is_better: bool = True
     full_state_update: bool = False
     plot_lower_bound: float = 0.0
     plot_upper_bound: float = 1.0
 
     sum_squared_error: Tensor
```

### Comparing `torchmetrics-1.3.1/src/torchmetrics/regression/rse.py` & `torchmetrics-1.3.2/src/torchmetrics/regression/rse.py`

 * *Files 0% similar despite different names*

```diff
@@ -57,14 +57,15 @@
         >>> target = torch.tensor([3, -0.5, 2, 7])
         >>> preds = torch.tensor([2.5, 0.0, 2, 8])
         >>> relative_squared_error = RelativeSquaredError()
         >>> relative_squared_error(preds, target)
         tensor(0.0514)
 
     """
+
     is_differentiable = True
     higher_is_better = False
     full_state_update = False
     sum_squared_error: Tensor
     sum_error: Tensor
     residual: Tensor
     total: Tensor
```

### Comparing `torchmetrics-1.3.1/src/torchmetrics/regression/spearman.py` & `torchmetrics-1.3.2/src/torchmetrics/regression/spearman.py`

 * *Files 4% similar despite different names*

```diff
@@ -63,14 +63,15 @@
         >>> target = tensor([[3, -0.5], [2, 7]])
         >>> preds = tensor([[2.5, 0.0], [2, 8]])
         >>> spearman = SpearmanCorrCoef(num_outputs=2)
         >>> spearman(preds, target)
         tensor([1.0000, 1.0000])
 
     """
+
     is_differentiable: bool = False
     higher_is_better: bool = True
     full_state_update: bool = False
     plot_lower_bound: float = -1.0
     plot_upper_bound: float = 1.0
 
     preds: List[Tensor]
@@ -92,16 +93,16 @@
 
         self.add_state("preds", default=[], dist_reduce_fx="cat")
         self.add_state("target", default=[], dist_reduce_fx="cat")
 
     def update(self, preds: Tensor, target: Tensor) -> None:
         """Update state with predictions and targets."""
         preds, target = _spearman_corrcoef_update(preds, target, num_outputs=self.num_outputs)
-        self.preds.append(preds)
-        self.target.append(target)
+        self.preds.append(preds.to(self.dtype))
+        self.target.append(target.to(self.dtype))
 
     def compute(self) -> Tensor:
         """Compute Spearman's correlation coefficient."""
         preds = dim_zero_cat(self.preds)
         target = dim_zero_cat(self.target)
         return _spearman_corrcoef_compute(preds, target)
```

### Comparing `torchmetrics-1.3.1/src/torchmetrics/regression/symmetric_mape.py` & `torchmetrics-1.3.2/src/torchmetrics/regression/symmetric_mape.py`

 * *Files 0% similar despite different names*

```diff
@@ -51,14 +51,15 @@
         >>> target = tensor([1, 10, 1e6])
         >>> preds = tensor([0.9, 15, 1.2e6])
         >>> smape = SymmetricMeanAbsolutePercentageError()
         >>> smape(preds, target)
         tensor(0.2290)
 
     """
+
     is_differentiable: bool = True
     higher_is_better: bool = False
     full_state_update: bool = False
     plot_lower_bound: float = 0.0
 
     sum_abs_per_error: Tensor
     total: Tensor
```

### Comparing `torchmetrics-1.3.1/src/torchmetrics/regression/tweedie_deviance.py` & `torchmetrics-1.3.2/src/torchmetrics/regression/tweedie_deviance.py`

 * *Files 0% similar despite different names*

```diff
@@ -71,14 +71,15 @@
         >>> targets = torch.tensor([1.0, 2.0, 3.0, 4.0])
         >>> preds = torch.tensor([4.0, 3.0, 2.0, 1.0])
         >>> deviance_score = TweedieDevianceScore(power=2)
         >>> deviance_score(preds, targets)
         tensor(1.2083)
 
     """
+
     is_differentiable: bool = True
     higher_is_better = None
     full_state_update: bool = False
     plot_lower_bound: float = 0.0
 
     sum_deviance_score: Tensor
     num_observations: Tensor
```

### Comparing `torchmetrics-1.3.1/src/torchmetrics/regression/wmape.py` & `torchmetrics-1.3.2/src/torchmetrics/regression/wmape.py`

 * *Files 0% similar despite different names*

```diff
@@ -56,14 +56,15 @@
         >>> preds = torch.randn(20,)
         >>> target = torch.randn(20,)
         >>> wmape = WeightedMeanAbsolutePercentageError()
         >>> wmape(preds, target)
         tensor(1.3967)
 
     """
+
     is_differentiable: bool = True
     higher_is_better: bool = False
     full_state_update: bool = False
     plot_lower_bound: float = 0.0
 
     sum_abs_error: Tensor
     sum_scale: Tensor
```

### Comparing `torchmetrics-1.3.1/src/torchmetrics/retrieval/__init__.py` & `torchmetrics-1.3.2/src/torchmetrics/retrieval/__init__.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.3.1/src/torchmetrics/retrieval/_deprecated.py` & `torchmetrics-1.3.2/src/torchmetrics/retrieval/_deprecated.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.3.1/src/torchmetrics/retrieval/auroc.py` & `torchmetrics-1.3.2/src/torchmetrics/retrieval/auroc.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.3.1/src/torchmetrics/retrieval/average_precision.py` & `torchmetrics-1.3.2/src/torchmetrics/retrieval/average_precision.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.3.1/src/torchmetrics/retrieval/base.py` & `torchmetrics-1.3.2/src/torchmetrics/retrieval/base.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.3.1/src/torchmetrics/retrieval/fall_out.py` & `torchmetrics-1.3.2/src/torchmetrics/retrieval/fall_out.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.3.1/src/torchmetrics/retrieval/hit_rate.py` & `torchmetrics-1.3.2/src/torchmetrics/retrieval/hit_rate.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.3.1/src/torchmetrics/retrieval/ndcg.py` & `torchmetrics-1.3.2/src/torchmetrics/retrieval/ndcg.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.3.1/src/torchmetrics/retrieval/precision.py` & `torchmetrics-1.3.2/src/torchmetrics/retrieval/precision.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.3.1/src/torchmetrics/retrieval/precision_recall_curve.py` & `torchmetrics-1.3.2/src/torchmetrics/retrieval/precision_recall_curve.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.3.1/src/torchmetrics/retrieval/r_precision.py` & `torchmetrics-1.3.2/src/torchmetrics/retrieval/r_precision.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.3.1/src/torchmetrics/retrieval/recall.py` & `torchmetrics-1.3.2/src/torchmetrics/retrieval/recall.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.3.1/src/torchmetrics/retrieval/reciprocal_rank.py` & `torchmetrics-1.3.2/src/torchmetrics/retrieval/reciprocal_rank.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.3.1/src/torchmetrics/text/__init__.py` & `torchmetrics-1.3.2/src/torchmetrics/text/__init__.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.3.1/src/torchmetrics/text/_deprecated.py` & `torchmetrics-1.3.2/src/torchmetrics/text/_deprecated.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.3.1/src/torchmetrics/text/bert.py` & `torchmetrics-1.3.2/src/torchmetrics/text/bert.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.3.1/src/torchmetrics/text/bleu.py` & `torchmetrics-1.3.2/src/torchmetrics/text/bleu.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.3.1/src/torchmetrics/text/cer.py` & `torchmetrics-1.3.2/src/torchmetrics/text/cer.py`

 * *Files 0% similar despite different names*

```diff
@@ -62,14 +62,15 @@
         >>> preds = ["this is the prediction", "there is an other sample"]
         >>> target = ["this is the reference", "there is another one"]
         >>> cer = CharErrorRate()
         >>> cer(preds, target)
         tensor(0.3415)
 
     """
+
     is_differentiable: bool = False
     higher_is_better: bool = False
     full_state_update: bool = False
     plot_lower_bound: float = 0.0
     plot_upper_bound: float = 1.0
 
     errors: Tensor
```

### Comparing `torchmetrics-1.3.1/src/torchmetrics/text/chrf.py` & `torchmetrics-1.3.2/src/torchmetrics/text/chrf.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.3.1/src/torchmetrics/text/edit.py` & `torchmetrics-1.3.2/src/torchmetrics/text/edit.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.3.1/src/torchmetrics/text/eed.py` & `torchmetrics-1.3.2/src/torchmetrics/text/eed.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.3.1/src/torchmetrics/text/infolm.py` & `torchmetrics-1.3.2/src/torchmetrics/text/infolm.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.3.1/src/torchmetrics/text/mer.py` & `torchmetrics-1.3.2/src/torchmetrics/text/mer.py`

 * *Files 0% similar despite different names*

```diff
@@ -59,14 +59,15 @@
         >>> preds = ["this is the prediction", "there is an other sample"]
         >>> target = ["this is the reference", "there is another one"]
         >>> mer = MatchErrorRate()
         >>> mer(preds, target)
         tensor(0.4444)
 
     """
+
     is_differentiable: bool = False
     higher_is_better: bool = False
     full_state_update: bool = False
     plot_lower_bound: float = 0.0
     plot_upper_bound: float = 1.0
 
     errors: Tensor
```

### Comparing `torchmetrics-1.3.1/src/torchmetrics/text/perplexity.py` & `torchmetrics-1.3.2/src/torchmetrics/text/perplexity.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,16 +29,16 @@
     r"""Perplexity measures how well a language model predicts a text sample.
 
     It's calculated as the average number of bits per word a model needs to represent the sample.
 
     As input to ``forward`` and ``update`` the metric accepts the following input:
 
     - ``preds`` (:class:`~torch.Tensor`): Logits or a unnormalized score assigned to each token in a sequence with shape
-        [batch_size, seq_len, vocab_size], which is the output of a language model. Scores will be normalized internally
-        using softmax.
+      [batch_size, seq_len, vocab_size], which is the output of a language model. Scores will be normalized internally
+      using softmax.
     - ``target`` (:class:`~torch.Tensor`): Ground truth values with a shape [batch_size, seq_len]
 
     As output of ``forward`` and ``compute`` the metric returns the following output:
 
     - ``perp`` (:class:`~torch.Tensor`): A tensor with the perplexity score
 
     Args:
@@ -55,14 +55,15 @@
         >>> target = torch.randint(5, (2, 8), generator=gen)
         >>> target[0, 6:] = -100
         >>> perp = Perplexity(ignore_index=-100)
         >>> perp(preds, target)
         tensor(5.8540)
 
     """
+
     is_differentiable = True
     higher_is_better = False
     full_state_update = False
     total_log_probs: Tensor
     count: Tensor
 
     def __init__(
```

### Comparing `torchmetrics-1.3.1/src/torchmetrics/text/rouge.py` & `torchmetrics-1.3.2/src/torchmetrics/text/rouge.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.3.1/src/torchmetrics/text/sacre_bleu.py` & `torchmetrics-1.3.2/src/torchmetrics/text/sacre_bleu.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.3.1/src/torchmetrics/text/squad.py` & `torchmetrics-1.3.2/src/torchmetrics/text/squad.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.3.1/src/torchmetrics/text/ter.py` & `torchmetrics-1.3.2/src/torchmetrics/text/ter.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.3.1/src/torchmetrics/text/wer.py` & `torchmetrics-1.3.2/src/torchmetrics/text/wer.py`

 * *Files 0% similar despite different names*

```diff
@@ -61,14 +61,15 @@
         >>> preds = ["this is the prediction", "there is an other sample"]
         >>> target = ["this is the reference", "there is another one"]
         >>> wer = WordErrorRate()
         >>> wer(preds, target)
         tensor(0.5000)
 
     """
+
     is_differentiable: bool = False
     higher_is_better: bool = False
     full_state_update: bool = False
     plot_lower_bound: float = 0.0
     plot_upper_bound: float = 1.0
 
     errors: Tensor
```

### Comparing `torchmetrics-1.3.1/src/torchmetrics/text/wil.py` & `torchmetrics-1.3.2/src/torchmetrics/text/wil.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,14 +57,15 @@
         >>> preds = ["this is the prediction", "there is an other sample"]
         >>> target = ["this is the reference", "there is another one"]
         >>> wil = WordInfoLost()
         >>> wil(preds, target)
         tensor(0.6528)
 
     """
+
     is_differentiable: bool = False
     higher_is_better: bool = False
     full_state_update: bool = False
     plot_lower_bound: float = 0.0
     plot_upper_bound: float = 1.0
 
     errors: Tensor
```

### Comparing `torchmetrics-1.3.1/src/torchmetrics/text/wip.py` & `torchmetrics-1.3.2/src/torchmetrics/text/wip.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 
     This value indicates the percentage of words that were correctly predicted between a set of ground-
     truth sentences and a set of hypothesis sentences. The higher the value, the better the performance of the ASR
     system with a WordInfoPreserved of 1 being a perfect score. Word Information Preserved rate can then be
     computed as:
 
     .. math::
-        wip = \frac{C}{N} + \frac{C}{P}
+        wip = \frac{C}{N} * \frac{C}{P}
 
     where:
 
         - :math:`C` is the number of correct words,
         - :math:`N` is the number of words in the reference
         - :math:`P` is the number of words in the prediction
 
@@ -58,14 +58,15 @@
         >>> preds = ["this is the prediction", "there is an other sample"]
         >>> target = ["this is the reference", "there is another one"]
         >>> wip = WordInfoPreserved()
         >>> wip(preds, target)
         tensor(0.3472)
 
     """
+
     is_differentiable: bool = False
     higher_is_better: bool = False
     full_state_update: bool = False
     plot_lower_bound: float = 0.0
     plot_upper_bound: float = 1.0
 
     errors: Tensor
```

### Comparing `torchmetrics-1.3.1/src/torchmetrics/utilities/__init__.py` & `torchmetrics-1.3.2/src/torchmetrics/utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.3.1/src/torchmetrics/utilities/checks.py` & `torchmetrics-1.3.2/src/torchmetrics/utilities/checks.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.3.1/src/torchmetrics/utilities/compute.py` & `torchmetrics-1.3.2/src/torchmetrics/utilities/compute.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,24 +52,24 @@
     denom[denom == 0.0] = 1
     num = num if num.is_floating_point() else num.float()
     denom = denom if denom.is_floating_point() else denom.float()
     return num / denom
 
 
 def _adjust_weights_safe_divide(
-    score: Tensor, average: Optional[str], multilabel: bool, tp: Tensor, fp: Tensor, fn: Tensor
+    score: Tensor, average: Optional[str], multilabel: bool, tp: Tensor, fp: Tensor, fn: Tensor, top_k: int = 1
 ) -> Tensor:
     if average is None or average == "none":
         return score
     if average == "weighted":
         weights = tp + fn
     else:
         weights = torch.ones_like(score)
         if not multilabel:
-            weights[tp + fp + fn == 0] = 0.0
+            weights[tp + fp + fn == 0 if top_k == 1 else tp + fn == 0] = 0.0
     return _safe_divide(weights * score, weights.sum(-1, keepdim=True)).sum(-1)
 
 
 def _auc_format_inputs(x: Tensor, y: Tensor) -> Tuple[Tensor, Tensor]:
     """Check that auc input is correct."""
     x = x.squeeze() if x.ndim > 1 else x
     y = y.squeeze() if y.ndim > 1 else y
@@ -88,16 +88,16 @@
 def _auc_compute_without_check(x: Tensor, y: Tensor, direction: float, axis: int = -1) -> Tensor:
     """Compute area under the curve using the trapezoidal rule.
 
     Assumes increasing or decreasing order of `x`.
 
     """
     with torch.no_grad():
-        auc_: Tensor = torch.trapz(y, x, dim=axis) * direction
-    return auc_
+        auc_score: Tensor = torch.trapz(y, x, dim=axis) * direction
+    return auc_score
 
 
 def _auc_compute(x: Tensor, y: Tensor, reorder: bool = False) -> Tensor:
     with torch.no_grad():
         if reorder:
             x, x_idx = torch.sort(x, stable=True)
             y = y[x_idx]
```

### Comparing `torchmetrics-1.3.1/src/torchmetrics/utilities/data.py` & `torchmetrics-1.3.2/src/torchmetrics/utilities/data.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.3.1/src/torchmetrics/utilities/distributed.py` & `torchmetrics-1.3.2/src/torchmetrics/utilities/distributed.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.3.1/src/torchmetrics/utilities/enums.py` & `torchmetrics-1.3.2/src/torchmetrics/utilities/enums.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.3.1/src/torchmetrics/utilities/exceptions.py` & `torchmetrics-1.3.2/src/torchmetrics/utilities/exceptions.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.3.1/src/torchmetrics/utilities/imports.py` & `torchmetrics-1.3.2/src/torchmetrics/utilities/imports.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,31 +8,29 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Import utilities."""
+
 import shutil
 import sys
 
 from lightning_utilities.core.imports import RequirementCache
-from packaging.version import Version, parse
 
 _PYTHON_VERSION = f"{sys.version_info.major}.{sys.version_info.minor}.{sys.version_info.micro}"
-_PYTHON_LOWER_3_8 = parse(_PYTHON_VERSION) < Version("3.8")
 _TORCH_LOWER_2_0 = RequirementCache("torch<2.0.0")
 _TORCH_GREATER_EQUAL_1_11 = RequirementCache("torch>=1.11.0")
 _TORCH_GREATER_EQUAL_1_12 = RequirementCache("torch>=1.12.0")
 _TORCH_GREATER_EQUAL_1_13 = RequirementCache("torch>=1.13.0")
 _TORCH_GREATER_EQUAL_2_0 = RequirementCache("torch>=2.0.0")
 _TORCH_GREATER_EQUAL_2_1 = RequirementCache("torch>=2.1.0")
 _TORCH_GREATER_EQUAL_2_2 = RequirementCache("torch>=2.2.0")
 
-_JIWER_AVAILABLE = RequirementCache("jiwer")
 _NLTK_AVAILABLE = RequirementCache("nltk")
 _ROUGE_SCORE_AVAILABLE = RequirementCache("rouge_score")
 _BERTSCORE_AVAILABLE = RequirementCache("bert_score")
 _SCIPY_AVAILABLE = RequirementCache("scipy")
 _SCIPY_GREATER_EQUAL_1_8 = RequirementCache("scipy>=1.8.0")
 _TORCH_FIDELITY_AVAILABLE = RequirementCache("torch_fidelity")
 _LPIPS_AVAILABLE = RequirementCache("lpips")
@@ -44,15 +42,14 @@
 _TRANSFORMERS_AVAILABLE = RequirementCache("transformers")
 _TRANSFORMERS_GREATER_EQUAL_4_4 = RequirementCache("transformers>=4.4.0")
 _TRANSFORMERS_GREATER_EQUAL_4_10 = RequirementCache("transformers>=4.10.0")
 _PESQ_AVAILABLE = RequirementCache("pesq")
 _GAMMATONE_AVAILABLE = RequirementCache("gammatone")
 _TORCHAUDIO_AVAILABLE = RequirementCache("torchaudio")
 _TORCHAUDIO_GREATER_EQUAL_0_10 = RequirementCache("torchaudio>=0.10.0")
-_SACREBLEU_AVAILABLE = RequirementCache("sacrebleu")
 _REGEX_AVAILABLE = RequirementCache("regex")
 _PYSTOI_AVAILABLE = RequirementCache("pystoi")
 _FAST_BSS_EVAL_AVAILABLE = RequirementCache("fast_bss_eval")
 _MATPLOTLIB_AVAILABLE = RequirementCache("matplotlib")
 _SCIENCEPLOT_AVAILABLE = RequirementCache("scienceplots")
 _MULTIPROCESSING_AVAILABLE = RequirementCache("multiprocessing")
 _XLA_AVAILABLE = RequirementCache("torch_xla")
```

### Comparing `torchmetrics-1.3.1/src/torchmetrics/utilities/plot.py` & `torchmetrics-1.3.2/src/torchmetrics/utilities/plot.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.3.1/src/torchmetrics/utilities/prints.py` & `torchmetrics-1.3.2/src/torchmetrics/utilities/prints.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.3.1/src/torchmetrics/wrappers/__init__.py` & `torchmetrics-1.3.2/src/torchmetrics/wrappers/__init__.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.3.1/src/torchmetrics/wrappers/abstract.py` & `torchmetrics-1.3.2/src/torchmetrics/wrappers/abstract.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.3.1/src/torchmetrics/wrappers/bootstrapping.py` & `torchmetrics-1.3.2/src/torchmetrics/wrappers/bootstrapping.py`

 * *Files 0% similar despite different names*

```diff
@@ -82,14 +82,15 @@
         >>> bootstrap = BootStrapper(base_metric, num_bootstraps=20)
         >>> bootstrap.update(torch.randint(5, (20,)), torch.randint(5, (20,)))
         >>> output = bootstrap.compute()
         >>> pprint(output)
         {'mean': tensor(0.2205), 'std': tensor(0.0859)}
 
     """
+
     full_state_update: Optional[bool] = True
 
     def __init__(
         self,
         base_metric: Metric,
         num_bootstraps: int = 10,
         mean: bool = True,
```

### Comparing `torchmetrics-1.3.1/src/torchmetrics/wrappers/classwise.py` & `torchmetrics-1.3.2/src/torchmetrics/wrappers/classwise.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,23 +7,27 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+import typing
 from typing import Any, Dict, List, Optional, Sequence, Union
 
 from torch import Tensor
 
 from torchmetrics.metric import Metric
 from torchmetrics.utilities.imports import _MATPLOTLIB_AVAILABLE
 from torchmetrics.utilities.plot import _AX_TYPE, _PLOT_OUT_TYPE
 from torchmetrics.wrappers.abstract import WrapperMetric
 
+if typing.TYPE_CHECKING:
+    from torch.nn import Module
+
 if not _MATPLOTLIB_AVAILABLE:
     __doctest_skip__ = ["ClasswiseWrapper.plot"]
 
 
 class ClasswiseWrapper(WrapperMetric):
     """Wrapper metric for altering the output of classification metrics.
 
@@ -205,7 +209,26 @@
             >>> values = [ ]
             >>> for _ in range(3):
             ...     values.append(metric(torch.randint(3, (20,)), torch.randint(3, (20,))))
             >>> fig_, ax_ = metric.plot(values)
 
         """
         return self._plot(val, ax)
+
+    def __getattr__(self, name: str) -> Union[Tensor, "Module"]:
+        """Get attribute from classwise wrapper."""
+        # return state from self.metric
+        if name in ["tp", "fp", "fn", "tn"]:
+            return getattr(self.metric, name)
+
+        return super().__getattr__(name)
+
+    def __setattr__(self, name: str, value: Any) -> None:
+        """Set attribute to classwise wrapper."""
+        super().__setattr__(name, value)
+        if name == "metric":
+            self._defaults = self.metric._defaults
+            self._persistent = self.metric._persistent
+            self._reductions = self.metric._reductions
+        if hasattr(self, "metric") and name in ["tp", "fp", "fn", "tn", "_update_count", "_computed"]:
+            # update ``_update_count`` and ``_computed`` of internal metric to prevent warning.
+            setattr(self.metric, name, value)
```

### Comparing `torchmetrics-1.3.1/src/torchmetrics/wrappers/feature_share.py` & `torchmetrics-1.3.2/src/torchmetrics/wrappers/feature_share.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.3.1/src/torchmetrics/wrappers/minmax.py` & `torchmetrics-1.3.2/src/torchmetrics/wrappers/minmax.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.3.1/src/torchmetrics/wrappers/multioutput.py` & `torchmetrics-1.3.2/src/torchmetrics/wrappers/multioutput.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.3.1/src/torchmetrics/wrappers/multitask.py` & `torchmetrics-1.3.2/src/torchmetrics/wrappers/multitask.py`

 * *Files 1% similar despite different names*

```diff
@@ -154,15 +154,15 @@
         for metric in task_metrics.values():
             if not (isinstance(metric, (Metric, MetricCollection))):
                 raise TypeError(
                     "Expected each task's metric to be a Metric or a MetricCollection. "
                     f"Found a metric of type {type(metric)}"
                 )
 
-    def update(self, task_preds: Dict[str, Tensor], task_targets: Dict[str, Tensor]) -> None:
+    def update(self, task_preds: Dict[str, Any], task_targets: Dict[str, Any]) -> None:
         """Update each task's metric with its corresponding pred and target.
 
         Args:
             task_preds: Dictionary associating each task to a Tensor of pred.
             task_targets: Dictionary associating each task to a Tensor of target.
 
         """
```

### Comparing `torchmetrics-1.3.1/src/torchmetrics/wrappers/running.py` & `torchmetrics-1.3.2/src/torchmetrics/wrappers/running.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.3.1/src/torchmetrics/wrappers/tracker.py` & `torchmetrics-1.3.2/src/torchmetrics/wrappers/tracker.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.3.1/src/torchmetrics.egg-info/PKG-INFO` & `torchmetrics-1.3.2/src/torchmetrics.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchmetrics
-Version: 1.3.1
+Version: 1.3.2
 Summary: PyTorch native Metrics
 Home-page: https://github.com/Lightning-AI/torchmetrics
 Download-URL: https://github.com/Lightning-AI/torchmetrics/archive/master.zip
 Author: Lightning-AI et al.
 Author-email: name@pytorchlightning.ai
 License: Apache-2.0
 Project-URL: Bug Tracker, https://github.com/Lightning-AI/torchmetrics/issues
@@ -27,140 +27,139 @@
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy>1.20.0
 Requires-Dist: packaging>17.1
 Requires-Dist: torch>=1.10.0
-Requires-Dist: torch>=1.10.0
 Requires-Dist: typing-extensions; python_version < "3.9"
 Requires-Dist: lightning-utilities>=0.8.0
 Provides-Extra: audio
-Requires-Dist: pystoi>=0.3.0; extra == "audio"
 Requires-Dist: torchaudio>=0.10.0; extra == "audio"
+Requires-Dist: pystoi>=0.3.0; extra == "audio"
 Provides-Extra: detection
-Requires-Dist: torchvision>=0.8; extra == "detection"
 Requires-Dist: pycocotools>2.0.0; extra == "detection"
+Requires-Dist: torchvision>=0.8; extra == "detection"
 Provides-Extra: image
-Requires-Dist: torchvision>=0.8; extra == "image"
 Requires-Dist: scipy>1.0.0; extra == "image"
 Requires-Dist: torch-fidelity<=0.4.0; extra == "image"
+Requires-Dist: torchvision>=0.8; extra == "image"
 Provides-Extra: multimodal
-Requires-Dist: transformers>=4.10.0; extra == "multimodal"
 Requires-Dist: piq<=0.8.0; extra == "multimodal"
+Requires-Dist: transformers>=4.10.0; extra == "multimodal"
 Provides-Extra: text
-Requires-Dist: transformers>4.4.0; extra == "text"
-Requires-Dist: mecab-python3>=1.0.6; extra == "text"
 Requires-Dist: mecab-ko>=1.0.0; extra == "text"
-Requires-Dist: sentencepiece>=0.1.98; extra == "text"
-Requires-Dist: tqdm>=4.41.0; extra == "text"
-Requires-Dist: nltk>=3.6; extra == "text"
 Requires-Dist: regex>=2021.9.24; extra == "text"
-Requires-Dist: ipadic>=1.0.0; extra == "text"
+Requires-Dist: mecab-python3>=1.0.6; extra == "text"
 Requires-Dist: mecab-ko-dic>=1.0.0; extra == "text"
+Requires-Dist: tqdm>=4.41.0; extra == "text"
+Requires-Dist: ipadic>=1.0.0; extra == "text"
+Requires-Dist: transformers>4.4.0; extra == "text"
+Requires-Dist: sentencepiece>=0.2.0; extra == "text"
+Requires-Dist: nltk>=3.6; extra == "text"
 Provides-Extra: typing
-Requires-Dist: torch==2.2.0; extra == "typing"
-Requires-Dist: types-PyYAML; extra == "typing"
-Requires-Dist: types-emoji; extra == "typing"
-Requires-Dist: types-requests; extra == "typing"
 Requires-Dist: types-setuptools; extra == "typing"
-Requires-Dist: types-six; extra == "typing"
-Requires-Dist: mypy==1.8.0; extra == "typing"
 Requires-Dist: types-tabulate; extra == "typing"
 Requires-Dist: types-protobuf; extra == "typing"
+Requires-Dist: torch==2.2.1; extra == "typing"
+Requires-Dist: types-requests; extra == "typing"
+Requires-Dist: types-PyYAML; extra == "typing"
+Requires-Dist: mypy==1.8.0; extra == "typing"
+Requires-Dist: types-emoji; extra == "typing"
+Requires-Dist: types-six; extra == "typing"
 Provides-Extra: visual
-Requires-Dist: SciencePlots>=2.0.0; extra == "visual"
 Requires-Dist: matplotlib>=3.3.0; extra == "visual"
+Requires-Dist: SciencePlots>=2.0.0; extra == "visual"
 Provides-Extra: all
-Requires-Dist: pystoi>=0.3.0; extra == "all"
 Requires-Dist: torchaudio>=0.10.0; extra == "all"
-Requires-Dist: torchvision>=0.8; extra == "all"
+Requires-Dist: pystoi>=0.3.0; extra == "all"
 Requires-Dist: pycocotools>2.0.0; extra == "all"
 Requires-Dist: torchvision>=0.8; extra == "all"
 Requires-Dist: scipy>1.0.0; extra == "all"
 Requires-Dist: torch-fidelity<=0.4.0; extra == "all"
-Requires-Dist: transformers>=4.10.0; extra == "all"
+Requires-Dist: torchvision>=0.8; extra == "all"
 Requires-Dist: piq<=0.8.0; extra == "all"
-Requires-Dist: transformers>4.4.0; extra == "all"
-Requires-Dist: mecab-python3>=1.0.6; extra == "all"
+Requires-Dist: transformers>=4.10.0; extra == "all"
 Requires-Dist: mecab-ko>=1.0.0; extra == "all"
-Requires-Dist: sentencepiece>=0.1.98; extra == "all"
-Requires-Dist: tqdm>=4.41.0; extra == "all"
-Requires-Dist: nltk>=3.6; extra == "all"
 Requires-Dist: regex>=2021.9.24; extra == "all"
-Requires-Dist: ipadic>=1.0.0; extra == "all"
+Requires-Dist: mecab-python3>=1.0.6; extra == "all"
 Requires-Dist: mecab-ko-dic>=1.0.0; extra == "all"
-Requires-Dist: torch==2.2.0; extra == "all"
-Requires-Dist: types-PyYAML; extra == "all"
-Requires-Dist: types-emoji; extra == "all"
-Requires-Dist: types-requests; extra == "all"
+Requires-Dist: tqdm>=4.41.0; extra == "all"
+Requires-Dist: ipadic>=1.0.0; extra == "all"
+Requires-Dist: transformers>4.4.0; extra == "all"
+Requires-Dist: sentencepiece>=0.2.0; extra == "all"
+Requires-Dist: nltk>=3.6; extra == "all"
 Requires-Dist: types-setuptools; extra == "all"
-Requires-Dist: types-six; extra == "all"
-Requires-Dist: mypy==1.8.0; extra == "all"
 Requires-Dist: types-tabulate; extra == "all"
 Requires-Dist: types-protobuf; extra == "all"
-Requires-Dist: SciencePlots>=2.0.0; extra == "all"
+Requires-Dist: torch==2.2.1; extra == "all"
+Requires-Dist: types-requests; extra == "all"
+Requires-Dist: types-PyYAML; extra == "all"
+Requires-Dist: mypy==1.8.0; extra == "all"
+Requires-Dist: types-emoji; extra == "all"
+Requires-Dist: types-six; extra == "all"
 Requires-Dist: matplotlib>=3.3.0; extra == "all"
+Requires-Dist: SciencePlots>=2.0.0; extra == "all"
 Provides-Extra: dev
-Requires-Dist: pystoi>=0.3.0; extra == "dev"
 Requires-Dist: torchaudio>=0.10.0; extra == "dev"
-Requires-Dist: torchvision>=0.8; extra == "dev"
+Requires-Dist: pystoi>=0.3.0; extra == "dev"
 Requires-Dist: pycocotools>2.0.0; extra == "dev"
 Requires-Dist: torchvision>=0.8; extra == "dev"
 Requires-Dist: scipy>1.0.0; extra == "dev"
 Requires-Dist: torch-fidelity<=0.4.0; extra == "dev"
-Requires-Dist: transformers>=4.10.0; extra == "dev"
+Requires-Dist: torchvision>=0.8; extra == "dev"
 Requires-Dist: piq<=0.8.0; extra == "dev"
-Requires-Dist: transformers>4.4.0; extra == "dev"
-Requires-Dist: mecab-python3>=1.0.6; extra == "dev"
+Requires-Dist: transformers>=4.10.0; extra == "dev"
 Requires-Dist: mecab-ko>=1.0.0; extra == "dev"
-Requires-Dist: sentencepiece>=0.1.98; extra == "dev"
-Requires-Dist: tqdm>=4.41.0; extra == "dev"
-Requires-Dist: nltk>=3.6; extra == "dev"
 Requires-Dist: regex>=2021.9.24; extra == "dev"
-Requires-Dist: ipadic>=1.0.0; extra == "dev"
+Requires-Dist: mecab-python3>=1.0.6; extra == "dev"
 Requires-Dist: mecab-ko-dic>=1.0.0; extra == "dev"
-Requires-Dist: torch==2.2.0; extra == "dev"
-Requires-Dist: types-PyYAML; extra == "dev"
-Requires-Dist: types-emoji; extra == "dev"
-Requires-Dist: types-requests; extra == "dev"
+Requires-Dist: tqdm>=4.41.0; extra == "dev"
+Requires-Dist: ipadic>=1.0.0; extra == "dev"
+Requires-Dist: transformers>4.4.0; extra == "dev"
+Requires-Dist: sentencepiece>=0.2.0; extra == "dev"
+Requires-Dist: nltk>=3.6; extra == "dev"
 Requires-Dist: types-setuptools; extra == "dev"
-Requires-Dist: types-six; extra == "dev"
-Requires-Dist: mypy==1.8.0; extra == "dev"
 Requires-Dist: types-tabulate; extra == "dev"
 Requires-Dist: types-protobuf; extra == "dev"
-Requires-Dist: SciencePlots>=2.0.0; extra == "dev"
+Requires-Dist: torch==2.2.1; extra == "dev"
+Requires-Dist: types-requests; extra == "dev"
+Requires-Dist: types-PyYAML; extra == "dev"
+Requires-Dist: mypy==1.8.0; extra == "dev"
+Requires-Dist: types-emoji; extra == "dev"
+Requires-Dist: types-six; extra == "dev"
 Requires-Dist: matplotlib>=3.3.0; extra == "dev"
-Requires-Dist: statsmodels>0.13.5; extra == "dev"
-Requires-Dist: torch_complex<=0.4.3; extra == "dev"
-Requires-Dist: monai==1.3.0; extra == "dev"
+Requires-Dist: SciencePlots>=2.0.0; extra == "dev"
 Requires-Dist: rouge-score>0.1.0; extra == "dev"
-Requires-Dist: fairlearn; extra == "dev"
+Requires-Dist: mir-eval>=0.6; extra == "dev"
+Requires-Dist: bert_score==0.3.13; extra == "dev"
+Requires-Dist: lpips<=0.1.4; extra == "dev"
 Requires-Dist: scikit-image>=0.19.0; extra == "dev"
+Requires-Dist: monai==1.3.0; extra == "dev"
+Requires-Dist: sewar>=0.4.4; extra == "dev"
 Requires-Dist: jiwer>=2.3.0; extra == "dev"
-Requires-Dist: pandas>=1.4.0; extra == "dev"
-Requires-Dist: fast-bss-eval>=0.1.0; extra == "dev"
-Requires-Dist: kornia>=0.6.7; extra == "dev"
-Requires-Dist: huggingface-hub<0.21; extra == "dev"
+Requires-Dist: dython<=0.7.5; extra == "dev"
+Requires-Dist: netcal>1.0.0; extra == "dev"
+Requires-Dist: torch_complex<=0.4.3; extra == "dev"
 Requires-Dist: numpy<1.25.0; extra == "dev"
-Requires-Dist: bert_score==0.3.13; extra == "dev"
-Requires-Dist: sewar>=0.4.4; extra == "dev"
-Requires-Dist: faster-coco-eval>=1.3.3; extra == "dev"
+Requires-Dist: fairlearn; extra == "dev"
+Requires-Dist: statsmodels>0.13.5; extra == "dev"
 Requires-Dist: scipy>1.0.0; extra == "dev"
-Requires-Dist: netcal>1.0.0; extra == "dev"
-Requires-Dist: dython<=0.7.5; extra == "dev"
-Requires-Dist: pandas>1.0.0; extra == "dev"
-Requires-Dist: lpips<=0.1.4; extra == "dev"
-Requires-Dist: sacrebleu>=2.3.0; extra == "dev"
-Requires-Dist: mir-eval>=0.6; extra == "dev"
+Requires-Dist: kornia>=0.6.7; extra == "dev"
+Requires-Dist: faster-coco-eval>=1.3.3; extra == "dev"
 Requires-Dist: pytorch-msssim==1.0.0; extra == "dev"
+Requires-Dist: sacrebleu>=2.3.0; extra == "dev"
+Requires-Dist: huggingface-hub<0.22; extra == "dev"
+Requires-Dist: fast-bss-eval>=0.1.0; extra == "dev"
+Requires-Dist: pandas>1.0.0; extra == "dev"
+Requires-Dist: pandas>=1.4.0; extra == "dev"
 
 <div align="center">
 
-<img src="https://github.com/Lightning-AI/torchmetrics/raw/v1.3.1/docs/source/_static/images/logo.png" width="400px">
+<img src="https://github.com/Lightning-AI/torchmetrics/raw/v1.3.2/docs/source/_static/images/logo.png" width="400px">
 
 **Machine learning metrics for distributed, scalable PyTorch applications.**
 
 ______________________________________________________________________
 
 <p align="center">
   <a href="#what-is-torchmetrics">What is Torchmetrics</a> •
@@ -177,16 +176,16 @@
 [![PyPI Status](https://badge.fury.io/py/torchmetrics.svg)](https://badge.fury.io/py/torchmetrics)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/torchmetrics)
 ](https://pepy.tech/project/torchmetrics)
 [![Conda](https://img.shields.io/conda/v/conda-forge/torchmetrics?label=conda&color=success)](https://anaconda.org/conda-forge/torchmetrics)
 [![license](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://github.com/Lightning-AI/torchmetrics/blob/master/LICENSE)
 
 [![CI testing | CPU](https://github.com/Lightning-AI/torchmetrics/actions/workflows/ci-tests.yml/badge.svg?event=push)](https://github.com/Lightning-AI/torchmetrics/actions/workflows/ci-tests.yml)
-[![Build Status](https://dev.azure.com/Lightning-AI/Metrics/_apis/build/status%2FTM.unittests?branchName=refs%2Ftags%2Fv1.3.1)](https://dev.azure.com/Lightning-AI/Metrics/_build/latest?definitionId=2&branchName=refs%2Ftags%2Fv1.3.1)
-[![codecov](https://codecov.io/gh/Lightning-AI/torchmetrics/release/v1.3.1/graph/badge.svg?token=NER6LPI3HS)](https://codecov.io/gh/Lightning-AI/torchmetrics)
+[![Build Status](https://dev.azure.com/Lightning-AI/Metrics/_apis/build/status%2FTM.unittests?branchName=refs%2Ftags%2Fv1.3.2)](https://dev.azure.com/Lightning-AI/Metrics/_build/latest?definitionId=2&branchName=refs%2Ftags%2Fv1.3.2)
+[![codecov](https://codecov.io/gh/Lightning-AI/torchmetrics/release/v1.3.2/graph/badge.svg?token=NER6LPI3HS)](https://codecov.io/gh/Lightning-AI/torchmetrics)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/Lightning-AI/torchmetrics/master.svg)](https://results.pre-commit.ci/latest/github/Lightning-AI/torchmetrics/master)
 
 [![Documentation Status](https://readthedocs.org/projects/torchmetrics/badge/?version=latest)](https://torchmetrics.readthedocs.io/en/latest/?badge=latest)
 [![Discord](https://img.shields.io/discord/1077906959069626439?style=plastic)](https://discord.gg/VptPCZkGNa)
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.5844769.svg)](https://doi.org/10.5281/zenodo.5844769)
 [![JOSS status](https://joss.theoj.org/papers/561d9bb59b400158bc8204e2639dca43/status.svg)](https://joss.theoj.org/papers/561d9bb59b400158bc8204e2639dca43)
 
@@ -483,15 +482,15 @@
 values = []
 for i in range(10):
     values.append(acc(preds(i), target(i)))
 fig3, ax3 = acc.plot(values)
 ```
 
 <p align="center">
-  <img src="https://github.com/Lightning-AI/torchmetrics/raw/v1.3.1/docs/source/_static/images/plot_example.png" width="1000">
+  <img src="https://github.com/Lightning-AI/torchmetrics/raw/v1.3.2/docs/source/_static/images/plot_example.png" width="1000">
 </p>
 
 For examples of plotting different metrics try running [this example file](examples/plotting.py).
 
 ## Contribute!
 
 The lightning + TorchMetrics team is hard at work adding even more metrics.
```

### Comparing `torchmetrics-1.3.1/src/torchmetrics.egg-info/SOURCES.txt` & `torchmetrics-1.3.2/src/torchmetrics.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -146,26 +146,26 @@
 src/torchmetrics/functional/detection/panoptic_qualities.py
 src/torchmetrics/functional/image/__init__.py
 src/torchmetrics/functional/image/_deprecated.py
 src/torchmetrics/functional/image/d_lambda.py
 src/torchmetrics/functional/image/d_s.py
 src/torchmetrics/functional/image/ergas.py
 src/torchmetrics/functional/image/gradients.py
-src/torchmetrics/functional/image/helper.py
 src/torchmetrics/functional/image/lpips.py
 src/torchmetrics/functional/image/perceptual_path_length.py
 src/torchmetrics/functional/image/psnr.py
 src/torchmetrics/functional/image/psnrb.py
 src/torchmetrics/functional/image/rase.py
 src/torchmetrics/functional/image/rmse_sw.py
 src/torchmetrics/functional/image/sam.py
 src/torchmetrics/functional/image/scc.py
 src/torchmetrics/functional/image/ssim.py
 src/torchmetrics/functional/image/tv.py
 src/torchmetrics/functional/image/uqi.py
+src/torchmetrics/functional/image/utils.py
 src/torchmetrics/functional/image/vif.py
 src/torchmetrics/functional/image/lpips_models/alex.pth
 src/torchmetrics/functional/image/lpips_models/squeeze.pth
 src/torchmetrics/functional/image/lpips_models/vgg.pth
 src/torchmetrics/functional/multimodal/__init__.py
 src/torchmetrics/functional/multimodal/clip_iqa.py
 src/torchmetrics/functional/multimodal/clip_score.py
```

### Comparing `torchmetrics-1.3.1/src/torchmetrics.egg-info/requires.txt` & `torchmetrics-1.3.2/src/torchmetrics.egg-info/requires.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,133 +1,132 @@
 numpy>1.20.0
 packaging>17.1
 torch>=1.10.0
-torch>=1.10.0
 lightning-utilities>=0.8.0
 
 [:python_version < "3.9"]
 typing-extensions
 
 [all]
-pystoi>=0.3.0
 torchaudio>=0.10.0
-torchvision>=0.8
+pystoi>=0.3.0
 pycocotools>2.0.0
+torchvision>=0.8
 scipy>1.0.0
 torch-fidelity<=0.4.0
-transformers>=4.10.0
 piq<=0.8.0
-transformers>4.4.0
-mecab-python3>=1.0.6
+transformers>=4.10.0
 mecab-ko>=1.0.0
-sentencepiece>=0.1.98
-tqdm>=4.41.0
-nltk>=3.6
 regex>=2021.9.24
-ipadic>=1.0.0
+mecab-python3>=1.0.6
 mecab-ko-dic>=1.0.0
-torch==2.2.0
-types-PyYAML
-types-emoji
-types-requests
+tqdm>=4.41.0
+ipadic>=1.0.0
+transformers>4.4.0
+sentencepiece>=0.2.0
+nltk>=3.6
 types-setuptools
-types-six
-mypy==1.8.0
 types-tabulate
 types-protobuf
-SciencePlots>=2.0.0
+torch==2.2.1
+types-requests
+types-PyYAML
+mypy==1.8.0
+types-emoji
+types-six
 matplotlib>=3.3.0
+SciencePlots>=2.0.0
 
 [audio]
-pystoi>=0.3.0
 torchaudio>=0.10.0
+pystoi>=0.3.0
 
 [detection]
-torchvision>=0.8
 pycocotools>2.0.0
+torchvision>=0.8
 
 [dev]
-pystoi>=0.3.0
 torchaudio>=0.10.0
-torchvision>=0.8
+pystoi>=0.3.0
 pycocotools>2.0.0
+torchvision>=0.8
 scipy>1.0.0
 torch-fidelity<=0.4.0
-transformers>=4.10.0
 piq<=0.8.0
-transformers>4.4.0
-mecab-python3>=1.0.6
+transformers>=4.10.0
 mecab-ko>=1.0.0
-sentencepiece>=0.1.98
-tqdm>=4.41.0
-nltk>=3.6
 regex>=2021.9.24
-ipadic>=1.0.0
+mecab-python3>=1.0.6
 mecab-ko-dic>=1.0.0
-torch==2.2.0
-types-PyYAML
-types-emoji
-types-requests
+tqdm>=4.41.0
+ipadic>=1.0.0
+transformers>4.4.0
+sentencepiece>=0.2.0
+nltk>=3.6
 types-setuptools
-types-six
-mypy==1.8.0
 types-tabulate
 types-protobuf
-SciencePlots>=2.0.0
+torch==2.2.1
+types-requests
+types-PyYAML
+mypy==1.8.0
+types-emoji
+types-six
 matplotlib>=3.3.0
-statsmodels>0.13.5
-torch_complex<=0.4.3
-monai==1.3.0
+SciencePlots>=2.0.0
 rouge-score>0.1.0
-fairlearn
+mir-eval>=0.6
+bert_score==0.3.13
+lpips<=0.1.4
 scikit-image>=0.19.0
+monai==1.3.0
+sewar>=0.4.4
 jiwer>=2.3.0
-pandas>=1.4.0
-fast-bss-eval>=0.1.0
-kornia>=0.6.7
-huggingface-hub<0.21
+dython<=0.7.5
+netcal>1.0.0
+torch_complex<=0.4.3
 numpy<1.25.0
-bert_score==0.3.13
-sewar>=0.4.4
+fairlearn
+statsmodels>0.13.5
+kornia>=0.6.7
 faster-coco-eval>=1.3.3
-netcal>1.0.0
-dython<=0.7.5
-pandas>1.0.0
-lpips<=0.1.4
-sacrebleu>=2.3.0
-mir-eval>=0.6
 pytorch-msssim==1.0.0
+sacrebleu>=2.3.0
+huggingface-hub<0.22
+fast-bss-eval>=0.1.0
+pandas>1.0.0
+pandas>=1.4.0
 
 [image]
-torchvision>=0.8
 scipy>1.0.0
 torch-fidelity<=0.4.0
+torchvision>=0.8
 
 [multimodal]
-transformers>=4.10.0
 piq<=0.8.0
+transformers>=4.10.0
 
 [text]
-transformers>4.4.0
-mecab-python3>=1.0.6
 mecab-ko>=1.0.0
-sentencepiece>=0.1.98
-tqdm>=4.41.0
-nltk>=3.6
 regex>=2021.9.24
-ipadic>=1.0.0
+mecab-python3>=1.0.6
 mecab-ko-dic>=1.0.0
+tqdm>=4.41.0
+ipadic>=1.0.0
+transformers>4.4.0
+sentencepiece>=0.2.0
+nltk>=3.6
 
 [typing]
-torch==2.2.0
-types-PyYAML
-types-emoji
-types-requests
 types-setuptools
-types-six
-mypy==1.8.0
 types-tabulate
 types-protobuf
+torch==2.2.1
+types-requests
+types-PyYAML
+mypy==1.8.0
+types-emoji
+types-six
 
 [visual]
-SciencePlots>=2.0.0
 matplotlib>=3.3.0
+SciencePlots>=2.0.0
```

