# Comparing `tmp/julearn-0.3.2.dev80.tar.gz` & `tmp/julearn-0.3.3.dev4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "julearn-0.3.2.dev80.tar", last modified: Fri May  3 15:18:31 2024, max compression
+gzip compressed data, was "julearn-0.3.3.dev4.tar", last modified: Mon May  6 09:04:03 2024, max compression
```

## Comparing `julearn-0.3.2.dev80.tar` & `julearn-0.3.3.dev4.tar`

### file list

```diff
@@ -1,284 +1,284 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:18:31.159508 julearn-0.3.2.dev80/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:18:31.107507 julearn-0.3.2.dev80/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:18:31.115507 julearn-0.3.2.dev80/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)     1683 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/.github/ISSUE_TEMPLATE/bug_report.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (127)      798 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/.github/ISSUE_TEMPLATE/documentation_request.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1412 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/.github/ISSUE_TEMPLATE/feature_request.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:18:31.119507 julearn-0.3.2.dev80/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/.github/workflows/check-stale.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1941 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/.github/workflows/ci-docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      999 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)      909 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/.github/workflows/docs-preview.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      519 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/.github/workflows/lint.yml
--rw-r--r--   0 runner    (1001) docker     (127)      958 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/.github/workflows/pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      218 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)    34354 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     4958 2024-05-03 15:18:31.159508 julearn-0.3.2.dev80/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      847 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:18:31.119507 julearn-0.3.2.dev80/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:18:31.107507 julearn-0.3.2.dev80/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:18:31.119507 julearn-0.3.2.dev80/docs/_static/css/
--rw-r--r--   0 runner    (1001) docker     (127)      472 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/docs/_static/css/custom.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:18:31.119507 julearn-0.3.2.dev80/docs/_static/js/
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/docs/_static/js/custom.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:18:31.119507 julearn-0.3.2.dev80/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (127)      559 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/docs/_templates/class.rst
--rw-r--r--   0 runner    (1001) docker     (127)      472 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/docs/_templates/function.rst
--rw-r--r--   0 runner    (1001) docker     (127)      720 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/docs/_templates/function_warning.rst
--rw-r--r--   0 runner    (1001) docker     (127)      806 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/docs/_templates/versions.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:18:31.123507 julearn-0.3.2.dev80/docs/api/
--rw-r--r--   0 runner    (1001) docker     (127)      519 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/docs/api/base.rst
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/docs/api/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      404 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/docs/api/inspect.rst
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/docs/api/main.rst
--rw-r--r--   0 runner    (1001) docker     (127)      674 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/docs/api/model_selection.rst
--rw-r--r--   0 runner    (1001) docker     (127)      791 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/docs/api/models.rst
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/docs/api/pipeline.rst
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/docs/api/prepare.rst
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/docs/api/scoring.rst
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/docs/api/stats.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/docs/api/transformers.rst
--rw-r--r--   0 runner    (1001) docker     (127)      719 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/docs/api/utils.rst
--rw-r--r--   0 runner    (1001) docker     (127)      668 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/docs/api/viz.rst
--rw-r--r--   0 runner    (1001) docker     (127)     9119 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/docs/available_pipeline_steps.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:18:31.123507 julearn-0.3.2.dev80/docs/changes/
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/docs/changes/contributors.inc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:18:31.123507 julearn-0.3.2.dev80/docs/changes/newsfragments/
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/docs/changes/newsfragments/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     7865 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2219 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/docs/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6916 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (127)      516 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1874 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/docs/faq.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2795 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/docs/getting_started.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:18:31.127507 julearn-0.3.2.dev80/docs/images/
--rw-r--r--   0 runner    (1001) docker     (127)    69241 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/docs/images/corrected_ttest.png
--rw-r--r--   0 runner    (1001) docker     (127)    39468 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/docs/images/final_estimator.png
--rw-r--r--   0 runner    (1001) docker     (127)    16172 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/docs/images/iris_X.png
--rw-r--r--   0 runner    (1001) docker     (127)    51228 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/docs/images/iris_df.png
--rw-r--r--   0 runner    (1001) docker     (127)     7879 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/docs/images/iris_y.png
--rw-r--r--   0 runner    (1001) docker     (127)    54482 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/docs/images/julearn_logo.png
--rw-r--r--   0 runner    (1001) docker     (127)    74874 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/docs/images/julearn_logo_calm.png
--rw-r--r--   0 runner    (1001) docker     (127)    78884 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/docs/images/julearn_logo_confbias.png
--rw-r--r--   0 runner    (1001) docker     (127)    61311 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/docs/images/julearn_logo_cv.png
--rw-r--r--   0 runner    (1001) docker     (127)    73031 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/docs/images/julearn_logo_generalization.png
--rwxr-xr-x   0 runner    (1001) docker     (127)    60581 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/docs/images/julearn_logo_it.png
--rw-r--r--   0 runner    (1001) docker     (127)    66833 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/docs/images/julearn_logo_ml.png
--rw-r--r--   0 runner    (1001) docker     (127)    60581 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/docs/images/julearn_logo_mlit.png
--rw-r--r--   0 runner    (1001) docker     (127)    94858 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/docs/images/multiple_scorers_run_cv.png
--rw-r--r--   0 runner    (1001) docker     (127)    84126 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/docs/images/plot_scores.png
--rw-r--r--   0 runner    (1001) docker     (127)    43199 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/docs/images/scores_run_cv.png
--rw-r--r--   0 runner    (1001) docker     (127)    83552 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/docs/images/scores_run_cv_splitter.png
--rw-r--r--   0 runner    (1001) docker     (127)    47133 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/docs/images/scores_run_cv_train.png
--rw-r--r--   0 runner    (1001) docker     (127)     3200 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/docs/links.inc
--rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/docs/maintaining.rst
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/docs/redirect.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:18:31.131507 julearn-0.3.2.dev80/docs/selected_deeper_topics/
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/docs/selected_deeper_topics/CBPM.rst
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/docs/selected_deeper_topics/confound_removal.rst
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/docs/selected_deeper_topics/cross_validation_splitter.rst
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/docs/selected_deeper_topics/hyperparameter_tuning.rst
--rw-r--r--   0 runner    (1001) docker     (127)      332 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/docs/selected_deeper_topics/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/docs/selected_deeper_topics/model_inspect.rst
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/docs/selected_deeper_topics/stacked_models.rst
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/docs/selected_deeper_topics/target_transformers.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:18:31.131507 julearn-0.3.2.dev80/docs/sphinxext/
--rw-r--r--   0 runner    (1001) docker     (127)      767 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/docs/sphinxext/gh_substitutions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:18:31.131507 julearn-0.3.2.dev80/docs/what_really_need_know/
--rw-r--r--   0 runner    (1001) docker     (127)     4279 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/docs/what_really_need_know/cross_validation.rst
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/docs/what_really_need_know/data.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/docs/what_really_need_know/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/docs/what_really_need_know/model_comparison.rst
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/docs/what_really_need_know/model_evaluation.rst
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/docs/what_really_need_know/pipeline.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5861 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/docs/whats_new.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:18:31.131507 julearn-0.3.2.dev80/examples/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:18:31.131507 julearn-0.3.2.dev80/examples/00_starting/
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/examples/00_starting/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3990 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/examples/00_starting/plot_cm_acc_multiclass.py
--rw-r--r--   0 runner    (1001) docker     (127)     5099 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/examples/00_starting/plot_example_regression.py
--rw-r--r--   0 runner    (1001) docker     (127)     4984 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/examples/00_starting/plot_stratified_kfold_reg.py
--rw-r--r--   0 runner    (1001) docker     (127)     5791 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/examples/00_starting/run_combine_pandas.py
--rw-r--r--   0 runner    (1001) docker     (127)     4254 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/examples/00_starting/run_grouped_cv.py
--rw-r--r--   0 runner    (1001) docker     (127)     3319 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/examples/00_starting/run_simple_binary_classification.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:18:31.131507 julearn-0.3.2.dev80/examples/01_model_comparison/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/examples/01_model_comparison/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5499 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/examples/01_model_comparison/plot_simple_model_comparison.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:18:31.131507 julearn-0.3.2.dev80/examples/02_inspection/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/examples/02_inspection/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7005 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/examples/02_inspection/plot_groupcv_inspect_svm.py
--rw-r--r--   0 runner    (1001) docker     (127)     3848 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/examples/02_inspection/plot_inspect_random_forest.py
--rw-r--r--   0 runner    (1001) docker     (127)     5556 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/examples/02_inspection/plot_preprocess.py
--rw-r--r--   0 runner    (1001) docker     (127)     2143 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/examples/02_inspection/run_binary_inspect_folds.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:18:31.135507 julearn-0.3.2.dev80/examples/03_complex_models/
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/examples/03_complex_models/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2934 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/examples/03_complex_models/run_apply_to_target.py
--rw-r--r--   0 runner    (1001) docker     (127)     6187 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/examples/03_complex_models/run_example_pca_featsets.py
--rw-r--r--   0 runner    (1001) docker     (127)     3206 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/examples/03_complex_models/run_hyperparameter_multiple_grids.py
--rw-r--r--   0 runner    (1001) docker     (127)     4499 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/examples/03_complex_models/run_hyperparameter_tuning.py
--rw-r--r--   0 runner    (1001) docker     (127)     2673 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/examples/03_complex_models/run_hyperparameter_tuning_bayessearch.py
--rw-r--r--   0 runner    (1001) docker     (127)     2417 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/examples/03_complex_models/run_stacked_models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:18:31.135507 julearn-0.3.2.dev80/examples/04_confounds/
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/examples/04_confounds/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     8747 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/examples/04_confounds/plot_confound_removal_classification.py
--rw-r--r--   0 runner    (1001) docker     (127)     7348 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/examples/04_confounds/run_return_confounds.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:18:31.135507 julearn-0.3.2.dev80/examples/05_customization/
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/examples/05_customization/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4374 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/examples/05_customization/run_custom_scorers_regression.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:18:31.139507 julearn-0.3.2.dev80/examples/99_docs/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/examples/99_docs/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6034 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/examples/99_docs/run_cbpm_docs.py
--rw-r--r--   0 runner    (1001) docker     (127)    11509 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/examples/99_docs/run_confound_removal_docs.py
--rw-r--r--   0 runner    (1001) docker     (127)    12785 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/examples/99_docs/run_cv_splitters_docs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4092 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/examples/99_docs/run_data_docs.py
--rw-r--r--   0 runner    (1001) docker     (127)    23638 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/examples/99_docs/run_hyperparameters_docs.py
--rw-r--r--   0 runner    (1001) docker     (127)     6861 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/examples/99_docs/run_model_comparison_docs.py
--rw-r--r--   0 runner    (1001) docker     (127)    10501 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/examples/99_docs/run_model_evaluation_docs.py
--rw-r--r--   0 runner    (1001) docker     (127)     7890 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/examples/99_docs/run_model_inspection_docs.py
--rw-r--r--   0 runner    (1001) docker     (127)    15278 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/examples/99_docs/run_pipeline_docs.py
--rw-r--r--   0 runner    (1001) docker     (127)     6960 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/examples/99_docs/run_stacked_models_docs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2918 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/examples/99_docs/run_target_transformer_docs.py
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/examples/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:18:31.139507 julearn-0.3.2.dev80/examples/XX_disabled/
--rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/examples/XX_disabled/dis_run_n_jobs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2148 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/examples/XX_disabled/dis_run_target_confound_removal.py
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/ignore_words.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:18:31.139507 julearn-0.3.2.dev80/julearn/
--rw-r--r--   0 runner    (1001) docker     (127)      498 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/julearn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      426 2024-05-03 15:18:30.000000 julearn-0.3.2.dev80/julearn/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    16093 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/julearn/api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:18:31.139507 julearn-0.3.2.dev80/julearn/base/
--rw-r--r--   0 runner    (1001) docker     (127)      431 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/julearn/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7285 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/julearn/base/column_types.py
--rw-r--r--   0 runner    (1001) docker     (127)    14916 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/julearn/base/estimators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:18:31.139507 julearn-0.3.2.dev80/julearn/base/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3048 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/julearn/base/tests/test_base_estimators.py
--rw-r--r--   0 runner    (1001) docker     (127)     6986 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/julearn/base/tests/test_column_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/julearn/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     9277 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/julearn/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:18:31.143507 julearn-0.3.2.dev80/julearn/inspect/
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/julearn/inspect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5747 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/julearn/inspect/_cv.py
--rw-r--r--   0 runner    (1001) docker     (127)     2096 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/julearn/inspect/_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     1897 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/julearn/inspect/_preprocess.py
--rw-r--r--   0 runner    (1001) docker     (127)     2937 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/julearn/inspect/inspector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:18:31.143507 julearn-0.3.2.dev80/julearn/inspect/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     5660 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/julearn/inspect/tests/test_cv.py
--rw-r--r--   0 runner    (1001) docker     (127)     2535 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/julearn/inspect/tests/test_inspector.py
--rw-r--r--   0 runner    (1001) docker     (127)     6587 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/julearn/inspect/tests/test_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     4605 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/julearn/inspect/tests/test_preprocess.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:18:31.143507 julearn-0.3.2.dev80/julearn/model_selection/
--rw-r--r--   0 runner    (1001) docker     (127)      661 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/julearn/model_selection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3818 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/julearn/model_selection/_optuna_searcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     3101 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/julearn/model_selection/_skopt_searcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     4878 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/julearn/model_selection/available_searchers.py
--rw-r--r--   0 runner    (1001) docker     (127)    11399 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/julearn/model_selection/continuous_stratified_kfold.py
--rw-r--r--   0 runner    (1001) docker     (127)     5326 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/julearn/model_selection/stratified_bootstrap.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:18:31.143507 julearn-0.3.2.dev80/julearn/model_selection/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3157 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/julearn/model_selection/tests/test_available_searchers.py
--rw-r--r--   0 runner    (1001) docker     (127)     6210 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/julearn/model_selection/tests/test_continous_stratified_kfold.py
--rw-r--r--   0 runner    (1001) docker     (127)     6337 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/julearn/model_selection/tests/test_optuna_searcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     4809 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/julearn/model_selection/tests/test_skopt_searcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/julearn/model_selection/tests/test_stratified_bootstrap.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:18:31.143507 julearn-0.3.2.dev80/julearn/models/
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/julearn/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7962 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/julearn/models/available_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     6797 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/julearn/models/dynamic.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:18:31.143507 julearn-0.3.2.dev80/julearn/models/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1854 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/julearn/models/tests/test_available_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     6491 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/julearn/models/tests/test_dynamic.py
--rw-r--r--   0 runner    (1001) docker     (127)    10172 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/julearn/models/tests/test_models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:18:31.147508 julearn-0.3.2.dev80/julearn/pipeline/
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/julearn/pipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5055 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/julearn/pipeline/merger.py
--rw-r--r--   0 runner    (1001) docker     (127)    36758 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/julearn/pipeline/pipeline_creator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4848 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/julearn/pipeline/target_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     3149 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/julearn/pipeline/target_pipeline_creator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:18:31.147508 julearn-0.3.2.dev80/julearn/pipeline/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4323 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/julearn/pipeline/tests/test_merger.py
--rw-r--r--   0 runner    (1001) docker     (127)    27718 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/julearn/pipeline/tests/test_pipeline_creator.py
--rw-r--r--   0 runner    (1001) docker     (127)     6016 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/julearn/pipeline/tests/test_target_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/julearn/pipeline/tests/test_target_pipeline_creator.py
--rw-r--r--   0 runner    (1001) docker     (127)    16207 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/julearn/prepare.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:18:31.147508 julearn-0.3.2.dev80/julearn/scoring/
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/julearn/scoring/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6059 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/julearn/scoring/available_scorers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/julearn/scoring/metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:18:31.147508 julearn-0.3.2.dev80/julearn/scoring/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1580 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/julearn/scoring/tests/test_available_scorers.py
--rw-r--r--   0 runner    (1001) docker     (127)      876 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/julearn/scoring/tests/test_metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:18:31.147508 julearn-0.3.2.dev80/julearn/stats/
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/julearn/stats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7896 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/julearn/stats/corrected_ttest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:18:31.147508 julearn-0.3.2.dev80/julearn/stats/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     5537 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/julearn/stats/tests/test_corrected_ttest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:18:31.147508 julearn-0.3.2.dev80/julearn/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    39240 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/julearn/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      647 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/julearn/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    24533 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/julearn/tests/test_prepare.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:18:31.151507 julearn-0.3.2.dev80/julearn/transformers/
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/julearn/transformers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4666 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/julearn/transformers/available_transformers.py
--rw-r--r--   0 runner    (1001) docker     (127)    10676 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/julearn/transformers/cbpm.py
--rw-r--r--   0 runner    (1001) docker     (127)     8837 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/julearn/transformers/confound_remover.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:18:31.151507 julearn-0.3.2.dev80/julearn/transformers/dataframe/
--rw-r--r--   0 runner    (1001) docker     (127)      297 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/julearn/transformers/dataframe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3892 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/julearn/transformers/dataframe/change_column_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     3294 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/julearn/transformers/dataframe/drop_columns.py
--rw-r--r--   0 runner    (1001) docker     (127)     3397 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/julearn/transformers/dataframe/filter_columns.py
--rw-r--r--   0 runner    (1001) docker     (127)     4909 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/julearn/transformers/dataframe/set_column_types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:18:31.151507 julearn-0.3.2.dev80/julearn/transformers/dataframe/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      989 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/julearn/transformers/dataframe/tests/test_change_column_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     1378 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/julearn/transformers/dataframe/tests/test_drop_columns.py
--rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/julearn/transformers/dataframe/tests/test_filter_columns.py
--rw-r--r--   0 runner    (1001) docker     (127)     3044 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/julearn/transformers/dataframe/tests/test_set_column_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     7018 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/julearn/transformers/ju_column_transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:18:31.151507 julearn-0.3.2.dev80/julearn/transformers/target/
--rw-r--r--   0 runner    (1001) docker     (127)      516 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/julearn/transformers/target/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3762 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/julearn/transformers/target/available_target_transformers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2082 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/julearn/transformers/target/ju_target_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6779 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/julearn/transformers/target/ju_transformed_target_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3386 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/julearn/transformers/target/target_confound_remover.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:18:31.151507 julearn-0.3.2.dev80/julearn/transformers/target/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/julearn/transformers/target/tests/test_available_target_transformers.py
--rw-r--r--   0 runner    (1001) docker     (127)      468 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/julearn/transformers/target/tests/test_ju_target_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3138 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/julearn/transformers/target/tests/test_ju_transformed_target_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/julearn/transformers/target/tests/test_target_confound_remover.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:18:31.151507 julearn-0.3.2.dev80/julearn/transformers/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2998 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/julearn/transformers/tests/test_available_transformers.py
--rw-r--r--   0 runner    (1001) docker     (127)     9852 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/julearn/transformers/tests/test_cbpm.py
--rw-r--r--   0 runner    (1001) docker     (127)     8736 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/julearn/transformers/tests/test_confounds.py
--rw-r--r--   0 runner    (1001) docker     (127)     4948 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/julearn/transformers/tests/test_jucolumntransformers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:18:31.155507 julearn-0.3.2.dev80/julearn/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/julearn/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/julearn/utils/_cv.py
--rw-r--r--   0 runner    (1001) docker     (127)     2776 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/julearn/utils/checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     7966 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/julearn/utils/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)    11247 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/julearn/utils/testing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:18:31.155507 julearn-0.3.2.dev80/julearn/utils/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     7434 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/julearn/utils/tests/test_logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     2507 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/julearn/utils/tests/test_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     8127 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/julearn/utils/typing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/julearn/utils/versions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:18:31.155507 julearn-0.3.2.dev80/julearn/viz/
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/julearn/viz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14647 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/julearn/viz/_scores.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:18:31.155507 julearn-0.3.2.dev80/julearn/viz/res/
--rw-r--r--   0 runner    (1001) docker     (127)    73031 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/julearn/viz/res/julearn_logo_generalization.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:18:31.155507 julearn-0.3.2.dev80/julearn.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4958 2024-05-03 15:18:31.000000 julearn-0.3.2.dev80/julearn.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8378 2024-05-03 15:18:31.000000 julearn-0.3.2.dev80/julearn.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 15:18:31.000000 julearn-0.3.2.dev80/julearn.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      565 2024-05-03 15:18:31.000000 julearn-0.3.2.dev80/julearn.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-03 15:18:31.000000 julearn-0.3.2.dev80/julearn.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5612 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 15:18:31.159508 julearn-0.3.2.dev80/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)     2099 2024-05-03 15:18:26.000000 julearn-0.3.2.dev80/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:04:03.097706 julearn-0.3.3.dev4/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:04:03.049705 julearn-0.3.3.dev4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:04:03.057705 julearn-0.3.3.dev4/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)     1683 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/.github/ISSUE_TEMPLATE/bug_report.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/.github/ISSUE_TEMPLATE/documentation_request.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1412 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/.github/ISSUE_TEMPLATE/feature_request.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:04:03.057705 julearn-0.3.3.dev4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/.github/workflows/check-stale.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1941 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/.github/workflows/ci-docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      999 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      909 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/.github/workflows/docs-preview.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/.github/workflows/lint.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      958 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/.github/workflows/pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    34354 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5177 2024-05-06 09:04:03.093706 julearn-0.3.3.dev4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2675 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      847 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:04:03.057705 julearn-0.3.3.dev4/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:04:03.049705 julearn-0.3.3.dev4/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:04:03.057705 julearn-0.3.3.dev4/docs/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (127)      472 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/docs/_static/css/custom.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:04:03.057705 julearn-0.3.3.dev4/docs/_static/js/
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/docs/_static/js/custom.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:04:03.061705 julearn-0.3.3.dev4/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/docs/_templates/class.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      472 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/docs/_templates/function.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/docs/_templates/function_warning.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      806 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/docs/_templates/versions.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:04:03.061705 julearn-0.3.3.dev4/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/docs/api/base.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/docs/api/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      404 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/docs/api/inspect.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/docs/api/main.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      674 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/docs/api/model_selection.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      791 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/docs/api/models.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/docs/api/pipeline.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/docs/api/prepare.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/docs/api/scoring.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/docs/api/stats.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/docs/api/transformers.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      719 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/docs/api/utils.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/docs/api/viz.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     9119 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/docs/available_pipeline_steps.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:04:03.061705 julearn-0.3.3.dev4/docs/changes/
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/docs/changes/contributors.inc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:04:03.061705 julearn-0.3.3.dev4/docs/changes/newsfragments/
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/docs/changes/newsfragments/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     7865 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2219 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/docs/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6916 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      516 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1874 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/docs/faq.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3051 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/docs/getting_started.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:04:03.065705 julearn-0.3.3.dev4/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (127)    69241 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/docs/images/corrected_ttest.png
+-rw-r--r--   0 runner    (1001) docker     (127)    39468 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/docs/images/final_estimator.png
+-rw-r--r--   0 runner    (1001) docker     (127)    16172 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/docs/images/iris_X.png
+-rw-r--r--   0 runner    (1001) docker     (127)    51228 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/docs/images/iris_df.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7879 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/docs/images/iris_y.png
+-rw-r--r--   0 runner    (1001) docker     (127)    54482 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/docs/images/julearn_logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)    74874 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/docs/images/julearn_logo_calm.png
+-rw-r--r--   0 runner    (1001) docker     (127)    78884 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/docs/images/julearn_logo_confbias.png
+-rw-r--r--   0 runner    (1001) docker     (127)    61311 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/docs/images/julearn_logo_cv.png
+-rw-r--r--   0 runner    (1001) docker     (127)    73031 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/docs/images/julearn_logo_generalization.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)    60581 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/docs/images/julearn_logo_it.png
+-rw-r--r--   0 runner    (1001) docker     (127)    66833 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/docs/images/julearn_logo_ml.png
+-rw-r--r--   0 runner    (1001) docker     (127)    60581 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/docs/images/julearn_logo_mlit.png
+-rw-r--r--   0 runner    (1001) docker     (127)    94858 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/docs/images/multiple_scorers_run_cv.png
+-rw-r--r--   0 runner    (1001) docker     (127)    84126 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/docs/images/plot_scores.png
+-rw-r--r--   0 runner    (1001) docker     (127)    43199 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/docs/images/scores_run_cv.png
+-rw-r--r--   0 runner    (1001) docker     (127)    83552 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/docs/images/scores_run_cv_splitter.png
+-rw-r--r--   0 runner    (1001) docker     (127)    47133 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/docs/images/scores_run_cv_train.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3200 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1879 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/docs/links.inc
+-rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/docs/maintaining.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/docs/redirect.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:04:03.069706 julearn-0.3.3.dev4/docs/selected_deeper_topics/
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/docs/selected_deeper_topics/CBPM.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/docs/selected_deeper_topics/confound_removal.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/docs/selected_deeper_topics/cross_validation_splitter.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/docs/selected_deeper_topics/hyperparameter_tuning.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/docs/selected_deeper_topics/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/docs/selected_deeper_topics/model_inspect.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/docs/selected_deeper_topics/stacked_models.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/docs/selected_deeper_topics/target_transformers.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:04:03.069706 julearn-0.3.3.dev4/docs/sphinxext/
+-rw-r--r--   0 runner    (1001) docker     (127)      767 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/docs/sphinxext/gh_substitutions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:04:03.069706 julearn-0.3.3.dev4/docs/what_really_need_know/
+-rw-r--r--   0 runner    (1001) docker     (127)     4279 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/docs/what_really_need_know/cross_validation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/docs/what_really_need_know/data.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/docs/what_really_need_know/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/docs/what_really_need_know/model_comparison.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/docs/what_really_need_know/model_evaluation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/docs/what_really_need_know/pipeline.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5861 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/docs/whats_new.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:04:03.069706 julearn-0.3.3.dev4/examples/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:04:03.069706 julearn-0.3.3.dev4/examples/00_starting/
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/examples/00_starting/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3990 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/examples/00_starting/plot_cm_acc_multiclass.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5099 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/examples/00_starting/plot_example_regression.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4984 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/examples/00_starting/plot_stratified_kfold_reg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5791 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/examples/00_starting/run_combine_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4254 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/examples/00_starting/run_grouped_cv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3319 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/examples/00_starting/run_simple_binary_classification.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:04:03.069706 julearn-0.3.3.dev4/examples/01_model_comparison/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/examples/01_model_comparison/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5499 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/examples/01_model_comparison/plot_simple_model_comparison.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:04:03.069706 julearn-0.3.3.dev4/examples/02_inspection/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/examples/02_inspection/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7005 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/examples/02_inspection/plot_groupcv_inspect_svm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3848 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/examples/02_inspection/plot_inspect_random_forest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5556 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/examples/02_inspection/plot_preprocess.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2143 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/examples/02_inspection/run_binary_inspect_folds.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:04:03.073706 julearn-0.3.3.dev4/examples/03_complex_models/
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/examples/03_complex_models/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2934 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/examples/03_complex_models/run_apply_to_target.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6187 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/examples/03_complex_models/run_example_pca_featsets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3206 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/examples/03_complex_models/run_hyperparameter_multiple_grids.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4499 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/examples/03_complex_models/run_hyperparameter_tuning.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2673 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/examples/03_complex_models/run_hyperparameter_tuning_bayessearch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2417 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/examples/03_complex_models/run_stacked_models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:04:03.073706 julearn-0.3.3.dev4/examples/04_confounds/
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/examples/04_confounds/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     8747 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/examples/04_confounds/plot_confound_removal_classification.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7348 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/examples/04_confounds/run_return_confounds.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:04:03.073706 julearn-0.3.3.dev4/examples/05_customization/
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/examples/05_customization/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4374 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/examples/05_customization/run_custom_scorers_regression.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:04:03.073706 julearn-0.3.3.dev4/examples/99_docs/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/examples/99_docs/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6034 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/examples/99_docs/run_cbpm_docs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11509 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/examples/99_docs/run_confound_removal_docs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12785 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/examples/99_docs/run_cv_splitters_docs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4092 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/examples/99_docs/run_data_docs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23638 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/examples/99_docs/run_hyperparameters_docs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6861 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/examples/99_docs/run_model_comparison_docs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10501 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/examples/99_docs/run_model_evaluation_docs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7890 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/examples/99_docs/run_model_inspection_docs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15278 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/examples/99_docs/run_pipeline_docs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6960 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/examples/99_docs/run_stacked_models_docs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2918 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/examples/99_docs/run_target_transformer_docs.py
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/examples/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:04:03.073706 julearn-0.3.3.dev4/examples/XX_disabled/
+-rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/examples/XX_disabled/dis_run_n_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2148 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/examples/XX_disabled/dis_run_target_confound_removal.py
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/ignore_words.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:04:03.077706 julearn-0.3.3.dev4/julearn/
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/julearn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-05-06 09:04:02.000000 julearn-0.3.3.dev4/julearn/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16093 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/julearn/api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:04:03.077706 julearn-0.3.3.dev4/julearn/base/
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/julearn/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7285 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/julearn/base/column_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14916 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/julearn/base/estimators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:04:03.077706 julearn-0.3.3.dev4/julearn/base/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3048 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/julearn/base/tests/test_base_estimators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6986 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/julearn/base/tests/test_column_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/julearn/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9277 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/julearn/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:04:03.077706 julearn-0.3.3.dev4/julearn/inspect/
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/julearn/inspect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5747 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/julearn/inspect/_cv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2096 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/julearn/inspect/_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1897 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/julearn/inspect/_preprocess.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2937 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/julearn/inspect/inspector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:04:03.077706 julearn-0.3.3.dev4/julearn/inspect/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     5660 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/julearn/inspect/tests/test_cv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2535 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/julearn/inspect/tests/test_inspector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6587 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/julearn/inspect/tests/test_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4605 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/julearn/inspect/tests/test_preprocess.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:04:03.081706 julearn-0.3.3.dev4/julearn/model_selection/
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/julearn/model_selection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3818 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/julearn/model_selection/_optuna_searcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3101 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/julearn/model_selection/_skopt_searcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4878 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/julearn/model_selection/available_searchers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11399 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/julearn/model_selection/continuous_stratified_kfold.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5326 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/julearn/model_selection/stratified_bootstrap.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:04:03.081706 julearn-0.3.3.dev4/julearn/model_selection/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3157 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/julearn/model_selection/tests/test_available_searchers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6210 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/julearn/model_selection/tests/test_continous_stratified_kfold.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6337 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/julearn/model_selection/tests/test_optuna_searcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4809 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/julearn/model_selection/tests/test_skopt_searcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/julearn/model_selection/tests/test_stratified_bootstrap.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:04:03.081706 julearn-0.3.3.dev4/julearn/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/julearn/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7962 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/julearn/models/available_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6797 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/julearn/models/dynamic.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:04:03.081706 julearn-0.3.3.dev4/julearn/models/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1854 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/julearn/models/tests/test_available_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6491 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/julearn/models/tests/test_dynamic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10172 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/julearn/models/tests/test_models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:04:03.081706 julearn-0.3.3.dev4/julearn/pipeline/
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/julearn/pipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5055 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/julearn/pipeline/merger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36758 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/julearn/pipeline/pipeline_creator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4848 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/julearn/pipeline/target_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3149 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/julearn/pipeline/target_pipeline_creator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:04:03.085706 julearn-0.3.3.dev4/julearn/pipeline/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4323 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/julearn/pipeline/tests/test_merger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27718 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/julearn/pipeline/tests/test_pipeline_creator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6016 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/julearn/pipeline/tests/test_target_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/julearn/pipeline/tests/test_target_pipeline_creator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16207 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/julearn/prepare.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:04:03.085706 julearn-0.3.3.dev4/julearn/scoring/
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/julearn/scoring/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6059 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/julearn/scoring/available_scorers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/julearn/scoring/metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:04:03.085706 julearn-0.3.3.dev4/julearn/scoring/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1580 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/julearn/scoring/tests/test_available_scorers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      876 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/julearn/scoring/tests/test_metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:04:03.085706 julearn-0.3.3.dev4/julearn/stats/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/julearn/stats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7896 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/julearn/stats/corrected_ttest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:04:03.085706 julearn-0.3.3.dev4/julearn/stats/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     5537 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/julearn/stats/tests/test_corrected_ttest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:04:03.085706 julearn-0.3.3.dev4/julearn/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    39240 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/julearn/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      647 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/julearn/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24533 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/julearn/tests/test_prepare.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:04:03.085706 julearn-0.3.3.dev4/julearn/transformers/
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/julearn/transformers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4666 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/julearn/transformers/available_transformers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10676 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/julearn/transformers/cbpm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8837 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/julearn/transformers/confound_remover.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:04:03.085706 julearn-0.3.3.dev4/julearn/transformers/dataframe/
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/julearn/transformers/dataframe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3892 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/julearn/transformers/dataframe/change_column_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3294 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/julearn/transformers/dataframe/drop_columns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3397 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/julearn/transformers/dataframe/filter_columns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4909 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/julearn/transformers/dataframe/set_column_types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:04:03.089706 julearn-0.3.3.dev4/julearn/transformers/dataframe/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      989 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/julearn/transformers/dataframe/tests/test_change_column_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1378 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/julearn/transformers/dataframe/tests/test_drop_columns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/julearn/transformers/dataframe/tests/test_filter_columns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3044 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/julearn/transformers/dataframe/tests/test_set_column_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7018 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/julearn/transformers/ju_column_transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:04:03.089706 julearn-0.3.3.dev4/julearn/transformers/target/
+-rw-r--r--   0 runner    (1001) docker     (127)      516 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/julearn/transformers/target/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3762 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/julearn/transformers/target/available_target_transformers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2082 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/julearn/transformers/target/ju_target_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6779 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/julearn/transformers/target/ju_transformed_target_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3386 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/julearn/transformers/target/target_confound_remover.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:04:03.089706 julearn-0.3.3.dev4/julearn/transformers/target/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/julearn/transformers/target/tests/test_available_target_transformers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/julearn/transformers/target/tests/test_ju_target_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3138 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/julearn/transformers/target/tests/test_ju_transformed_target_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/julearn/transformers/target/tests/test_target_confound_remover.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:04:03.089706 julearn-0.3.3.dev4/julearn/transformers/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2998 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/julearn/transformers/tests/test_available_transformers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9852 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/julearn/transformers/tests/test_cbpm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8736 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/julearn/transformers/tests/test_confounds.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4948 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/julearn/transformers/tests/test_jucolumntransformers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:04:03.089706 julearn-0.3.3.dev4/julearn/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/julearn/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/julearn/utils/_cv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2776 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/julearn/utils/checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7966 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/julearn/utils/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11247 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/julearn/utils/testing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:04:03.089706 julearn-0.3.3.dev4/julearn/utils/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     7434 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/julearn/utils/tests/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2507 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/julearn/utils/tests/test_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8127 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/julearn/utils/typing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/julearn/utils/versions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:04:03.093706 julearn-0.3.3.dev4/julearn/viz/
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/julearn/viz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14647 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/julearn/viz/_scores.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:04:03.093706 julearn-0.3.3.dev4/julearn/viz/res/
+-rw-r--r--   0 runner    (1001) docker     (127)    73031 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/julearn/viz/res/julearn_logo_generalization.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:04:03.093706 julearn-0.3.3.dev4/julearn.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5177 2024-05-06 09:04:02.000000 julearn-0.3.3.dev4/julearn.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8378 2024-05-06 09:04:03.000000 julearn-0.3.3.dev4/julearn.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 09:04:02.000000 julearn-0.3.3.dev4/julearn.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-05-06 09:04:02.000000 julearn-0.3.3.dev4/julearn.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-06 09:04:02.000000 julearn-0.3.3.dev4/julearn.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5612 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 09:04:03.097706 julearn-0.3.3.dev4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2099 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/tox.ini
```

### Comparing `julearn-0.3.2.dev80/.github/ISSUE_TEMPLATE/bug_report.yaml` & `julearn-0.3.3.dev4/.github/ISSUE_TEMPLATE/bug_report.yaml`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev80/.github/ISSUE_TEMPLATE/documentation_request.yaml` & `julearn-0.3.3.dev4/.github/ISSUE_TEMPLATE/documentation_request.yaml`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev80/.github/ISSUE_TEMPLATE/feature_request.yaml` & `julearn-0.3.3.dev4/.github/ISSUE_TEMPLATE/feature_request.yaml`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev80/.github/workflows/ci-docs.yml` & `julearn-0.3.3.dev4/.github/workflows/ci-docs.yml`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev80/.github/workflows/ci.yml` & `julearn-0.3.3.dev4/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev80/.github/workflows/docs-preview.yml` & `julearn-0.3.3.dev4/.github/workflows/docs-preview.yml`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev80/.github/workflows/docs.yml` & `julearn-0.3.3.dev4/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev80/.github/workflows/lint.yml` & `julearn-0.3.3.dev4/.github/workflows/lint.yml`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev80/.github/workflows/pypi.yml` & `julearn-0.3.3.dev4/.github/workflows/pypi.yml`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev80/.gitignore` & `julearn-0.3.3.dev4/.gitignore`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev80/.pre-commit-config.yaml` & `julearn-0.3.3.dev4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev80/LICENSE.md` & `julearn-0.3.3.dev4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev80/PKG-INFO` & `julearn-0.3.3.dev4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: julearn
-Version: 0.3.2.dev80
+Version: 0.3.3.dev4
 Summary: Juelich Machine Learning Library
 Author-email: Fede Raimondo <f.raimondo@fz-juelich.de>, Sami Hamdan <s.hamdan@fz-juelich.de>
 Maintainer-email: Sami Hamdan <s.hamdan@fz-juelich.de>
 License: AGPL-3.0-only
 Project-URL: homepage, https://juaml.github.io/julearn
 Project-URL: documentation, https://juaml.github.io/julearn
 Project-URL: repository, https://github.com/juaml/julearn
