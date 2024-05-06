# Comparing `tmp/pycyclops-0.2.6.tar.gz` & `tmp/pycyclops-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycyclops-0.2.6.tar", max compression
+gzip compressed data, was "pycyclops-0.2.7.tar", max compression
```

## Comparing `pycyclops-0.2.6.tar` & `pycyclops-0.2.7.tar`

### file list

```diff
@@ -1,170 +1,170 @@
--rw-r--r--   0        0        0    11347 2024-04-10 21:12:46.385642 pycyclops-0.2.6/LICENSE.md
--rw-r--r--   0        0        0     6433 2024-04-10 21:12:46.385642 pycyclops-0.2.6/README.md
--rw-r--r--   0        0        0       23 2024-04-10 21:12:46.385642 pycyclops-0.2.6/cyclops/__init__.py
--rw-r--r--   0        0        0      192 2024-04-10 21:12:46.385642 pycyclops-0.2.6/cyclops/data/__init__.py
--rw-r--r--   0        0        0    25741 2024-04-10 21:12:46.385642 pycyclops-0.2.6/cyclops/data/aggregate.py
--rw-r--r--   0        0        0     4344 2024-04-10 21:12:46.385642 pycyclops-0.2.6/cyclops/data/clean.py
--rw-r--r--   0        0        0     3469 2024-04-10 21:12:46.385642 pycyclops-0.2.6/cyclops/data/constants.py
--rw-r--r--   0        0        0       39 2024-04-10 21:12:46.385642 pycyclops-0.2.6/cyclops/data/df/__init__.py
--rw-r--r--   0        0        0    26086 2024-04-10 21:12:46.385642 pycyclops-0.2.6/cyclops/data/df/feature.py
--rw-r--r--   0        0        0    26171 2024-04-10 21:12:46.385642 pycyclops-0.2.6/cyclops/data/df/handle_types.py
--rw-r--r--   0        0        0    17267 2024-04-10 21:12:46.385642 pycyclops-0.2.6/cyclops/data/df/normalize.py
--rw-r--r--   0        0        0    12116 2024-04-10 21:12:46.385642 pycyclops-0.2.6/cyclops/data/df/split.py
--rw-r--r--   0        0        0    30240 2024-04-10 21:12:46.385642 pycyclops-0.2.6/cyclops/data/df/vectorized.py
--rw-r--r--   0        0        0     3295 2024-04-10 21:12:46.385642 pycyclops-0.2.6/cyclops/data/diagnoses.py
--rw-r--r--   0        0        0      118 2024-04-10 21:12:46.385642 pycyclops-0.2.6/cyclops/data/features/__init__.py
--rw-r--r--   0        0        0     9640 2024-04-10 21:12:46.385642 pycyclops-0.2.6/cyclops/data/features/medical_image.py
--rw-r--r--   0        0        0    17072 2024-04-10 21:12:46.385642 pycyclops-0.2.6/cyclops/data/impute.py
--rw-r--r--   0        0        0     3228 2024-04-10 21:12:46.385642 pycyclops-0.2.6/cyclops/data/loader.py
--rw-r--r--   0        0        0      638 2024-04-10 21:12:46.385642 pycyclops-0.2.6/cyclops/data/packaged_loading_scripts/__init__.py
--rw-r--r--   0        0        0       36 2024-04-10 21:12:46.385642 pycyclops-0.2.6/cyclops/data/packaged_loading_scripts/medical_imagefolder/__init__.py
--rw-r--r--   0        0        0     2110 2024-04-10 21:12:46.385642 pycyclops-0.2.6/cyclops/data/packaged_loading_scripts/medical_imagefolder/medical_imagefolder.py
--rw-r--r--   0        0        0      881 2024-04-10 21:12:46.385642 pycyclops-0.2.6/cyclops/data/preprocess.py
--rw-r--r--   0        0        0    32163 2024-04-10 21:12:46.385642 pycyclops-0.2.6/cyclops/data/slicer.py
--rw-r--r--   0        0        0     6471 2024-04-10 21:12:46.385642 pycyclops-0.2.6/cyclops/data/string_ops.py
--rw-r--r--   0        0        0     3027 2024-04-10 21:12:46.385642 pycyclops-0.2.6/cyclops/data/transforms.py
--rw-r--r--   0        0        0    13157 2024-04-10 21:12:46.385642 pycyclops-0.2.6/cyclops/data/utils.py
--rw-r--r--   0        0        0      139 2024-04-10 21:12:46.385642 pycyclops-0.2.6/cyclops/evaluate/__init__.py
--rw-r--r--   0        0        0    12362 2024-04-10 21:12:46.385642 pycyclops-0.2.6/cyclops/evaluate/evaluator.py
--rw-r--r--   0        0        0      159 2024-04-10 21:12:46.385642 pycyclops-0.2.6/cyclops/evaluate/fairness/__init__.py
--rw-r--r--   0        0        0     1104 2024-04-10 21:12:46.389643 pycyclops-0.2.6/cyclops/evaluate/fairness/config.py
--rw-r--r--   0        0        0    36125 2024-04-10 21:12:46.389643 pycyclops-0.2.6/cyclops/evaluate/fairness/evaluator.py
--rw-r--r--   0        0        0     1837 2024-04-10 21:12:46.389643 pycyclops-0.2.6/cyclops/evaluate/metrics/__init__.py
--rw-r--r--   0        0        0    13476 2024-04-10 21:12:46.389643 pycyclops-0.2.6/cyclops/evaluate/metrics/accuracy.py
--rw-r--r--   0        0        0    13702 2024-04-10 21:12:46.389643 pycyclops-0.2.6/cyclops/evaluate/metrics/auroc.py
--rw-r--r--   0        0        0     4899 2024-04-10 21:12:46.389643 pycyclops-0.2.6/cyclops/evaluate/metrics/average_precision.py
--rw-r--r--   0        0        0     2484 2024-04-10 21:12:46.389643 pycyclops-0.2.6/cyclops/evaluate/metrics/experimental/__init__.py
--rw-r--r--   0        0        0     7774 2024-04-10 21:12:46.389643 pycyclops-0.2.6/cyclops/evaluate/metrics/experimental/_stat_scores.py
--rw-r--r--   0        0        0     7217 2024-04-10 21:12:46.389643 pycyclops-0.2.6/cyclops/evaluate/metrics/experimental/accuracy.py
--rw-r--r--   0        0        0    11290 2024-04-10 21:12:46.389643 pycyclops-0.2.6/cyclops/evaluate/metrics/experimental/auroc.py
--rw-r--r--   0        0        0    11136 2024-04-10 21:12:46.389643 pycyclops-0.2.6/cyclops/evaluate/metrics/experimental/average_precision.py
--rw-r--r--   0        0        0    12934 2024-04-10 21:12:46.389643 pycyclops-0.2.6/cyclops/evaluate/metrics/experimental/confusion_matrix.py
--rw-r--r--   0        0        0     1349 2024-04-10 21:12:46.389643 pycyclops-0.2.6/cyclops/evaluate/metrics/experimental/distributed_backends/__init__.py
--rw-r--r--   0        0        0     2066 2024-04-10 21:12:46.389643 pycyclops-0.2.6/cyclops/evaluate/metrics/experimental/distributed_backends/base.py
--rw-r--r--   0        0        0     3491 2024-04-10 21:12:46.389643 pycyclops-0.2.6/cyclops/evaluate/metrics/experimental/distributed_backends/mpi4py.py
--rw-r--r--   0        0        0     1062 2024-04-10 21:12:46.389643 pycyclops-0.2.6/cyclops/evaluate/metrics/experimental/distributed_backends/non_distributed.py
--rw-r--r--   0        0        0     3916 2024-04-10 21:12:46.389643 pycyclops-0.2.6/cyclops/evaluate/metrics/experimental/distributed_backends/torch_distributed.py
--rw-r--r--   0        0        0    17182 2024-04-10 21:12:46.389643 pycyclops-0.2.6/cyclops/evaluate/metrics/experimental/f_score.py
--rw-r--r--   0        0        0     2614 2024-04-10 21:12:46.389643 pycyclops-0.2.6/cyclops/evaluate/metrics/experimental/functional/__init__.py
--rw-r--r--   0        0        0    17136 2024-04-10 21:12:46.389643 pycyclops-0.2.6/cyclops/evaluate/metrics/experimental/functional/_stat_scores.py
--rw-r--r--   0        0        0    17396 2024-04-10 21:12:46.389643 pycyclops-0.2.6/cyclops/evaluate/metrics/experimental/functional/accuracy.py
--rw-r--r--   0        0        0    25070 2024-04-10 21:12:46.389643 pycyclops-0.2.6/cyclops/evaluate/metrics/experimental/functional/auroc.py
--rw-r--r--   0        0        0    26707 2024-04-10 21:12:46.389643 pycyclops-0.2.6/cyclops/evaluate/metrics/experimental/functional/average_precision.py
--rw-r--r--   0        0        0    27926 2024-04-10 21:12:46.389643 pycyclops-0.2.6/cyclops/evaluate/metrics/experimental/functional/confusion_matrix.py
--rw-r--r--   0        0        0    34008 2024-04-10 21:12:46.389643 pycyclops-0.2.6/cyclops/evaluate/metrics/experimental/functional/f_score.py
--rw-r--r--   0        0        0     2631 2024-04-10 21:12:46.389643 pycyclops-0.2.6/cyclops/evaluate/metrics/experimental/functional/mae.py
--rw-r--r--   0        0        0     3551 2024-04-10 21:12:46.389643 pycyclops-0.2.6/cyclops/evaluate/metrics/experimental/functional/mape.py
--rw-r--r--   0        0        0    12394 2024-04-10 21:12:46.389643 pycyclops-0.2.6/cyclops/evaluate/metrics/experimental/functional/matthews_corr_coef.py
--rw-r--r--   0        0        0     4101 2024-04-10 21:12:46.389643 pycyclops-0.2.6/cyclops/evaluate/metrics/experimental/functional/mse.py
--rw-r--r--   0        0        0    16833 2024-04-10 21:12:46.389643 pycyclops-0.2.6/cyclops/evaluate/metrics/experimental/functional/negative_predictive_value.py
--rw-r--r--   0        0        0    32246 2024-04-10 21:12:46.389643 pycyclops-0.2.6/cyclops/evaluate/metrics/experimental/functional/precision_recall.py
--rw-r--r--   0        0        0    45990 2024-04-10 21:12:46.389643 pycyclops-0.2.6/cyclops/evaluate/metrics/experimental/functional/precision_recall_curve.py
--rw-r--r--   0        0        0    25481 2024-04-10 21:12:46.389643 pycyclops-0.2.6/cyclops/evaluate/metrics/experimental/functional/roc.py
--rw-r--r--   0        0        0     3612 2024-04-10 21:12:46.389643 pycyclops-0.2.6/cyclops/evaluate/metrics/experimental/functional/smape.py
--rw-r--r--   0        0        0    16929 2024-04-10 21:12:46.389643 pycyclops-0.2.6/cyclops/evaluate/metrics/experimental/functional/specificity.py
--rw-r--r--   0        0        0     3253 2024-04-10 21:12:46.389643 pycyclops-0.2.6/cyclops/evaluate/metrics/experimental/functional/wmape.py
--rw-r--r--   0        0        0     1858 2024-04-10 21:12:46.389643 pycyclops-0.2.6/cyclops/evaluate/metrics/experimental/mae.py
--rw-r--r--   0        0        0     2498 2024-04-10 21:12:46.389643 pycyclops-0.2.6/cyclops/evaluate/metrics/experimental/mape.py
--rw-r--r--   0        0        0     6089 2024-04-10 21:12:46.389643 pycyclops-0.2.6/cyclops/evaluate/metrics/experimental/matthews_corr_coef.py
--rw-r--r--   0        0        0    26623 2024-04-10 21:12:46.389643 pycyclops-0.2.6/cyclops/evaluate/metrics/experimental/metric.py
--rw-r--r--   0        0        0    21975 2024-04-10 21:12:46.389643 pycyclops-0.2.6/cyclops/evaluate/metrics/experimental/metric_dict.py
--rw-r--r--   0        0        0     3290 2024-04-10 21:12:46.389643 pycyclops-0.2.6/cyclops/evaluate/metrics/experimental/mse.py
--rw-r--r--   0        0        0     7802 2024-04-10 21:12:46.389643 pycyclops-0.2.6/cyclops/evaluate/metrics/experimental/negative_predictive_value.py
--rw-r--r--   0        0        0    33336 2024-04-10 21:12:46.389643 pycyclops-0.2.6/cyclops/evaluate/metrics/experimental/precision_recall.py
--rw-r--r--   0        0        0    19586 2024-04-10 21:12:46.389643 pycyclops-0.2.6/cyclops/evaluate/metrics/experimental/precision_recall_curve.py
--rw-r--r--   0        0        0     9557 2024-04-10 21:12:46.389643 pycyclops-0.2.6/cyclops/evaluate/metrics/experimental/roc.py
--rw-r--r--   0        0        0     2597 2024-04-10 21:12:46.389643 pycyclops-0.2.6/cyclops/evaluate/metrics/experimental/smape.py
--rw-r--r--   0        0        0    13798 2024-04-10 21:12:46.389643 pycyclops-0.2.6/cyclops/evaluate/metrics/experimental/specificity.py
--rw-r--r--   0        0        0      546 2024-04-10 21:12:46.389643 pycyclops-0.2.6/cyclops/evaluate/metrics/experimental/utils/__init__.py
--rw-r--r--   0        0        0    36009 2024-04-10 21:12:46.393643 pycyclops-0.2.6/cyclops/evaluate/metrics/experimental/utils/ops.py
--rw-r--r--   0        0        0     9057 2024-04-10 21:12:46.393643 pycyclops-0.2.6/cyclops/evaluate/metrics/experimental/utils/types.py
--rw-r--r--   0        0        0     4589 2024-04-10 21:12:46.393643 pycyclops-0.2.6/cyclops/evaluate/metrics/experimental/utils/validation.py
--rw-r--r--   0        0        0     2727 2024-04-10 21:12:46.393643 pycyclops-0.2.6/cyclops/evaluate/metrics/experimental/wmape.py
--rw-r--r--   0        0        0    26187 2024-04-10 21:12:46.393643 pycyclops-0.2.6/cyclops/evaluate/metrics/f_beta.py
--rw-r--r--   0        0        0     1815 2024-04-10 21:12:46.393643 pycyclops-0.2.6/cyclops/evaluate/metrics/factory.py
--rw-r--r--   0        0        0     1933 2024-04-10 21:12:46.393643 pycyclops-0.2.6/cyclops/evaluate/metrics/functional/__init__.py
--rw-r--r--   0        0        0    16824 2024-04-10 21:12:46.393643 pycyclops-0.2.6/cyclops/evaluate/metrics/functional/accuracy.py
--rw-r--r--   0        0        0    22142 2024-04-10 21:12:46.393643 pycyclops-0.2.6/cyclops/evaluate/metrics/functional/auroc.py
--rw-r--r--   0        0        0     5544 2024-04-10 21:12:46.393643 pycyclops-0.2.6/cyclops/evaluate/metrics/functional/average_precision.py
--rw-r--r--   0        0        0    26687 2024-04-10 21:12:46.393643 pycyclops-0.2.6/cyclops/evaluate/metrics/functional/f_beta.py
--rw-r--r--   0        0        0    27455 2024-04-10 21:12:46.393643 pycyclops-0.2.6/cyclops/evaluate/metrics/functional/precision_recall.py
--rw-r--r--   0        0        0    37364 2024-04-10 21:12:46.393643 pycyclops-0.2.6/cyclops/evaluate/metrics/functional/precision_recall_curve.py
--rw-r--r--   0        0        0    21633 2024-04-10 21:12:46.393643 pycyclops-0.2.6/cyclops/evaluate/metrics/functional/roc.py
--rw-r--r--   0        0        0    11342 2024-04-10 21:12:46.393643 pycyclops-0.2.6/cyclops/evaluate/metrics/functional/sensitivity.py
--rw-r--r--   0        0        0    16029 2024-04-10 21:12:46.393643 pycyclops-0.2.6/cyclops/evaluate/metrics/functional/specificity.py
--rw-r--r--   0        0        0    26592 2024-04-10 21:12:46.393643 pycyclops-0.2.6/cyclops/evaluate/metrics/functional/stat_scores.py
--rw-r--r--   0        0        0    32052 2024-04-10 21:12:46.393643 pycyclops-0.2.6/cyclops/evaluate/metrics/metric.py
--rw-r--r--   0        0        0    26995 2024-04-10 21:12:46.393643 pycyclops-0.2.6/cyclops/evaluate/metrics/precision_recall.py
--rw-r--r--   0        0        0    23073 2024-04-10 21:12:46.393643 pycyclops-0.2.6/cyclops/evaluate/metrics/precision_recall_curve.py
--rw-r--r--   0        0        0    13622 2024-04-10 21:12:46.393643 pycyclops-0.2.6/cyclops/evaluate/metrics/roc.py
--rw-r--r--   0        0        0    12350 2024-04-10 21:12:46.393643 pycyclops-0.2.6/cyclops/evaluate/metrics/sensitivity.py
--rw-r--r--   0        0        0    14376 2024-04-10 21:12:46.393643 pycyclops-0.2.6/cyclops/evaluate/metrics/specificity.py
--rw-r--r--   0        0        0    16991 2024-04-10 21:12:46.393643 pycyclops-0.2.6/cyclops/evaluate/metrics/stat_scores.py
--rw-r--r--   0        0        0    10157 2024-04-10 21:12:46.393643 pycyclops-0.2.6/cyclops/evaluate/metrics/utils.py
--rw-r--r--   0        0        0     2388 2024-04-10 21:12:46.393643 pycyclops-0.2.6/cyclops/evaluate/utils.py
--rw-r--r--   0        0        0     1658 2024-04-10 21:12:46.393643 pycyclops-0.2.6/cyclops/models/__init__.py
--rw-r--r--   0        0        0     7660 2024-04-10 21:12:46.393643 pycyclops-0.2.6/cyclops/models/catalog.py
--rw-r--r--   0        0        0      727 2024-04-10 21:12:46.393643 pycyclops-0.2.6/cyclops/models/configs/densenet.yaml
--rw-r--r--   0        0        0      647 2024-04-10 21:12:46.393643 pycyclops-0.2.6/cyclops/models/configs/gru.yaml
--rw-r--r--   0        0        0       34 2024-04-10 21:12:46.393643 pycyclops-0.2.6/cyclops/models/configs/logistic_regression.yaml
--rw-r--r--   0        0        0      647 2024-04-10 21:12:46.393643 pycyclops-0.2.6/cyclops/models/configs/lstm.yaml
--rw-r--r--   0        0        0      117 2024-04-10 21:12:46.393643 pycyclops-0.2.6/cyclops/models/configs/mlp_classifier.yaml
--rw-r--r--   0        0        0      577 2024-04-10 21:12:46.393643 pycyclops-0.2.6/cyclops/models/configs/mlp_pt.yaml
--rw-r--r--   0        0        0      512 2024-04-10 21:12:46.393643 pycyclops-0.2.6/cyclops/models/configs/resnet.yaml
--rw-r--r--   0        0        0       53 2024-04-10 21:12:46.393643 pycyclops-0.2.6/cyclops/models/configs/rf_classifier.yaml
--rw-r--r--   0        0        0      590 2024-04-10 21:12:46.393643 pycyclops-0.2.6/cyclops/models/configs/rnn.yaml
--rw-r--r--   0        0        0       91 2024-04-10 21:12:46.393643 pycyclops-0.2.6/cyclops/models/configs/sgd_classifier.yaml
--rw-r--r--   0        0        0      180 2024-04-10 21:12:46.393643 pycyclops-0.2.6/cyclops/models/configs/xgb_classifier.yaml
--rw-r--r--   0        0        0     1791 2024-04-10 21:12:46.393643 pycyclops-0.2.6/cyclops/models/data.py
--rw-r--r--   0        0        0      266 2024-04-10 21:12:46.393643 pycyclops-0.2.6/cyclops/models/neural_nets/__init__.py
--rw-r--r--   0        0        0     2226 2024-04-10 21:12:46.393643 pycyclops-0.2.6/cyclops/models/neural_nets/gru.py
--rw-r--r--   0        0        0     2436 2024-04-10 21:12:46.393643 pycyclops-0.2.6/cyclops/models/neural_nets/lstm.py
--rw-r--r--   0        0        0     3013 2024-04-10 21:12:46.393643 pycyclops-0.2.6/cyclops/models/neural_nets/mlp.py
--rw-r--r--   0        0        0     2214 2024-04-10 21:12:46.393643 pycyclops-0.2.6/cyclops/models/neural_nets/rnn.py
--rw-r--r--   0        0        0     2588 2024-04-10 21:12:46.393643 pycyclops-0.2.6/cyclops/models/plotter.py
--rw-r--r--   0        0        0     7171 2024-04-10 21:12:46.393643 pycyclops-0.2.6/cyclops/models/torch_utils.py
--rw-r--r--   0        0        0     4371 2024-04-10 21:12:46.393643 pycyclops-0.2.6/cyclops/models/utils.py
--rw-r--r--   0        0        0      372 2024-04-10 21:12:46.393643 pycyclops-0.2.6/cyclops/models/wrappers/__init__.py
--rw-r--r--   0        0        0    10026 2024-04-10 21:12:46.393643 pycyclops-0.2.6/cyclops/models/wrappers/base.py
--rw-r--r--   0        0        0    49399 2024-04-10 21:12:46.393643 pycyclops-0.2.6/cyclops/models/wrappers/pt_model.py
--rw-r--r--   0        0        0    39968 2024-04-10 21:12:46.393643 pycyclops-0.2.6/cyclops/models/wrappers/sk_model.py
--rw-r--r--   0        0        0     9899 2024-04-10 21:12:46.393643 pycyclops-0.2.6/cyclops/models/wrappers/utils.py
--rw-r--r--   0        0        0      468 2024-04-10 21:12:46.393643 pycyclops-0.2.6/cyclops/monitor/__init__.py
--rw-r--r--   0        0        0    16172 2024-04-10 21:12:46.393643 pycyclops-0.2.6/cyclops/monitor/clinical_applicator.py
--rw-r--r--   0        0        0    13248 2024-04-10 21:12:46.397643 pycyclops-0.2.6/cyclops/monitor/detector.py
--rw-r--r--   0        0        0     2554 2024-04-10 21:12:46.397643 pycyclops-0.2.6/cyclops/monitor/explainer.py
--rw-r--r--   0        0        0    13859 2024-04-10 21:12:46.397643 pycyclops-0.2.6/cyclops/monitor/plotter.py
--rw-r--r--   0        0        0     9566 2024-04-10 21:12:46.397643 pycyclops-0.2.6/cyclops/monitor/reductor.py
--rw-r--r--   0        0        0     9118 2024-04-10 21:12:46.397643 pycyclops-0.2.6/cyclops/monitor/synthetic_applicator.py
--rw-r--r--   0        0        0    37496 2024-04-10 21:12:46.397643 pycyclops-0.2.6/cyclops/monitor/tester.py
--rw-r--r--   0        0        0    18561 2024-04-10 21:12:46.397643 pycyclops-0.2.6/cyclops/monitor/utils.py
--rw-r--r--   0        0        0       81 2024-04-10 21:12:46.397643 pycyclops-0.2.6/cyclops/report/__init__.py
--rw-r--r--   0        0        0      100 2024-04-10 21:12:46.397643 pycyclops-0.2.6/cyclops/report/model_card/__init__.py
--rw-r--r--   0        0        0     6005 2024-04-10 21:12:46.397643 pycyclops-0.2.6/cyclops/report/model_card/base.py
--rw-r--r--   0        0        0    18872 2024-04-10 21:12:46.397643 pycyclops-0.2.6/cyclops/report/model_card/fields.py
--rw-r--r--   0        0        0     3054 2024-04-10 21:12:46.397643 pycyclops-0.2.6/cyclops/report/model_card/model_card.py
--rw-r--r--   0        0        0     6166 2024-04-10 21:12:46.397643 pycyclops-0.2.6/cyclops/report/model_card/sections.py
--rw-r--r--   0        0        0       37 2024-04-10 21:12:46.397643 pycyclops-0.2.6/cyclops/report/plot/__init__.py
--rw-r--r--   0        0        0     3275 2024-04-10 21:12:46.397643 pycyclops-0.2.6/cyclops/report/plot/base.py
--rw-r--r--   0        0        0    47331 2024-04-10 21:12:46.397643 pycyclops-0.2.6/cyclops/report/plot/classification.py
--rw-r--r--   0        0        0     5463 2024-04-10 21:12:46.397643 pycyclops-0.2.6/cyclops/report/plot/utils.py
--rw-r--r--   0        0        0    39651 2024-04-10 21:12:46.397643 pycyclops-0.2.6/cyclops/report/report.py
--rw-r--r--   0        0        0     1828 2024-04-10 21:12:46.397643 pycyclops-0.2.6/cyclops/report/templates/model_report/button.js
--rw-r--r--   0        0        0    15741 2024-04-10 21:12:46.397643 pycyclops-0.2.6/cyclops/report/templates/model_report/macros.jinja
--rw-r--r--   0        0        0    14849 2024-04-10 21:12:46.397643 pycyclops-0.2.6/cyclops/report/templates/model_report/model_report.jinja
--rw-r--r--   0        0        0    30509 2024-04-10 21:12:46.397643 pycyclops-0.2.6/cyclops/report/templates/model_report/plot.js
--rw-r--r--   0        0        0    33209 2024-04-10 21:12:46.397643 pycyclops-0.2.6/cyclops/report/utils.py
--rw-r--r--   0        0        0      143 2024-04-10 21:12:46.397643 pycyclops-0.2.6/cyclops/tasks/__init__.py
--rw-r--r--   0        0        0     7447 2024-04-10 21:12:46.397643 pycyclops-0.2.6/cyclops/tasks/base.py
--rw-r--r--   0        0        0    22027 2024-04-10 21:12:46.397643 pycyclops-0.2.6/cyclops/tasks/classification.py
--rw-r--r--   0        0        0     4211 2024-04-10 21:12:46.397643 pycyclops-0.2.6/cyclops/tasks/utils.py
--rw-r--r--   0        0        0       23 2024-04-10 21:12:46.397643 pycyclops-0.2.6/cyclops/utils/__init__.py
--rw-r--r--   0        0        0     4966 2024-04-10 21:12:46.397643 pycyclops-0.2.6/cyclops/utils/common.py
--rw-r--r--   0        0        0    10240 2024-04-10 21:12:46.397643 pycyclops-0.2.6/cyclops/utils/file.py
--rw-r--r--   0        0        0     2423 2024-04-10 21:12:46.397643 pycyclops-0.2.6/cyclops/utils/index.py
--rw-r--r--   0        0        0     3611 2024-04-10 21:12:46.397643 pycyclops-0.2.6/cyclops/utils/log.py
--rw-r--r--   0        0        0     1701 2024-04-10 21:12:46.397643 pycyclops-0.2.6/cyclops/utils/optional.py
--rw-r--r--   0        0        0     5571 2024-04-10 21:12:46.397643 pycyclops-0.2.6/cyclops/utils/plot.py
--rw-r--r--   0        0        0      874 2024-04-10 21:12:46.397643 pycyclops-0.2.6/cyclops/utils/profile.py
--rw-r--r--   0        0        0     6350 2024-04-10 21:12:46.409643 pycyclops-0.2.6/pyproject.toml
--rw-r--r--   0        0        0     8864 1970-01-01 00:00:00.000000 pycyclops-0.2.6/PKG-INFO
+-rw-r--r--   0        0        0    11347 2024-05-06 13:04:25.205522 pycyclops-0.2.7/LICENSE.md
+-rw-r--r--   0        0        0     6440 2024-05-06 13:04:25.205522 pycyclops-0.2.7/README.md
+-rw-r--r--   0        0        0       23 2024-05-06 13:04:25.209522 pycyclops-0.2.7/cyclops/__init__.py
+-rw-r--r--   0        0        0      192 2024-05-06 13:04:25.209522 pycyclops-0.2.7/cyclops/data/__init__.py
+-rw-r--r--   0        0        0    25741 2024-05-06 13:04:25.209522 pycyclops-0.2.7/cyclops/data/aggregate.py
+-rw-r--r--   0        0        0     4344 2024-05-06 13:04:25.209522 pycyclops-0.2.7/cyclops/data/clean.py
+-rw-r--r--   0        0        0     3469 2024-05-06 13:04:25.209522 pycyclops-0.2.7/cyclops/data/constants.py
+-rw-r--r--   0        0        0       39 2024-05-06 13:04:25.209522 pycyclops-0.2.7/cyclops/data/df/__init__.py
+-rw-r--r--   0        0        0    26086 2024-05-06 13:04:25.209522 pycyclops-0.2.7/cyclops/data/df/feature.py
+-rw-r--r--   0        0        0    26171 2024-05-06 13:04:25.209522 pycyclops-0.2.7/cyclops/data/df/handle_types.py
+-rw-r--r--   0        0        0    17267 2024-05-06 13:04:25.209522 pycyclops-0.2.7/cyclops/data/df/normalize.py
+-rw-r--r--   0        0        0    12116 2024-05-06 13:04:25.209522 pycyclops-0.2.7/cyclops/data/df/split.py
+-rw-r--r--   0        0        0    30240 2024-05-06 13:04:25.209522 pycyclops-0.2.7/cyclops/data/df/vectorized.py
+-rw-r--r--   0        0        0     3295 2024-05-06 13:04:25.209522 pycyclops-0.2.7/cyclops/data/diagnoses.py
+-rw-r--r--   0        0        0      118 2024-05-06 13:04:25.209522 pycyclops-0.2.7/cyclops/data/features/__init__.py
+-rw-r--r--   0        0        0     9640 2024-05-06 13:04:25.209522 pycyclops-0.2.7/cyclops/data/features/medical_image.py
+-rw-r--r--   0        0        0    17072 2024-05-06 13:04:25.209522 pycyclops-0.2.7/cyclops/data/impute.py
+-rw-r--r--   0        0        0     3228 2024-05-06 13:04:25.209522 pycyclops-0.2.7/cyclops/data/loader.py
+-rw-r--r--   0        0        0      638 2024-05-06 13:04:25.209522 pycyclops-0.2.7/cyclops/data/packaged_loading_scripts/__init__.py
+-rw-r--r--   0        0        0       36 2024-05-06 13:04:25.209522 pycyclops-0.2.7/cyclops/data/packaged_loading_scripts/medical_imagefolder/__init__.py
+-rw-r--r--   0        0        0     2110 2024-05-06 13:04:25.209522 pycyclops-0.2.7/cyclops/data/packaged_loading_scripts/medical_imagefolder/medical_imagefolder.py
+-rw-r--r--   0        0        0      881 2024-05-06 13:04:25.209522 pycyclops-0.2.7/cyclops/data/preprocess.py
+-rw-r--r--   0        0        0    32163 2024-05-06 13:04:25.209522 pycyclops-0.2.7/cyclops/data/slicer.py
+-rw-r--r--   0        0        0     6471 2024-05-06 13:04:25.209522 pycyclops-0.2.7/cyclops/data/string_ops.py
+-rw-r--r--   0        0        0     3027 2024-05-06 13:04:25.209522 pycyclops-0.2.7/cyclops/data/transforms.py
+-rw-r--r--   0        0        0    13157 2024-05-06 13:04:25.209522 pycyclops-0.2.7/cyclops/data/utils.py
+-rw-r--r--   0        0        0      139 2024-05-06 13:04:25.209522 pycyclops-0.2.7/cyclops/evaluate/__init__.py
+-rw-r--r--   0        0        0    12362 2024-05-06 13:04:25.209522 pycyclops-0.2.7/cyclops/evaluate/evaluator.py
+-rw-r--r--   0        0        0      159 2024-05-06 13:04:25.209522 pycyclops-0.2.7/cyclops/evaluate/fairness/__init__.py
+-rw-r--r--   0        0        0     1104 2024-05-06 13:04:25.209522 pycyclops-0.2.7/cyclops/evaluate/fairness/config.py
+-rw-r--r--   0        0        0    36125 2024-05-06 13:04:25.209522 pycyclops-0.2.7/cyclops/evaluate/fairness/evaluator.py
+-rw-r--r--   0        0        0     1837 2024-05-06 13:04:25.209522 pycyclops-0.2.7/cyclops/evaluate/metrics/__init__.py
+-rw-r--r--   0        0        0    13476 2024-05-06 13:04:25.209522 pycyclops-0.2.7/cyclops/evaluate/metrics/accuracy.py
+-rw-r--r--   0        0        0    13702 2024-05-06 13:04:25.209522 pycyclops-0.2.7/cyclops/evaluate/metrics/auroc.py
+-rw-r--r--   0        0        0     4899 2024-05-06 13:04:25.209522 pycyclops-0.2.7/cyclops/evaluate/metrics/average_precision.py
+-rw-r--r--   0        0        0     2484 2024-05-06 13:04:25.209522 pycyclops-0.2.7/cyclops/evaluate/metrics/experimental/__init__.py
+-rw-r--r--   0        0        0     7774 2024-05-06 13:04:25.209522 pycyclops-0.2.7/cyclops/evaluate/metrics/experimental/_stat_scores.py
+-rw-r--r--   0        0        0     7217 2024-05-06 13:04:25.209522 pycyclops-0.2.7/cyclops/evaluate/metrics/experimental/accuracy.py
+-rw-r--r--   0        0        0    11290 2024-05-06 13:04:25.209522 pycyclops-0.2.7/cyclops/evaluate/metrics/experimental/auroc.py
+-rw-r--r--   0        0        0    11136 2024-05-06 13:04:25.209522 pycyclops-0.2.7/cyclops/evaluate/metrics/experimental/average_precision.py
+-rw-r--r--   0        0        0    12934 2024-05-06 13:04:25.209522 pycyclops-0.2.7/cyclops/evaluate/metrics/experimental/confusion_matrix.py
+-rw-r--r--   0        0        0     1349 2024-05-06 13:04:25.209522 pycyclops-0.2.7/cyclops/evaluate/metrics/experimental/distributed_backends/__init__.py
+-rw-r--r--   0        0        0     2066 2024-05-06 13:04:25.209522 pycyclops-0.2.7/cyclops/evaluate/metrics/experimental/distributed_backends/base.py
+-rw-r--r--   0        0        0     3491 2024-05-06 13:04:25.209522 pycyclops-0.2.7/cyclops/evaluate/metrics/experimental/distributed_backends/mpi4py.py
+-rw-r--r--   0        0        0     1062 2024-05-06 13:04:25.209522 pycyclops-0.2.7/cyclops/evaluate/metrics/experimental/distributed_backends/non_distributed.py
+-rw-r--r--   0        0        0     3916 2024-05-06 13:04:25.209522 pycyclops-0.2.7/cyclops/evaluate/metrics/experimental/distributed_backends/torch_distributed.py
+-rw-r--r--   0        0        0    17182 2024-05-06 13:04:25.209522 pycyclops-0.2.7/cyclops/evaluate/metrics/experimental/f_score.py
+-rw-r--r--   0        0        0     2614 2024-05-06 13:04:25.209522 pycyclops-0.2.7/cyclops/evaluate/metrics/experimental/functional/__init__.py
+-rw-r--r--   0        0        0    17136 2024-05-06 13:04:25.209522 pycyclops-0.2.7/cyclops/evaluate/metrics/experimental/functional/_stat_scores.py
+-rw-r--r--   0        0        0    17396 2024-05-06 13:04:25.213522 pycyclops-0.2.7/cyclops/evaluate/metrics/experimental/functional/accuracy.py
+-rw-r--r--   0        0        0    25070 2024-05-06 13:04:25.213522 pycyclops-0.2.7/cyclops/evaluate/metrics/experimental/functional/auroc.py
+-rw-r--r--   0        0        0    26707 2024-05-06 13:04:25.213522 pycyclops-0.2.7/cyclops/evaluate/metrics/experimental/functional/average_precision.py
+-rw-r--r--   0        0        0    27926 2024-05-06 13:04:25.213522 pycyclops-0.2.7/cyclops/evaluate/metrics/experimental/functional/confusion_matrix.py
+-rw-r--r--   0        0        0    34008 2024-05-06 13:04:25.213522 pycyclops-0.2.7/cyclops/evaluate/metrics/experimental/functional/f_score.py
+-rw-r--r--   0        0        0     2631 2024-05-06 13:04:25.213522 pycyclops-0.2.7/cyclops/evaluate/metrics/experimental/functional/mae.py
+-rw-r--r--   0        0        0     3551 2024-05-06 13:04:25.213522 pycyclops-0.2.7/cyclops/evaluate/metrics/experimental/functional/mape.py
+-rw-r--r--   0        0        0    12394 2024-05-06 13:04:25.213522 pycyclops-0.2.7/cyclops/evaluate/metrics/experimental/functional/matthews_corr_coef.py
+-rw-r--r--   0        0        0     4101 2024-05-06 13:04:25.213522 pycyclops-0.2.7/cyclops/evaluate/metrics/experimental/functional/mse.py
+-rw-r--r--   0        0        0    16833 2024-05-06 13:04:25.213522 pycyclops-0.2.7/cyclops/evaluate/metrics/experimental/functional/negative_predictive_value.py
+-rw-r--r--   0        0        0    32246 2024-05-06 13:04:25.213522 pycyclops-0.2.7/cyclops/evaluate/metrics/experimental/functional/precision_recall.py
+-rw-r--r--   0        0        0    45990 2024-05-06 13:04:25.213522 pycyclops-0.2.7/cyclops/evaluate/metrics/experimental/functional/precision_recall_curve.py
+-rw-r--r--   0        0        0    25481 2024-05-06 13:04:25.213522 pycyclops-0.2.7/cyclops/evaluate/metrics/experimental/functional/roc.py
+-rw-r--r--   0        0        0     3612 2024-05-06 13:04:25.213522 pycyclops-0.2.7/cyclops/evaluate/metrics/experimental/functional/smape.py
+-rw-r--r--   0        0        0    16929 2024-05-06 13:04:25.213522 pycyclops-0.2.7/cyclops/evaluate/metrics/experimental/functional/specificity.py
+-rw-r--r--   0        0        0     3253 2024-05-06 13:04:25.213522 pycyclops-0.2.7/cyclops/evaluate/metrics/experimental/functional/wmape.py
+-rw-r--r--   0        0        0     1858 2024-05-06 13:04:25.213522 pycyclops-0.2.7/cyclops/evaluate/metrics/experimental/mae.py
+-rw-r--r--   0        0        0     2498 2024-05-06 13:04:25.213522 pycyclops-0.2.7/cyclops/evaluate/metrics/experimental/mape.py
+-rw-r--r--   0        0        0     6089 2024-05-06 13:04:25.213522 pycyclops-0.2.7/cyclops/evaluate/metrics/experimental/matthews_corr_coef.py
+-rw-r--r--   0        0        0    26623 2024-05-06 13:04:25.213522 pycyclops-0.2.7/cyclops/evaluate/metrics/experimental/metric.py
+-rw-r--r--   0        0        0    22036 2024-05-06 13:04:25.213522 pycyclops-0.2.7/cyclops/evaluate/metrics/experimental/metric_dict.py
+-rw-r--r--   0        0        0     3290 2024-05-06 13:04:25.213522 pycyclops-0.2.7/cyclops/evaluate/metrics/experimental/mse.py
+-rw-r--r--   0        0        0     7802 2024-05-06 13:04:25.213522 pycyclops-0.2.7/cyclops/evaluate/metrics/experimental/negative_predictive_value.py
+-rw-r--r--   0        0        0    33336 2024-05-06 13:04:25.213522 pycyclops-0.2.7/cyclops/evaluate/metrics/experimental/precision_recall.py
+-rw-r--r--   0        0        0    19586 2024-05-06 13:04:25.213522 pycyclops-0.2.7/cyclops/evaluate/metrics/experimental/precision_recall_curve.py
+-rw-r--r--   0        0        0     9557 2024-05-06 13:04:25.213522 pycyclops-0.2.7/cyclops/evaluate/metrics/experimental/roc.py
+-rw-r--r--   0        0        0     2597 2024-05-06 13:04:25.213522 pycyclops-0.2.7/cyclops/evaluate/metrics/experimental/smape.py
+-rw-r--r--   0        0        0    13798 2024-05-06 13:04:25.213522 pycyclops-0.2.7/cyclops/evaluate/metrics/experimental/specificity.py
+-rw-r--r--   0        0        0      546 2024-05-06 13:04:25.213522 pycyclops-0.2.7/cyclops/evaluate/metrics/experimental/utils/__init__.py
+-rw-r--r--   0        0        0    36009 2024-05-06 13:04:25.213522 pycyclops-0.2.7/cyclops/evaluate/metrics/experimental/utils/ops.py
+-rw-r--r--   0        0        0     9057 2024-05-06 13:04:25.213522 pycyclops-0.2.7/cyclops/evaluate/metrics/experimental/utils/types.py
+-rw-r--r--   0        0        0     4589 2024-05-06 13:04:25.213522 pycyclops-0.2.7/cyclops/evaluate/metrics/experimental/utils/validation.py
+-rw-r--r--   0        0        0     2727 2024-05-06 13:04:25.213522 pycyclops-0.2.7/cyclops/evaluate/metrics/experimental/wmape.py
+-rw-r--r--   0        0        0    26187 2024-05-06 13:04:25.213522 pycyclops-0.2.7/cyclops/evaluate/metrics/f_beta.py
+-rw-r--r--   0        0        0     1815 2024-05-06 13:04:25.213522 pycyclops-0.2.7/cyclops/evaluate/metrics/factory.py
+-rw-r--r--   0        0        0     1933 2024-05-06 13:04:25.213522 pycyclops-0.2.7/cyclops/evaluate/metrics/functional/__init__.py
+-rw-r--r--   0        0        0    16824 2024-05-06 13:04:25.213522 pycyclops-0.2.7/cyclops/evaluate/metrics/functional/accuracy.py
+-rw-r--r--   0        0        0    22142 2024-05-06 13:04:25.213522 pycyclops-0.2.7/cyclops/evaluate/metrics/functional/auroc.py
+-rw-r--r--   0        0        0     5544 2024-05-06 13:04:25.213522 pycyclops-0.2.7/cyclops/evaluate/metrics/functional/average_precision.py
+-rw-r--r--   0        0        0    26687 2024-05-06 13:04:25.213522 pycyclops-0.2.7/cyclops/evaluate/metrics/functional/f_beta.py
+-rw-r--r--   0        0        0    27455 2024-05-06 13:04:25.213522 pycyclops-0.2.7/cyclops/evaluate/metrics/functional/precision_recall.py
+-rw-r--r--   0        0        0    37364 2024-05-06 13:04:25.213522 pycyclops-0.2.7/cyclops/evaluate/metrics/functional/precision_recall_curve.py
+-rw-r--r--   0        0        0    21633 2024-05-06 13:04:25.213522 pycyclops-0.2.7/cyclops/evaluate/metrics/functional/roc.py
+-rw-r--r--   0        0        0    11342 2024-05-06 13:04:25.213522 pycyclops-0.2.7/cyclops/evaluate/metrics/functional/sensitivity.py
+-rw-r--r--   0        0        0    16029 2024-05-06 13:04:25.213522 pycyclops-0.2.7/cyclops/evaluate/metrics/functional/specificity.py
+-rw-r--r--   0        0        0    26592 2024-05-06 13:04:25.213522 pycyclops-0.2.7/cyclops/evaluate/metrics/functional/stat_scores.py
+-rw-r--r--   0        0        0    32052 2024-05-06 13:04:25.217522 pycyclops-0.2.7/cyclops/evaluate/metrics/metric.py
+-rw-r--r--   0        0        0    26995 2024-05-06 13:04:25.217522 pycyclops-0.2.7/cyclops/evaluate/metrics/precision_recall.py
+-rw-r--r--   0        0        0    23073 2024-05-06 13:04:25.217522 pycyclops-0.2.7/cyclops/evaluate/metrics/precision_recall_curve.py
+-rw-r--r--   0        0        0    13622 2024-05-06 13:04:25.217522 pycyclops-0.2.7/cyclops/evaluate/metrics/roc.py
+-rw-r--r--   0        0        0    12350 2024-05-06 13:04:25.217522 pycyclops-0.2.7/cyclops/evaluate/metrics/sensitivity.py
+-rw-r--r--   0        0        0    14376 2024-05-06 13:04:25.217522 pycyclops-0.2.7/cyclops/evaluate/metrics/specificity.py
+-rw-r--r--   0        0        0    16991 2024-05-06 13:04:25.217522 pycyclops-0.2.7/cyclops/evaluate/metrics/stat_scores.py
+-rw-r--r--   0        0        0    10157 2024-05-06 13:04:25.217522 pycyclops-0.2.7/cyclops/evaluate/metrics/utils.py
+-rw-r--r--   0        0        0     2388 2024-05-06 13:04:25.217522 pycyclops-0.2.7/cyclops/evaluate/utils.py
+-rw-r--r--   0        0        0     1658 2024-05-06 13:04:25.217522 pycyclops-0.2.7/cyclops/models/__init__.py
+-rw-r--r--   0        0        0     7660 2024-05-06 13:04:25.217522 pycyclops-0.2.7/cyclops/models/catalog.py
+-rw-r--r--   0        0        0      727 2024-05-06 13:04:25.217522 pycyclops-0.2.7/cyclops/models/configs/densenet.yaml
+-rw-r--r--   0        0        0      647 2024-05-06 13:04:25.217522 pycyclops-0.2.7/cyclops/models/configs/gru.yaml
+-rw-r--r--   0        0        0       34 2024-05-06 13:04:25.217522 pycyclops-0.2.7/cyclops/models/configs/logistic_regression.yaml
+-rw-r--r--   0        0        0      647 2024-05-06 13:04:25.217522 pycyclops-0.2.7/cyclops/models/configs/lstm.yaml
+-rw-r--r--   0        0        0      117 2024-05-06 13:04:25.217522 pycyclops-0.2.7/cyclops/models/configs/mlp_classifier.yaml
+-rw-r--r--   0        0        0      577 2024-05-06 13:04:25.217522 pycyclops-0.2.7/cyclops/models/configs/mlp_pt.yaml
+-rw-r--r--   0        0        0      512 2024-05-06 13:04:25.217522 pycyclops-0.2.7/cyclops/models/configs/resnet.yaml
+-rw-r--r--   0        0        0       53 2024-05-06 13:04:25.217522 pycyclops-0.2.7/cyclops/models/configs/rf_classifier.yaml
+-rw-r--r--   0        0        0      590 2024-05-06 13:04:25.217522 pycyclops-0.2.7/cyclops/models/configs/rnn.yaml
+-rw-r--r--   0        0        0       91 2024-05-06 13:04:25.217522 pycyclops-0.2.7/cyclops/models/configs/sgd_classifier.yaml
+-rw-r--r--   0        0        0      180 2024-05-06 13:04:25.217522 pycyclops-0.2.7/cyclops/models/configs/xgb_classifier.yaml
+-rw-r--r--   0        0        0     1791 2024-05-06 13:04:25.217522 pycyclops-0.2.7/cyclops/models/data.py
+-rw-r--r--   0        0        0      266 2024-05-06 13:04:25.217522 pycyclops-0.2.7/cyclops/models/neural_nets/__init__.py
+-rw-r--r--   0        0        0     2226 2024-05-06 13:04:25.217522 pycyclops-0.2.7/cyclops/models/neural_nets/gru.py
+-rw-r--r--   0        0        0     2436 2024-05-06 13:04:25.217522 pycyclops-0.2.7/cyclops/models/neural_nets/lstm.py
+-rw-r--r--   0        0        0     3013 2024-05-06 13:04:25.217522 pycyclops-0.2.7/cyclops/models/neural_nets/mlp.py
+-rw-r--r--   0        0        0     2214 2024-05-06 13:04:25.217522 pycyclops-0.2.7/cyclops/models/neural_nets/rnn.py
+-rw-r--r--   0        0        0     2588 2024-05-06 13:04:25.217522 pycyclops-0.2.7/cyclops/models/plotter.py
+-rw-r--r--   0        0        0     7238 2024-05-06 13:04:25.217522 pycyclops-0.2.7/cyclops/models/torch_utils.py
+-rw-r--r--   0        0        0     4371 2024-05-06 13:04:25.217522 pycyclops-0.2.7/cyclops/models/utils.py
+-rw-r--r--   0        0        0      372 2024-05-06 13:04:25.217522 pycyclops-0.2.7/cyclops/models/wrappers/__init__.py
+-rw-r--r--   0        0        0    10026 2024-05-06 13:04:25.217522 pycyclops-0.2.7/cyclops/models/wrappers/base.py
+-rw-r--r--   0        0        0    49399 2024-05-06 13:04:25.217522 pycyclops-0.2.7/cyclops/models/wrappers/pt_model.py
+-rw-r--r--   0        0        0    39968 2024-05-06 13:04:25.217522 pycyclops-0.2.7/cyclops/models/wrappers/sk_model.py
+-rw-r--r--   0        0        0     9899 2024-05-06 13:04:25.217522 pycyclops-0.2.7/cyclops/models/wrappers/utils.py
+-rw-r--r--   0        0        0      468 2024-05-06 13:04:25.217522 pycyclops-0.2.7/cyclops/monitor/__init__.py
+-rw-r--r--   0        0        0    16172 2024-05-06 13:04:25.217522 pycyclops-0.2.7/cyclops/monitor/clinical_applicator.py
+-rw-r--r--   0        0        0    13248 2024-05-06 13:04:25.217522 pycyclops-0.2.7/cyclops/monitor/detector.py
+-rw-r--r--   0        0        0     2554 2024-05-06 13:04:25.217522 pycyclops-0.2.7/cyclops/monitor/explainer.py
+-rw-r--r--   0        0        0    13859 2024-05-06 13:04:25.217522 pycyclops-0.2.7/cyclops/monitor/plotter.py
+-rw-r--r--   0        0        0     9566 2024-05-06 13:04:25.217522 pycyclops-0.2.7/cyclops/monitor/reductor.py
+-rw-r--r--   0        0        0     9118 2024-05-06 13:04:25.217522 pycyclops-0.2.7/cyclops/monitor/synthetic_applicator.py
+-rw-r--r--   0        0        0    37496 2024-05-06 13:04:25.217522 pycyclops-0.2.7/cyclops/monitor/tester.py
+-rw-r--r--   0        0        0    18561 2024-05-06 13:04:25.217522 pycyclops-0.2.7/cyclops/monitor/utils.py
+-rw-r--r--   0        0        0       81 2024-05-06 13:04:25.217522 pycyclops-0.2.7/cyclops/report/__init__.py
+-rw-r--r--   0        0        0      100 2024-05-06 13:04:25.217522 pycyclops-0.2.7/cyclops/report/model_card/__init__.py
+-rw-r--r--   0        0        0     6005 2024-05-06 13:04:25.217522 pycyclops-0.2.7/cyclops/report/model_card/base.py
+-rw-r--r--   0        0        0    18872 2024-05-06 13:04:25.217522 pycyclops-0.2.7/cyclops/report/model_card/fields.py
+-rw-r--r--   0        0        0     3054 2024-05-06 13:04:25.217522 pycyclops-0.2.7/cyclops/report/model_card/model_card.py
+-rw-r--r--   0        0        0     6166 2024-05-06 13:04:25.217522 pycyclops-0.2.7/cyclops/report/model_card/sections.py
+-rw-r--r--   0        0        0       37 2024-05-06 13:04:25.221522 pycyclops-0.2.7/cyclops/report/plot/__init__.py
+-rw-r--r--   0        0        0     3275 2024-05-06 13:04:25.221522 pycyclops-0.2.7/cyclops/report/plot/base.py
+-rw-r--r--   0        0        0    47331 2024-05-06 13:04:25.221522 pycyclops-0.2.7/cyclops/report/plot/classification.py
+-rw-r--r--   0        0        0     5463 2024-05-06 13:04:25.221522 pycyclops-0.2.7/cyclops/report/plot/utils.py
+-rw-r--r--   0        0        0    39651 2024-05-06 13:04:25.221522 pycyclops-0.2.7/cyclops/report/report.py
+-rw-r--r--   0        0        0     1828 2024-05-06 13:04:25.221522 pycyclops-0.2.7/cyclops/report/templates/model_report/button.js
+-rw-r--r--   0        0        0    15741 2024-05-06 13:04:25.221522 pycyclops-0.2.7/cyclops/report/templates/model_report/macros.jinja
+-rw-r--r--   0        0        0    14849 2024-05-06 13:04:25.221522 pycyclops-0.2.7/cyclops/report/templates/model_report/model_report.jinja
+-rw-r--r--   0        0        0    30509 2024-05-06 13:04:25.221522 pycyclops-0.2.7/cyclops/report/templates/model_report/plot.js
+-rw-r--r--   0        0        0    33209 2024-05-06 13:04:25.221522 pycyclops-0.2.7/cyclops/report/utils.py
+-rw-r--r--   0        0        0      143 2024-05-06 13:04:25.221522 pycyclops-0.2.7/cyclops/tasks/__init__.py
+-rw-r--r--   0        0        0     7447 2024-05-06 13:04:25.221522 pycyclops-0.2.7/cyclops/tasks/base.py
+-rw-r--r--   0        0        0    22027 2024-05-06 13:04:25.221522 pycyclops-0.2.7/cyclops/tasks/classification.py
+-rw-r--r--   0        0        0     4211 2024-05-06 13:04:25.221522 pycyclops-0.2.7/cyclops/tasks/utils.py
+-rw-r--r--   0        0        0       23 2024-05-06 13:04:25.221522 pycyclops-0.2.7/cyclops/utils/__init__.py
+-rw-r--r--   0        0        0     4966 2024-05-06 13:04:25.221522 pycyclops-0.2.7/cyclops/utils/common.py
+-rw-r--r--   0        0        0    10240 2024-05-06 13:04:25.221522 pycyclops-0.2.7/cyclops/utils/file.py
+-rw-r--r--   0        0        0     2423 2024-05-06 13:04:25.221522 pycyclops-0.2.7/cyclops/utils/index.py
+-rw-r--r--   0        0        0     3611 2024-05-06 13:04:25.221522 pycyclops-0.2.7/cyclops/utils/log.py
+-rw-r--r--   0        0        0     2294 2024-05-06 13:04:25.221522 pycyclops-0.2.7/cyclops/utils/optional.py
+-rw-r--r--   0        0        0     5571 2024-05-06 13:04:25.221522 pycyclops-0.2.7/cyclops/utils/plot.py
+-rw-r--r--   0        0        0      874 2024-05-06 13:04:25.221522 pycyclops-0.2.7/cyclops/utils/profile.py
+-rw-r--r--   0        0        0     6427 2024-05-06 13:04:25.229522 pycyclops-0.2.7/pyproject.toml
+-rw-r--r--   0        0        0     8871 1970-01-01 00:00:00.000000 pycyclops-0.2.7/PKG-INFO
```

### Comparing `pycyclops-0.2.6/LICENSE.md` & `pycyclops-0.2.7/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.6/README.md` & `pycyclops-0.2.7/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 ``cyclops`` is a toolkit for facilitating research and deployment of ML models for healthcare. It provides a few high-level APIs namely:
 
 * `data` - Create datasets for training, inference and evaluation. We use the popular 🤗 [datasets](https://github.com/huggingface/datasets) to efficiently load and slice different modalities of data
 * `models` - Use common model implementations using [scikit-learn](https://scikit-learn.org/stable/) and [PyTorch](https://pytorch.org/)
 * `tasks` - Use common ML task formulations such as binary classification or multi-label classification on tabular, time-series and image data
 * `evaluate` - Evaluate models on clinical prediction tasks
 * `monitor` - Detect dataset shift relevant for clinical use cases
-* `report` - Create [model report cards](https://vectorinstitute.github.io/cyclops/api/tutorials/nihcxr/nihcxr_report_periodic.html) for clinical ML models
+* `report` - Create [model report cards](https://vectorinstitute.github.io/cyclops/api/tutorials/kaggle/heart_failure_report_periodic.html) for clinical ML models
 
 ``cyclops`` also provides example end-to-end use case implementations on clinical datasets such as
 
 * [NIH chest x-ray](https://www.nih.gov/news-events/news-releases/nih-clinical-center-provides-one-largest-publicly-available-chest-x-ray-datasets-scientific-community)
 * [MIMIC-IV](https://physionet.org/content/mimiciv/2.0/)
```

### Comparing `pycyclops-0.2.6/cyclops/data/aggregate.py` & `pycyclops-0.2.7/cyclops/data/aggregate.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.6/cyclops/data/clean.py` & `pycyclops-0.2.7/cyclops/data/clean.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.6/cyclops/data/constants.py` & `pycyclops-0.2.7/cyclops/data/constants.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.6/cyclops/data/df/feature.py` & `pycyclops-0.2.7/cyclops/data/df/feature.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.6/cyclops/data/df/handle_types.py` & `pycyclops-0.2.7/cyclops/data/df/handle_types.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.6/cyclops/data/df/normalize.py` & `pycyclops-0.2.7/cyclops/data/df/normalize.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.6/cyclops/data/df/split.py` & `pycyclops-0.2.7/cyclops/data/df/split.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.6/cyclops/data/df/vectorized.py` & `pycyclops-0.2.7/cyclops/data/df/vectorized.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.6/cyclops/data/diagnoses.py` & `pycyclops-0.2.7/cyclops/data/diagnoses.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.6/cyclops/data/features/medical_image.py` & `pycyclops-0.2.7/cyclops/data/features/medical_image.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.6/cyclops/data/impute.py` & `pycyclops-0.2.7/cyclops/data/impute.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.6/cyclops/data/loader.py` & `pycyclops-0.2.7/cyclops/data/loader.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.6/cyclops/data/packaged_loading_scripts/__init__.py` & `pycyclops-0.2.7/cyclops/data/packaged_loading_scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.6/cyclops/data/packaged_loading_scripts/medical_imagefolder/medical_imagefolder.py` & `pycyclops-0.2.7/cyclops/data/packaged_loading_scripts/medical_imagefolder/medical_imagefolder.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.6/cyclops/data/preprocess.py` & `pycyclops-0.2.7/cyclops/data/preprocess.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.6/cyclops/data/slicer.py` & `pycyclops-0.2.7/cyclops/data/slicer.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.6/cyclops/data/string_ops.py` & `pycyclops-0.2.7/cyclops/data/string_ops.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.6/cyclops/data/transforms.py` & `pycyclops-0.2.7/cyclops/data/transforms.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.6/cyclops/data/utils.py` & `pycyclops-0.2.7/cyclops/data/utils.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.6/cyclops/evaluate/evaluator.py` & `pycyclops-0.2.7/cyclops/evaluate/evaluator.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.6/cyclops/evaluate/fairness/config.py` & `pycyclops-0.2.7/cyclops/evaluate/fairness/config.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.6/cyclops/evaluate/fairness/evaluator.py` & `pycyclops-0.2.7/cyclops/evaluate/fairness/evaluator.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.6/cyclops/evaluate/metrics/__init__.py` & `pycyclops-0.2.7/cyclops/evaluate/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.6/cyclops/evaluate/metrics/accuracy.py` & `pycyclops-0.2.7/cyclops/evaluate/metrics/accuracy.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.6/cyclops/evaluate/metrics/auroc.py` & `pycyclops-0.2.7/cyclops/evaluate/metrics/auroc.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.6/cyclops/evaluate/metrics/average_precision.py` & `pycyclops-0.2.7/cyclops/evaluate/metrics/average_precision.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.6/cyclops/evaluate/metrics/experimental/__init__.py` & `pycyclops-0.2.7/cyclops/evaluate/metrics/experimental/__init__.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.6/cyclops/evaluate/metrics/experimental/_stat_scores.py` & `pycyclops-0.2.7/cyclops/evaluate/metrics/experimental/_stat_scores.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.6/cyclops/evaluate/metrics/experimental/accuracy.py` & `pycyclops-0.2.7/cyclops/evaluate/metrics/experimental/accuracy.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.6/cyclops/evaluate/metrics/experimental/auroc.py` & `pycyclops-0.2.7/cyclops/evaluate/metrics/experimental/auroc.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.6/cyclops/evaluate/metrics/experimental/average_precision.py` & `pycyclops-0.2.7/cyclops/evaluate/metrics/experimental/average_precision.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.6/cyclops/evaluate/metrics/experimental/confusion_matrix.py` & `pycyclops-0.2.7/cyclops/evaluate/metrics/experimental/confusion_matrix.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.6/cyclops/evaluate/metrics/experimental/distributed_backends/__init__.py` & `pycyclops-0.2.7/cyclops/evaluate/metrics/experimental/distributed_backends/__init__.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.6/cyclops/evaluate/metrics/experimental/distributed_backends/base.py` & `pycyclops-0.2.7/cyclops/evaluate/metrics/experimental/distributed_backends/base.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.6/cyclops/evaluate/metrics/experimental/distributed_backends/mpi4py.py` & `pycyclops-0.2.7/cyclops/evaluate/metrics/experimental/distributed_backends/mpi4py.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.6/cyclops/evaluate/metrics/experimental/distributed_backends/non_distributed.py` & `pycyclops-0.2.7/cyclops/evaluate/metrics/experimental/distributed_backends/non_distributed.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.6/cyclops/evaluate/metrics/experimental/distributed_backends/torch_distributed.py` & `pycyclops-0.2.7/cyclops/evaluate/metrics/experimental/distributed_backends/torch_distributed.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.6/cyclops/evaluate/metrics/experimental/f_score.py` & `pycyclops-0.2.7/cyclops/evaluate/metrics/experimental/f_score.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.6/cyclops/evaluate/metrics/experimental/functional/__init__.py` & `pycyclops-0.2.7/cyclops/evaluate/metrics/experimental/functional/__init__.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.6/cyclops/evaluate/metrics/experimental/functional/_stat_scores.py` & `pycyclops-0.2.7/cyclops/evaluate/metrics/experimental/functional/_stat_scores.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.6/cyclops/evaluate/metrics/experimental/functional/accuracy.py` & `pycyclops-0.2.7/cyclops/evaluate/metrics/experimental/functional/accuracy.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.6/cyclops/evaluate/metrics/experimental/functional/auroc.py` & `pycyclops-0.2.7/cyclops/evaluate/metrics/experimental/functional/auroc.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.6/cyclops/evaluate/metrics/experimental/functional/average_precision.py` & `pycyclops-0.2.7/cyclops/evaluate/metrics/experimental/functional/average_precision.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.6/cyclops/evaluate/metrics/experimental/functional/confusion_matrix.py` & `pycyclops-0.2.7/cyclops/evaluate/metrics/experimental/functional/confusion_matrix.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.6/cyclops/evaluate/metrics/experimental/functional/f_score.py` & `pycyclops-0.2.7/cyclops/evaluate/metrics/experimental/functional/f_score.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.6/cyclops/evaluate/metrics/experimental/functional/mae.py` & `pycyclops-0.2.7/cyclops/evaluate/metrics/experimental/functional/mae.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.6/cyclops/evaluate/metrics/experimental/functional/mape.py` & `pycyclops-0.2.7/cyclops/evaluate/metrics/experimental/functional/mape.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.6/cyclops/evaluate/metrics/experimental/functional/matthews_corr_coef.py` & `pycyclops-0.2.7/cyclops/evaluate/metrics/experimental/functional/matthews_corr_coef.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.6/cyclops/evaluate/metrics/experimental/functional/mse.py` & `pycyclops-0.2.7/cyclops/evaluate/metrics/experimental/functional/mse.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.6/cyclops/evaluate/metrics/experimental/functional/negative_predictive_value.py` & `pycyclops-0.2.7/cyclops/evaluate/metrics/experimental/functional/negative_predictive_value.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.6/cyclops/evaluate/metrics/experimental/functional/precision_recall.py` & `pycyclops-0.2.7/cyclops/evaluate/metrics/experimental/functional/precision_recall.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.6/cyclops/evaluate/metrics/experimental/functional/precision_recall_curve.py` & `pycyclops-0.2.7/cyclops/evaluate/metrics/experimental/functional/precision_recall_curve.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.6/cyclops/evaluate/metrics/experimental/functional/roc.py` & `pycyclops-0.2.7/cyclops/evaluate/metrics/experimental/functional/roc.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.6/cyclops/evaluate/metrics/experimental/functional/smape.py` & `pycyclops-0.2.7/cyclops/evaluate/metrics/experimental/functional/smape.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.6/cyclops/evaluate/metrics/experimental/functional/specificity.py` & `pycyclops-0.2.7/cyclops/evaluate/metrics/experimental/functional/specificity.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.6/cyclops/evaluate/metrics/experimental/functional/wmape.py` & `pycyclops-0.2.7/cyclops/evaluate/metrics/experimental/functional/wmape.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.6/cyclops/evaluate/metrics/experimental/mae.py` & `pycyclops-0.2.7/cyclops/evaluate/metrics/experimental/mae.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.6/cyclops/evaluate/metrics/experimental/mape.py` & `pycyclops-0.2.7/cyclops/evaluate/metrics/experimental/mape.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.6/cyclops/evaluate/metrics/experimental/matthews_corr_coef.py` & `pycyclops-0.2.7/cyclops/evaluate/metrics/experimental/matthews_corr_coef.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.6/cyclops/evaluate/metrics/experimental/metric.py` & `pycyclops-0.2.7/cyclops/evaluate/metrics/experimental/metric.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.6/cyclops/evaluate/metrics/experimental/metric_dict.py` & `pycyclops-0.2.7/cyclops/evaluate/metrics/experimental/metric_dict.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,14 +34,16 @@
     from torchmetrics.metric import Metric as TorchMetric
 else:
     TorchMetric = import_optional_module(
         "torchmetrics.metric",
         attribute="Metric",
         error="ignore",
     )
+    if TorchMetric is None:
+        TorchMetric = type(None)
 
 
 LOGGER = logging.getLogger(__name__)
 setup_logging(print_level="WARN", logger=LOGGER)
 
 
 class ArrayEncoder(json.JSONEncoder):
```

### Comparing `pycyclops-0.2.6/cyclops/evaluate/metrics/experimental/mse.py` & `pycyclops-0.2.7/cyclops/evaluate/metrics/experimental/mse.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.6/cyclops/evaluate/metrics/experimental/negative_predictive_value.py` & `pycyclops-0.2.7/cyclops/evaluate/metrics/experimental/negative_predictive_value.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.6/cyclops/evaluate/metrics/experimental/precision_recall.py` & `pycyclops-0.2.7/cyclops/evaluate/metrics/experimental/precision_recall.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.6/cyclops/evaluate/metrics/experimental/precision_recall_curve.py` & `pycyclops-0.2.7/cyclops/evaluate/metrics/experimental/precision_recall_curve.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.6/cyclops/evaluate/metrics/experimental/roc.py` & `pycyclops-0.2.7/cyclops/evaluate/metrics/experimental/roc.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.6/cyclops/evaluate/metrics/experimental/smape.py` & `pycyclops-0.2.7/cyclops/evaluate/metrics/experimental/smape.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.6/cyclops/evaluate/metrics/experimental/specificity.py` & `pycyclops-0.2.7/cyclops/evaluate/metrics/experimental/specificity.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.6/cyclops/evaluate/metrics/experimental/utils/__init__.py` & `pycyclops-0.2.7/cyclops/evaluate/metrics/experimental/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.6/cyclops/evaluate/metrics/experimental/utils/ops.py` & `pycyclops-0.2.7/cyclops/evaluate/metrics/experimental/utils/ops.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.6/cyclops/evaluate/metrics/experimental/utils/types.py` & `pycyclops-0.2.7/cyclops/evaluate/metrics/experimental/utils/types.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.6/cyclops/evaluate/metrics/experimental/utils/validation.py` & `pycyclops-0.2.7/cyclops/evaluate/metrics/experimental/utils/validation.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.6/cyclops/evaluate/metrics/experimental/wmape.py` & `pycyclops-0.2.7/cyclops/evaluate/metrics/experimental/wmape.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.6/cyclops/evaluate/metrics/f_beta.py` & `pycyclops-0.2.7/cyclops/evaluate/metrics/f_beta.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.6/cyclops/evaluate/metrics/factory.py` & `pycyclops-0.2.7/cyclops/evaluate/metrics/factory.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.6/cyclops/evaluate/metrics/functional/__init__.py` & `pycyclops-0.2.7/cyclops/evaluate/metrics/functional/__init__.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.6/cyclops/evaluate/metrics/functional/accuracy.py` & `pycyclops-0.2.7/cyclops/evaluate/metrics/functional/accuracy.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.6/cyclops/evaluate/metrics/functional/auroc.py` & `pycyclops-0.2.7/cyclops/evaluate/metrics/functional/auroc.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.6/cyclops/evaluate/metrics/functional/average_precision.py` & `pycyclops-0.2.7/cyclops/evaluate/metrics/functional/average_precision.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.6/cyclops/evaluate/metrics/functional/f_beta.py` & `pycyclops-0.2.7/cyclops/evaluate/metrics/functional/f_beta.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.6/cyclops/evaluate/metrics/functional/precision_recall.py` & `pycyclops-0.2.7/cyclops/evaluate/metrics/functional/precision_recall.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.6/cyclops/evaluate/metrics/functional/precision_recall_curve.py` & `pycyclops-0.2.7/cyclops/evaluate/metrics/functional/precision_recall_curve.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.6/cyclops/evaluate/metrics/functional/roc.py` & `pycyclops-0.2.7/cyclops/evaluate/metrics/functional/roc.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.6/cyclops/evaluate/metrics/functional/sensitivity.py` & `pycyclops-0.2.7/cyclops/evaluate/metrics/functional/sensitivity.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.6/cyclops/evaluate/metrics/functional/specificity.py` & `pycyclops-0.2.7/cyclops/evaluate/metrics/functional/specificity.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.6/cyclops/evaluate/metrics/functional/stat_scores.py` & `pycyclops-0.2.7/cyclops/evaluate/metrics/functional/stat_scores.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.6/cyclops/evaluate/metrics/metric.py` & `pycyclops-0.2.7/cyclops/evaluate/metrics/metric.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.6/cyclops/evaluate/metrics/precision_recall.py` & `pycyclops-0.2.7/cyclops/evaluate/metrics/precision_recall.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.6/cyclops/evaluate/metrics/precision_recall_curve.py` & `pycyclops-0.2.7/cyclops/evaluate/metrics/precision_recall_curve.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.6/cyclops/evaluate/metrics/roc.py` & `pycyclops-0.2.7/cyclops/evaluate/metrics/roc.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.6/cyclops/evaluate/metrics/sensitivity.py` & `pycyclops-0.2.7/cyclops/evaluate/metrics/sensitivity.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.6/cyclops/evaluate/metrics/specificity.py` & `pycyclops-0.2.7/cyclops/evaluate/metrics/specificity.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.6/cyclops/evaluate/metrics/stat_scores.py` & `pycyclops-0.2.7/cyclops/evaluate/metrics/stat_scores.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.6/cyclops/evaluate/metrics/utils.py` & `pycyclops-0.2.7/cyclops/evaluate/metrics/utils.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.6/cyclops/evaluate/utils.py` & `pycyclops-0.2.7/cyclops/evaluate/utils.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.6/cyclops/models/__init__.py` & `pycyclops-0.2.7/cyclops/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.6/cyclops/models/catalog.py` & `pycyclops-0.2.7/cyclops/models/catalog.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.6/cyclops/models/configs/densenet.yaml` & `pycyclops-0.2.7/cyclops/models/configs/densenet.yaml`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.6/cyclops/models/configs/gru.yaml` & `pycyclops-0.2.7/cyclops/models/configs/gru.yaml`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.6/cyclops/models/configs/lstm.yaml` & `pycyclops-0.2.7/cyclops/models/configs/lstm.yaml`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.6/cyclops/models/configs/mlp_pt.yaml` & `pycyclops-0.2.7/cyclops/models/configs/mlp_pt.yaml`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.6/cyclops/models/configs/resnet.yaml` & `pycyclops-0.2.7/cyclops/models/configs/resnet.yaml`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.6/cyclops/models/configs/rnn.yaml` & `pycyclops-0.2.7/cyclops/models/configs/rnn.yaml`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.6/cyclops/models/data.py` & `pycyclops-0.2.7/cyclops/models/data.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.6/cyclops/models/neural_nets/gru.py` & `pycyclops-0.2.7/cyclops/models/neural_nets/gru.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.6/cyclops/models/neural_nets/lstm.py` & `pycyclops-0.2.7/cyclops/models/neural_nets/lstm.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.6/cyclops/models/neural_nets/mlp.py` & `pycyclops-0.2.7/cyclops/models/neural_nets/mlp.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.6/cyclops/models/neural_nets/rnn.py` & `pycyclops-0.2.7/cyclops/models/neural_nets/rnn.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.6/cyclops/models/plotter.py` & `pycyclops-0.2.7/cyclops/models/plotter.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.6/cyclops/models/torch_utils.py` & `pycyclops-0.2.7/cyclops/models/torch_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,14 +17,16 @@
     torch = import_optional_module("torch", error="warn")
     nn = import_optional_module("torch.nn", error="warn")
     PackedSequence = import_optional_module(
         "torch.nn.utils.rnn",
         attribute="PackedSequence",
         error="warn",
     )
+    if PackedSequence is None:
+        PackedSequence = type(None)
 
 
 def _get_class_members(
     module,
     include_only: Optional[List[str]] = None,
     exclude: Optional[List[str]] = None,
 ) -> dict:
```

### Comparing `pycyclops-0.2.6/cyclops/models/utils.py` & `pycyclops-0.2.7/cyclops/models/utils.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.6/cyclops/models/wrappers/base.py` & `pycyclops-0.2.7/cyclops/models/wrappers/base.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.6/cyclops/models/wrappers/pt_model.py` & `pycyclops-0.2.7/cyclops/models/wrappers/pt_model.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.6/cyclops/models/wrappers/sk_model.py` & `pycyclops-0.2.7/cyclops/models/wrappers/sk_model.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.6/cyclops/models/wrappers/utils.py` & `pycyclops-0.2.7/cyclops/models/wrappers/utils.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.6/cyclops/monitor/clinical_applicator.py` & `pycyclops-0.2.7/cyclops/monitor/clinical_applicator.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.6/cyclops/monitor/detector.py` & `pycyclops-0.2.7/cyclops/monitor/detector.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.6/cyclops/monitor/explainer.py` & `pycyclops-0.2.7/cyclops/monitor/explainer.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.6/cyclops/monitor/plotter.py` & `pycyclops-0.2.7/cyclops/monitor/plotter.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.6/cyclops/monitor/reductor.py` & `pycyclops-0.2.7/cyclops/monitor/reductor.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.6/cyclops/monitor/synthetic_applicator.py` & `pycyclops-0.2.7/cyclops/monitor/synthetic_applicator.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.6/cyclops/monitor/tester.py` & `pycyclops-0.2.7/cyclops/monitor/tester.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.6/cyclops/monitor/utils.py` & `pycyclops-0.2.7/cyclops/monitor/utils.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.6/cyclops/report/model_card/base.py` & `pycyclops-0.2.7/cyclops/report/model_card/base.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.6/cyclops/report/model_card/fields.py` & `pycyclops-0.2.7/cyclops/report/model_card/fields.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.6/cyclops/report/model_card/model_card.py` & `pycyclops-0.2.7/cyclops/report/model_card/model_card.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.6/cyclops/report/model_card/sections.py` & `pycyclops-0.2.7/cyclops/report/model_card/sections.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.6/cyclops/report/plot/base.py` & `pycyclops-0.2.7/cyclops/report/plot/base.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.6/cyclops/report/plot/classification.py` & `pycyclops-0.2.7/cyclops/report/plot/classification.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.6/cyclops/report/plot/utils.py` & `pycyclops-0.2.7/cyclops/report/plot/utils.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.6/cyclops/report/report.py` & `pycyclops-0.2.7/cyclops/report/report.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.6/cyclops/report/templates/model_report/button.js` & `pycyclops-0.2.7/cyclops/report/templates/model_report/button.js`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.6/cyclops/report/templates/model_report/macros.jinja` & `pycyclops-0.2.7/cyclops/report/templates/model_report/macros.jinja`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.6/cyclops/report/templates/model_report/model_report.jinja` & `pycyclops-0.2.7/cyclops/report/templates/model_report/model_report.jinja`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.6/cyclops/report/templates/model_report/plot.js` & `pycyclops-0.2.7/cyclops/report/templates/model_report/plot.js`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.6/cyclops/report/utils.py` & `pycyclops-0.2.7/cyclops/report/utils.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.6/cyclops/tasks/base.py` & `pycyclops-0.2.7/cyclops/tasks/base.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.6/cyclops/tasks/classification.py` & `pycyclops-0.2.7/cyclops/tasks/classification.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.6/cyclops/tasks/utils.py` & `pycyclops-0.2.7/cyclops/tasks/utils.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.6/cyclops/utils/common.py` & `pycyclops-0.2.7/cyclops/utils/common.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.6/cyclops/utils/file.py` & `pycyclops-0.2.7/cyclops/utils/file.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.6/cyclops/utils/index.py` & `pycyclops-0.2.7/cyclops/utils/index.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.6/cyclops/utils/log.py` & `pycyclops-0.2.7/cyclops/utils/log.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.6/cyclops/utils/optional.py` & `pycyclops-0.2.7/cyclops/utils/optional.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 """Utilities for handling optional dependencies."""
 
 import importlib
 import importlib.util
 import warnings
-from typing import Any, Literal, Optional
+from types import ModuleType
+from typing import Literal, Optional, Union
 
 
 def import_optional_module(
     name: str,
     attribute: Optional[str] = None,
     error: Literal["raise", "warn", "ignore"] = "raise",
-) -> Optional[Any]:
+) -> Union[ModuleType, None]:
     """Import an optional module.
 
     Parameters
     ----------
     name : str
         The name of the module to import.
     attribute : Optional[str], optional
@@ -23,17 +24,35 @@
         How to handle errors. One of:
         - "raise": raise an error if the module cannot be imported.
         - "warn": raise a warning if the module cannot be imported.
         - "ignore": ignore the missing module and return `None`.
 
     Returns
     -------
-    Optional[Any]
-        The imported module or attribute from the module, or `None` if the
-        module could not be imported.
+    ModuleType or None
+        None if the module could not be imported,
+        or the module or attribute if it was imported successfully.
+
+    Raises
+    ------
+    ImportError
+        If the module could not be imported and `error` is set to "raise".
+
+    Warns
+    -----
+    UserWarning
+        If the module could not be imported and `error` is set to "warn".
+
+    Notes
+    -----
+    This function is useful for handling optional dependencies. It will
+    attempt to import the specified module and return it if it is found.
+    If the module is not found, it will raise an ImportError, raise a
+    warning, or return ``None`` based on the value of
+    the `error` parameter.
 
     """
     if error not in ("raise", "warn", "ignore"):
         raise ValueError(
             "Expected `error` to be one of 'raise', 'warn, or 'ignore', "
             f"but got {error}.",
         )
```

### Comparing `pycyclops-0.2.6/cyclops/utils/plot.py` & `pycyclops-0.2.7/cyclops/utils/plot.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.6/cyclops/utils/profile.py` & `pycyclops-0.2.7/cyclops/utils/profile.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.6/pyproject.toml` & `pycyclops-0.2.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pycyclops"
-version = "0.2.6"
+version = "0.2.7"
 description = "Framework for healthcare ML implementation"
 authors = ["Vector AI Engineering <cyclops@vectorinstitute.ai>"]
 license = "Apache-2.0"
 repository = "https://github.com/VectorInstitute/cyclops"
 documentation = "https://vectorinstitute.github.io/cyclops/"
 packages = [
     { include = "cyclops" },
@@ -95,19 +95,21 @@
 [tool.poetry.group.test.dependencies]
 pytest = "^7.1.1"
 pre-commit = "^2.17.0"
 pytest-cov = "^3.0.0"
 codecov = "^2.1.13"
 nbstripout = "^0.6.1"
 mypy = "^1.7.0"
-ruff = "^0.3.0"
+ruff = "^0.4.0"
 nbqa = { version = "^1.7.0", extras = ["toolchain"] }
 pip-audit = "^2.7.1"
 cycquery = "^0.1.2" # used for integration test
 torchmetrics = {version = "^1.2.0", extras = ["classification", "regression"]}
+pytest-mpi = "^0.6"
+pytest-xdist = {extras = ["psutil"], version = "^3.5.0"}
 
 [tool.poetry.group.docs]
 optional = true
 
 [tool.poetry.group.docs.dependencies]
 numpydoc = "^1.2"
 sphinx = "^7.2.5"
```

### Comparing `pycyclops-0.2.6/PKG-INFO` & `pycyclops-0.2.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycyclops
-Version: 0.2.6
+Version: 0.2.7
 Summary: Framework for healthcare ML implementation
 Home-page: https://github.com/VectorInstitute/cyclops
 License: Apache-2.0
 Author: Vector AI Engineering
 Author-email: cyclops@vectorinstitute.ai
 Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: Apache Software License
@@ -66,15 +66,15 @@
 ``cyclops`` is a toolkit for facilitating research and deployment of ML models for healthcare. It provides a few high-level APIs namely:
 
 * `data` - Create datasets for training, inference and evaluation. We use the popular 🤗 [datasets](https://github.com/huggingface/datasets) to efficiently load and slice different modalities of data
 * `models` - Use common model implementations using [scikit-learn](https://scikit-learn.org/stable/) and [PyTorch](https://pytorch.org/)
 * `tasks` - Use common ML task formulations such as binary classification or multi-label classification on tabular, time-series and image data
 * `evaluate` - Evaluate models on clinical prediction tasks
 * `monitor` - Detect dataset shift relevant for clinical use cases
-* `report` - Create [model report cards](https://vectorinstitute.github.io/cyclops/api/tutorials/nihcxr/nihcxr_report_periodic.html) for clinical ML models
+* `report` - Create [model report cards](https://vectorinstitute.github.io/cyclops/api/tutorials/kaggle/heart_failure_report_periodic.html) for clinical ML models
 
 ``cyclops`` also provides example end-to-end use case implementations on clinical datasets such as
 
 * [NIH chest x-ray](https://www.nih.gov/news-events/news-releases/nih-clinical-center-provides-one-largest-publicly-available-chest-x-ray-datasets-scientific-community)
 * [MIMIC-IV](https://physionet.org/content/mimiciv/2.0/)
```