@@ -58,14 +58,15 @@
 Requires-Dist: julearn[optuna,skopt,viz]; extra == "all"
 
 # julearn
 
 ![PyPI](https://img.shields.io/pypi/v/julearn?style=flat-square)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/julearn?style=flat-square)
 ![PyPI - Wheel](https://img.shields.io/pypi/wheel/julearn?style=flat-square)
+[![Anaconda-Server Badge](https://anaconda.org/conda-forge/julearn/badges/version.svg)](https://anaconda.org/conda-forge/julearn)
 ![GitHub](https://img.shields.io/github/license/juaml/julearn?style=flat-square)
 ![Codecov](https://img.shields.io/codecov/c/github/juaml/julearn?style=flat-square)
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json)](https://github.com/charliermarsh/ruff)
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit)](https://github.com/pre-commit/pre-commit)
 
 ## About
 
@@ -79,14 +80,20 @@
 
 Use `pip` to install from PyPI like so:
 
 ```
 pip install julearn
 ```
 
+You can also install via `conda`, like so:
+
+```
+conda install -c conda-forge julearn
+```
+
 ## Licensing
 
 julearn is released under the AGPL v3 license:
 
 julearn, FZJuelich AML machine learning library.
 Copyright (C) 2020, authors of julearn.
```

### Comparing `julearn-0.3.2.dev80/README.md` & `julearn-0.3.3.dev4/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # julearn
 
 ![PyPI](https://img.shields.io/pypi/v/julearn?style=flat-square)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/julearn?style=flat-square)
 ![PyPI - Wheel](https://img.shields.io/pypi/wheel/julearn?style=flat-square)
+[![Anaconda-Server Badge](https://anaconda.org/conda-forge/julearn/badges/version.svg)](https://anaconda.org/conda-forge/julearn)
 ![GitHub](https://img.shields.io/github/license/juaml/julearn?style=flat-square)
 ![Codecov](https://img.shields.io/codecov/c/github/juaml/julearn?style=flat-square)
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json)](https://github.com/charliermarsh/ruff)
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit)](https://github.com/pre-commit/pre-commit)
 
 ## About
 
@@ -20,14 +21,20 @@
 
 Use `pip` to install from PyPI like so:
 
 ```
 pip install julearn
 ```
 
+You can also install via `conda`, like so:
+
+```
+conda install -c conda-forge julearn
+```
+
 ## Licensing
 
 julearn is released under the AGPL v3 license:
 
 julearn, FZJuelich AML machine learning library.
 Copyright (C) 2020, authors of julearn.
```

### Comparing `julearn-0.3.2.dev80/codecov.yml` & `julearn-0.3.3.dev4/codecov.yml`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev80/docs/Makefile` & `julearn-0.3.3.dev4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev80/docs/_templates/class.rst` & `julearn-0.3.3.dev4/docs/_templates/class.rst`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev80/docs/_templates/function_warning.rst` & `julearn-0.3.3.dev4/docs/_templates/function_warning.rst`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev80/docs/_templates/versions.html` & `julearn-0.3.3.dev4/docs/_templates/versions.html`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev80/docs/api/base.rst` & `julearn-0.3.3.dev4/docs/api/base.rst`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev80/docs/api/model_selection.rst` & `julearn-0.3.3.dev4/docs/api/model_selection.rst`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev80/docs/api/models.rst` & `julearn-0.3.3.dev4/docs/api/models.rst`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev80/docs/api/scoring.rst` & `julearn-0.3.3.dev4/docs/api/scoring.rst`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev80/docs/api/transformers.rst` & `julearn-0.3.3.dev4/docs/api/transformers.rst`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev80/docs/api/utils.rst` & `julearn-0.3.3.dev4/docs/api/utils.rst`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev80/docs/api/viz.rst` & `julearn-0.3.3.dev4/docs/api/viz.rst`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev80/docs/available_pipeline_steps.rst` & `julearn-0.3.3.dev4/docs/available_pipeline_steps.rst`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev80/docs/conf.py` & `julearn-0.3.3.dev4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev80/docs/configuration.rst` & `julearn-0.3.3.dev4/docs/configuration.rst`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev80/docs/contributing.rst` & `julearn-0.3.3.dev4/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev80/docs/examples.rst` & `julearn-0.3.3.dev4/docs/examples.rst`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev80/docs/faq.rst` & `julearn-0.3.3.dev4/docs/faq.rst`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev80/docs/getting_started.rst` & `julearn-0.3.3.dev4/docs/getting_started.rst`

 * *Files 5% similar despite different names*

```diff
@@ -8,25 +8,25 @@
 ------------
 
 ``julearn`` is compatible with `Python`_ >= 3.8 and requires the following
 packages:
 
 * ``numpy>=1.24,<1.27``
 * ``pandas>=1.5.0,<2.2``
-* ``scikit-learn>=1.2,<1.4``
+* ``scikit-learn>=1.2.0,<1.5.0``
 * ``statsmodels>=0.13,<0.15``
 
 Running the examples require:
 
 * ``seaborn>=0.12.2,<0.13``
 * ``bokeh>=3.0.0``
-* ``panel>=1.0.0b1``
-* ``param>=1.11.0``
+* ``panel>=1.3.0``
+* ``param>=2.0.0``
 
-Depending on the installation method (e.g. the `pip install` option below),
+Depending on the installation method (e.g. the ``pip install`` option below),
 these packages might be installed automatically. It is nevertheless good to be
 aware of these dependencies as installing ``julearn`` might lead to changes in
 these packages.
 
 Setup suggestion
 ================
 
@@ -43,25 +43,31 @@
 .. note::
     ``julearn`` keeps on being updated and improved. The latest stable release
     and the developer version therefore often differ quite a bit.
     If you want the newest updates, it might make more sense for you to use the
     developer version until we release the next stable ``julearn`` version.
 
 
-Depending on your aimed usage of ``julearn`` you have two different options
+Depending on your aimed usage of ``julearn`` you have different options
 how to install ``julearn``:
 
 #. Install the *latest release*: Likely most suitable for most
    **end users**. This is done by installing the latest stable release from
-   PyPI.
+   PyPI:
 
    .. code-block:: bash
 
        pip install -U julearn
 
+   or via ``conda`` like so:
+
+   .. code-block:: bash
+
+     conda install -c conda-forge julearn
+
 #. Install the *latest pre-relase*: This version will have the
    **latest updates**. However, it is still under development and not yet
    officially released. Some features might still change before the next stable
    release.
 
    .. code-block:: bash
 
@@ -86,8 +92,9 @@
 
 * ``viz``: Visualization tools for ``julearn``. This includes the
   :mod:`.viz` module.
 * ``deslib``: The :mod:`.dynamic` module requires the `deslib`_ package. This
   module is not compatible with newer Python versions and it is unmaintained.
 * ``skopt``: Using the ``"bayes"`` searcher (:class:`~skopt.BayesSearchCV`)
   requires the `scikit-optimize`_ package.
+* ``optuna``: Using the ``"optuna"`` searcher (:class:`~optuna_integration.sklearn.OptunaSearchCV`) requires the `Optuna`_ and `optuna_integration`_ packages.
 * ``all``: Install all optional functional dependencies (except ``deslib``).
```

### Comparing `julearn-0.3.2.dev80/docs/images/corrected_ttest.png` & `julearn-0.3.3.dev4/docs/images/corrected_ttest.png`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev80/docs/images/final_estimator.png` & `julearn-0.3.3.dev4/docs/images/final_estimator.png`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev80/docs/images/iris_X.png` & `julearn-0.3.3.dev4/docs/images/iris_X.png`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev80/docs/images/iris_df.png` & `julearn-0.3.3.dev4/docs/images/iris_df.png`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev80/docs/images/iris_y.png` & `julearn-0.3.3.dev4/docs/images/iris_y.png`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev80/docs/images/julearn_logo.png` & `julearn-0.3.3.dev4/docs/images/julearn_logo.png`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev80/docs/images/julearn_logo_calm.png` & `julearn-0.3.3.dev4/docs/images/julearn_logo_calm.png`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev80/docs/images/julearn_logo_confbias.png` & `julearn-0.3.3.dev4/docs/images/julearn_logo_confbias.png`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev80/docs/images/julearn_logo_cv.png` & `julearn-0.3.3.dev4/docs/images/julearn_logo_cv.png`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev80/docs/images/julearn_logo_generalization.png` & `julearn-0.3.3.dev4/docs/images/julearn_logo_generalization.png`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev80/docs/images/julearn_logo_it.png` & `julearn-0.3.3.dev4/docs/images/julearn_logo_it.png`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev80/docs/images/julearn_logo_ml.png` & `julearn-0.3.3.dev4/docs/images/julearn_logo_ml.png`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev80/docs/images/julearn_logo_mlit.png` & `julearn-0.3.3.dev4/docs/images/julearn_logo_mlit.png`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev80/docs/images/multiple_scorers_run_cv.png` & `julearn-0.3.3.dev4/docs/images/multiple_scorers_run_cv.png`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev80/docs/images/plot_scores.png` & `julearn-0.3.3.dev4/docs/images/plot_scores.png`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev80/docs/images/scores_run_cv.png` & `julearn-0.3.3.dev4/docs/images/scores_run_cv.png`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev80/docs/images/scores_run_cv_splitter.png` & `julearn-0.3.3.dev4/docs/images/scores_run_cv_splitter.png`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev80/docs/images/scores_run_cv_train.png` & `julearn-0.3.3.dev4/docs/images/scores_run_cv_train.png`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev80/docs/index.rst` & `julearn-0.3.3.dev4/docs/index.rst`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev80/docs/links.inc` & `julearn-0.3.3.dev4/docs/links.inc`

 * *Files 6% similar despite different names*

```diff
@@ -37,8 +37,9 @@
 
 .. _`sphinx gallery`: https://sphinx-gallery.github.io/stable/index.html
 .. _`sphinx RST reference`: https://www.sphinx-doc.org/en/master/usage/restructuredtext/basics.html#inline-markup
 
 
 .. _`DESlib`: https://github.com/scikit-learn-contrib/DESlib
 .. _`scikit-optimize`: https://scikit-optimize.readthedocs.io/en/stable/
-.. _`Optuna`: https://optuna.org
+.. _`Optuna`: https://optuna.org
+.. _`optuna_integration`: https://github.com/optuna/optuna-integration
```

### Comparing `julearn-0.3.2.dev80/docs/maintaining.rst` & `julearn-0.3.3.dev4/docs/maintaining.rst`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev80/docs/sphinxext/gh_substitutions.py` & `julearn-0.3.3.dev4/docs/sphinxext/gh_substitutions.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev80/docs/what_really_need_know/cross_validation.rst` & `julearn-0.3.3.dev4/docs/what_really_need_know/cross_validation.rst`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev80/docs/what_really_need_know/index.rst` & `julearn-0.3.3.dev4/docs/what_really_need_know/index.rst`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev80/docs/whats_new.rst` & `julearn-0.3.3.dev4/docs/whats_new.rst`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev80/examples/00_starting/plot_cm_acc_multiclass.py` & `julearn-0.3.3.dev4/examples/00_starting/plot_cm_acc_multiclass.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev80/examples/00_starting/plot_example_regression.py` & `julearn-0.3.3.dev4/examples/00_starting/plot_example_regression.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev80/examples/00_starting/plot_stratified_kfold_reg.py` & `julearn-0.3.3.dev4/examples/00_starting/plot_stratified_kfold_reg.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev80/examples/00_starting/run_combine_pandas.py` & `julearn-0.3.3.dev4/examples/00_starting/run_combine_pandas.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev80/examples/00_starting/run_grouped_cv.py` & `julearn-0.3.3.dev4/examples/00_starting/run_grouped_cv.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev80/examples/00_starting/run_simple_binary_classification.py` & `julearn-0.3.3.dev4/examples/00_starting/run_simple_binary_classification.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev80/examples/01_model_comparison/plot_simple_model_comparison.py` & `julearn-0.3.3.dev4/examples/01_model_comparison/plot_simple_model_comparison.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev80/examples/02_inspection/plot_groupcv_inspect_svm.py` & `julearn-0.3.3.dev4/examples/02_inspection/plot_groupcv_inspect_svm.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev80/examples/02_inspection/plot_inspect_random_forest.py` & `julearn-0.3.3.dev4/examples/02_inspection/plot_inspect_random_forest.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev80/examples/02_inspection/plot_preprocess.py` & `julearn-0.3.3.dev4/examples/02_inspection/plot_preprocess.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev80/examples/02_inspection/run_binary_inspect_folds.py` & `julearn-0.3.3.dev4/examples/02_inspection/run_binary_inspect_folds.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev80/examples/03_complex_models/run_apply_to_target.py` & `julearn-0.3.3.dev4/examples/03_complex_models/run_apply_to_target.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev80/examples/03_complex_models/run_example_pca_featsets.py` & `julearn-0.3.3.dev4/examples/03_complex_models/run_example_pca_featsets.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev80/examples/03_complex_models/run_hyperparameter_multiple_grids.py` & `julearn-0.3.3.dev4/examples/03_complex_models/run_hyperparameter_multiple_grids.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev80/examples/03_complex_models/run_hyperparameter_tuning.py` & `julearn-0.3.3.dev4/examples/03_complex_models/run_hyperparameter_tuning.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev80/examples/03_complex_models/run_hyperparameter_tuning_bayessearch.py` & `julearn-0.3.3.dev4/examples/03_complex_models/run_hyperparameter_tuning_bayessearch.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev80/examples/03_complex_models/run_stacked_models.py` & `julearn-0.3.3.dev4/examples/03_complex_models/run_stacked_models.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev80/examples/04_confounds/plot_confound_removal_classification.py` & `julearn-0.3.3.dev4/examples/04_confounds/plot_confound_removal_classification.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev80/examples/04_confounds/run_return_confounds.py` & `julearn-0.3.3.dev4/examples/04_confounds/run_return_confounds.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev80/examples/05_customization/run_custom_scorers_regression.py` & `julearn-0.3.3.dev4/examples/05_customization/run_custom_scorers_regression.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev80/examples/99_docs/run_cbpm_docs.py` & `julearn-0.3.3.dev4/examples/99_docs/run_cbpm_docs.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev80/examples/99_docs/run_confound_removal_docs.py` & `julearn-0.3.3.dev4/examples/99_docs/run_confound_removal_docs.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev80/examples/99_docs/run_cv_splitters_docs.py` & `julearn-0.3.3.dev4/examples/99_docs/run_cv_splitters_docs.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev80/examples/99_docs/run_data_docs.py` & `julearn-0.3.3.dev4/examples/99_docs/run_data_docs.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev80/examples/99_docs/run_hyperparameters_docs.py` & `julearn-0.3.3.dev4/examples/99_docs/run_hyperparameters_docs.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev80/examples/99_docs/run_model_comparison_docs.py` & `julearn-0.3.3.dev4/examples/99_docs/run_model_comparison_docs.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev80/examples/99_docs/run_model_evaluation_docs.py` & `julearn-0.3.3.dev4/examples/99_docs/run_model_evaluation_docs.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev80/examples/99_docs/run_model_inspection_docs.py` & `julearn-0.3.3.dev4/examples/99_docs/run_model_inspection_docs.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev80/examples/99_docs/run_pipeline_docs.py` & `julearn-0.3.3.dev4/examples/99_docs/run_pipeline_docs.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev80/examples/99_docs/run_stacked_models_docs.py` & `julearn-0.3.3.dev4/examples/99_docs/run_stacked_models_docs.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev80/examples/99_docs/run_target_transformer_docs.py` & `julearn-0.3.3.dev4/examples/99_docs/run_target_transformer_docs.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev80/examples/XX_disabled/dis_run_n_jobs.py` & `julearn-0.3.3.dev4/examples/XX_disabled/dis_run_n_jobs.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev80/examples/XX_disabled/dis_run_target_confound_removal.py` & `julearn-0.3.3.dev4/examples/XX_disabled/dis_run_target_confound_removal.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev80/julearn/api.py` & `julearn-0.3.3.dev4/julearn/api.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev80/julearn/base/column_types.py` & `julearn-0.3.3.dev4/julearn/base/column_types.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev80/julearn/base/estimators.py` & `julearn-0.3.3.dev4/julearn/base/estimators.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev80/julearn/base/tests/test_base_estimators.py` & `julearn-0.3.3.dev4/julearn/base/tests/test_base_estimators.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev80/julearn/base/tests/test_column_types.py` & `julearn-0.3.3.dev4/julearn/base/tests/test_column_types.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev80/julearn/config.py` & `julearn-0.3.3.dev4/julearn/config.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev80/julearn/conftest.py` & `julearn-0.3.3.dev4/julearn/conftest.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev80/julearn/inspect/_cv.py` & `julearn-0.3.3.dev4/julearn/inspect/_cv.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev80/julearn/inspect/_pipeline.py` & `julearn-0.3.3.dev4/julearn/inspect/_pipeline.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev80/julearn/inspect/_preprocess.py` & `julearn-0.3.3.dev4/julearn/inspect/_preprocess.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev80/julearn/inspect/inspector.py` & `julearn-0.3.3.dev4/julearn/inspect/inspector.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev80/julearn/inspect/tests/test_cv.py` & `julearn-0.3.3.dev4/julearn/inspect/tests/test_cv.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev80/julearn/inspect/tests/test_inspector.py` & `julearn-0.3.3.dev4/julearn/inspect/tests/test_inspector.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev80/julearn/inspect/tests/test_pipeline.py` & `julearn-0.3.3.dev4/julearn/inspect/tests/test_pipeline.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev80/julearn/inspect/tests/test_preprocess.py` & `julearn-0.3.3.dev4/julearn/inspect/tests/test_preprocess.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev80/julearn/model_selection/__init__.py` & `julearn-0.3.3.dev4/julearn/model_selection/__init__.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev80/julearn/model_selection/_optuna_searcher.py` & `julearn-0.3.3.dev4/julearn/model_selection/_optuna_searcher.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev80/julearn/model_selection/_skopt_searcher.py` & `julearn-0.3.3.dev4/julearn/model_selection/_skopt_searcher.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev80/julearn/model_selection/available_searchers.py` & `julearn-0.3.3.dev4/julearn/model_selection/available_searchers.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev80/julearn/model_selection/continuous_stratified_kfold.py` & `julearn-0.3.3.dev4/julearn/model_selection/continuous_stratified_kfold.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev80/julearn/model_selection/stratified_bootstrap.py` & `julearn-0.3.3.dev4/julearn/model_selection/stratified_bootstrap.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev80/julearn/model_selection/tests/test_available_searchers.py` & `julearn-0.3.3.dev4/julearn/model_selection/tests/test_available_searchers.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev80/julearn/model_selection/tests/test_continous_stratified_kfold.py` & `julearn-0.3.3.dev4/julearn/model_selection/tests/test_continous_stratified_kfold.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev80/julearn/model_selection/tests/test_optuna_searcher.py` & `julearn-0.3.3.dev4/julearn/model_selection/tests/test_optuna_searcher.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev80/julearn/model_selection/tests/test_skopt_searcher.py` & `julearn-0.3.3.dev4/julearn/model_selection/tests/test_skopt_searcher.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev80/julearn/model_selection/tests/test_stratified_bootstrap.py` & `julearn-0.3.3.dev4/julearn/model_selection/tests/test_stratified_bootstrap.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev80/julearn/models/available_models.py` & `julearn-0.3.3.dev4/julearn/models/available_models.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev80/julearn/models/dynamic.py` & `julearn-0.3.3.dev4/julearn/models/dynamic.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev80/julearn/models/tests/test_available_models.py` & `julearn-0.3.3.dev4/julearn/models/tests/test_available_models.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev80/julearn/models/tests/test_dynamic.py` & `julearn-0.3.3.dev4/julearn/models/tests/test_dynamic.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev80/julearn/models/tests/test_models.py` & `julearn-0.3.3.dev4/julearn/models/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev80/julearn/pipeline/merger.py` & `julearn-0.3.3.dev4/julearn/pipeline/merger.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev80/julearn/pipeline/pipeline_creator.py` & `julearn-0.3.3.dev4/julearn/pipeline/pipeline_creator.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev80/julearn/pipeline/target_pipeline.py` & `julearn-0.3.3.dev4/julearn/pipeline/target_pipeline.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev80/julearn/pipeline/target_pipeline_creator.py` & `julearn-0.3.3.dev4/julearn/pipeline/target_pipeline_creator.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev80/julearn/pipeline/tests/test_merger.py` & `julearn-0.3.3.dev4/julearn/pipeline/tests/test_merger.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev80/julearn/pipeline/tests/test_pipeline_creator.py` & `julearn-0.3.3.dev4/julearn/pipeline/tests/test_pipeline_creator.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev80/julearn/pipeline/tests/test_target_pipeline.py` & `julearn-0.3.3.dev4/julearn/pipeline/tests/test_target_pipeline.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev80/julearn/pipeline/tests/test_target_pipeline_creator.py` & `julearn-0.3.3.dev4/julearn/pipeline/tests/test_target_pipeline_creator.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev80/julearn/prepare.py` & `julearn-0.3.3.dev4/julearn/prepare.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev80/julearn/scoring/available_scorers.py` & `julearn-0.3.3.dev4/julearn/scoring/available_scorers.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev80/julearn/scoring/metrics.py` & `julearn-0.3.3.dev4/julearn/scoring/metrics.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev80/julearn/scoring/tests/test_available_scorers.py` & `julearn-0.3.3.dev4/julearn/scoring/tests/test_available_scorers.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev80/julearn/scoring/tests/test_metrics.py` & `julearn-0.3.3.dev4/julearn/scoring/tests/test_metrics.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev80/julearn/stats/corrected_ttest.py` & `julearn-0.3.3.dev4/julearn/stats/corrected_ttest.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev80/julearn/stats/tests/test_corrected_ttest.py` & `julearn-0.3.3.dev4/julearn/stats/tests/test_corrected_ttest.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev80/julearn/tests/test_api.py` & `julearn-0.3.3.dev4/julearn/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev80/julearn/tests/test_config.py` & `julearn-0.3.3.dev4/julearn/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev80/julearn/tests/test_prepare.py` & `julearn-0.3.3.dev4/julearn/tests/test_prepare.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev80/julearn/transformers/__init__.py` & `julearn-0.3.3.dev4/julearn/transformers/__init__.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev80/julearn/transformers/available_transformers.py` & `julearn-0.3.3.dev4/julearn/transformers/available_transformers.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev80/julearn/transformers/cbpm.py` & `julearn-0.3.3.dev4/julearn/transformers/cbpm.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev80/julearn/transformers/confound_remover.py` & `julearn-0.3.3.dev4/julearn/transformers/confound_remover.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev80/julearn/transformers/dataframe/change_column_types.py` & `julearn-0.3.3.dev4/julearn/transformers/dataframe/change_column_types.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev80/julearn/transformers/dataframe/drop_columns.py` & `julearn-0.3.3.dev4/julearn/transformers/dataframe/drop_columns.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev80/julearn/transformers/dataframe/filter_columns.py` & `julearn-0.3.3.dev4/julearn/transformers/dataframe/filter_columns.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev80/julearn/transformers/dataframe/set_column_types.py` & `julearn-0.3.3.dev4/julearn/transformers/dataframe/set_column_types.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev80/julearn/transformers/dataframe/tests/test_change_column_types.py` & `julearn-0.3.3.dev4/julearn/transformers/dataframe/tests/test_change_column_types.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev80/julearn/transformers/dataframe/tests/test_drop_columns.py` & `julearn-0.3.3.dev4/julearn/transformers/dataframe/tests/test_drop_columns.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev80/julearn/transformers/dataframe/tests/test_filter_columns.py` & `julearn-0.3.3.dev4/julearn/transformers/dataframe/tests/test_filter_columns.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev80/julearn/transformers/dataframe/tests/test_set_column_types.py` & `julearn-0.3.3.dev4/julearn/transformers/dataframe/tests/test_set_column_types.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev80/julearn/transformers/ju_column_transformer.py` & `julearn-0.3.3.dev4/julearn/transformers/ju_column_transformer.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev80/julearn/transformers/target/__init__.py` & `julearn-0.3.3.dev4/julearn/transformers/target/__init__.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev80/julearn/transformers/target/available_target_transformers.py` & `julearn-0.3.3.dev4/julearn/transformers/target/available_target_transformers.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev80/julearn/transformers/target/ju_target_transformer.py` & `julearn-0.3.3.dev4/julearn/transformers/target/ju_target_transformer.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev80/julearn/transformers/target/ju_transformed_target_model.py` & `julearn-0.3.3.dev4/julearn/transformers/target/ju_transformed_target_model.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev80/julearn/transformers/target/target_confound_remover.py` & `julearn-0.3.3.dev4/julearn/transformers/target/target_confound_remover.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev80/julearn/transformers/target/tests/test_available_target_transformers.py` & `julearn-0.3.3.dev4/julearn/transformers/target/tests/test_available_target_transformers.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev80/julearn/transformers/target/tests/test_ju_transformed_target_model.py` & `julearn-0.3.3.dev4/julearn/transformers/target/tests/test_ju_transformed_target_model.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev80/julearn/transformers/target/tests/test_target_confound_remover.py` & `julearn-0.3.3.dev4/julearn/transformers/target/tests/test_target_confound_remover.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev80/julearn/transformers/tests/test_available_transformers.py` & `julearn-0.3.3.dev4/julearn/transformers/tests/test_available_transformers.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev80/julearn/transformers/tests/test_cbpm.py` & `julearn-0.3.3.dev4/julearn/transformers/tests/test_cbpm.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev80/julearn/transformers/tests/test_confounds.py` & `julearn-0.3.3.dev4/julearn/transformers/tests/test_confounds.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev80/julearn/transformers/tests/test_jucolumntransformers.py` & `julearn-0.3.3.dev4/julearn/transformers/tests/test_jucolumntransformers.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev80/julearn/utils/_cv.py` & `julearn-0.3.3.dev4/julearn/utils/_cv.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev80/julearn/utils/checks.py` & `julearn-0.3.3.dev4/julearn/utils/checks.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev80/julearn/utils/logging.py` & `julearn-0.3.3.dev4/julearn/utils/logging.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev80/julearn/utils/testing.py` & `julearn-0.3.3.dev4/julearn/utils/testing.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev80/julearn/utils/tests/test_logging.py` & `julearn-0.3.3.dev4/julearn/utils/tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev80/julearn/utils/tests/test_version.py` & `julearn-0.3.3.dev4/julearn/utils/tests/test_version.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev80/julearn/utils/typing.py` & `julearn-0.3.3.dev4/julearn/utils/typing.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev80/julearn/utils/versions.py` & `julearn-0.3.3.dev4/julearn/utils/versions.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev80/julearn/viz/_scores.py` & `julearn-0.3.3.dev4/julearn/viz/_scores.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev80/julearn/viz/res/julearn_logo_generalization.png` & `julearn-0.3.3.dev4/julearn/viz/res/julearn_logo_generalization.png`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev80/julearn.egg-info/PKG-INFO` & `julearn-0.3.3.dev4/julearn.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: julearn
-Version: 0.3.2.dev80
+Version: 0.3.3.dev4
 Summary: Juelich Machine Learning Library
 Author-email: Fede Raimondo <f.raimondo@fz-juelich.de>, Sami Hamdan <s.hamdan@fz-juelich.de>
 Maintainer-email: Sami Hamdan <s.hamdan@fz-juelich.de>
 License: AGPL-3.0-only
 Project-URL: homepage, https://juaml.github.io/julearn
 Project-URL: documentation, https://juaml.github.io/julearn
 Project-URL: repository, https://github.com/juaml/julearn
@@ -58,14 +58,15 @@
 Requires-Dist: julearn[optuna,skopt,viz]; extra == "all"
 
 # julearn
 
 ![PyPI](https://img.shields.io/pypi/v/julearn?style=flat-square)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/julearn?style=flat-square)
 ![PyPI - Wheel](https://img.shields.io/pypi/wheel/julearn?style=flat-square)
+[![Anaconda-Server Badge](https://anaconda.org/conda-forge/julearn/badges/version.svg)](https://anaconda.org/conda-forge/julearn)
 ![GitHub](https://img.shields.io/github/license/juaml/julearn?style=flat-square)
 ![Codecov](https://img.shields.io/codecov/c/github/juaml/julearn?style=flat-square)
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json)](https://github.com/charliermarsh/ruff)
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit)](https://github.com/pre-commit/pre-commit)
 
 ## About
 
@@ -79,14 +80,20 @@
 
 Use `pip` to install from PyPI like so:
 
 ```
 pip install julearn
 ```
 
+You can also install via `conda`, like so:
+
+```
+conda install -c conda-forge julearn
+```
+
 ## Licensing
 
 julearn is released under the AGPL v3 license:
 
 julearn, FZJuelich AML machine learning library.
 Copyright (C) 2020, authors of julearn.
```

### Comparing `julearn-0.3.2.dev80/julearn.egg-info/SOURCES.txt` & `julearn-0.3.3.dev4/julearn.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev80/julearn.egg-info/requires.txt` & `julearn-0.3.3.dev4/julearn.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `julearn-0.3.2.dev80/pyproject.toml` & `julearn-0.3.3.dev4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -65,21 +65,19 @@
 ]
 deslib = ["deslib>=0.3.5,<0.4"]
 viz = [
     "panel>=1.3.0",
     "bokeh>=3.0.0",
     "param>=2.0.0",
 ]
-
 skopt = ["scikit-optimize>=0.10.0,<0.11"]
 optuna = [
     "optuna>=3.6.0,<3.7",
     "optuna_integration>=3.6.0,<3.7",
 ]
-
 # Add all optional functional dependencies (skip deslib until its fixed)
 # This does not include dev/docs building dependencies
 all = ["julearn[viz,skopt,optuna]"]
 
 ################
 # Tool configs #
 ################
@@ -222,15 +220,15 @@
 showcontent = true
 
 # Add custom towncrier fragment for API changes
 [tool.towncrier.fragment.change]
 name = "API Changes"
 showcontent = true
 
-## Configure pyright to ignore assigment types until scikit-learn stubs are updated
+## Configure pyright to ignore assignment types until scikit-learn stubs are updated
 [tool.pyright]
 reportAssignmentType = "none"
 exclude = [
     "docs/auto_examples/",
     "*.html",
     ".git/",
     "*.pyc,",
@@ -238,8 +236,8 @@
     "*/api/generated/*.examples",
     "build/",
     "examples/XX_disabled/",
     ".tox",
     ".eggs",
     "examples/",  # Lots of problems due to bad stubs, avoid filling the example with # type:ignore
     "scratch/",  # place to prototype, not to be checked
-]
+]
```

### Comparing `julearn-0.3.2.dev80/tox.ini` & `julearn-0.3.3.dev4/tox.ini`

 * *Files identical despite different names*

