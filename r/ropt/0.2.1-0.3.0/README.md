# Comparing `tmp/ropt-0.2.1.tar.gz` & `tmp/ropt-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ropt-0.2.1.tar", last modified: Mon Apr 29 11:32:19 2024, max compression
+gzip compressed data, was "ropt-0.3.0.tar", last modified: Mon May  6 15:21:08 2024, max compression
```

## Comparing `ropt-0.2.1.tar` & `ropt-0.3.0.tar`

### file list

```diff
@@ -1,183 +1,185 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:32:19.555861 ropt-0.2.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:32:19.523861 ropt-0.2.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:32:19.527861 ropt-0.2.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-04-29 11:32:13.000000 ropt-0.2.1/.github/workflows/build-docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1708 2024-04-29 11:32:13.000000 ropt-0.2.1/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)      999 2024-04-29 11:32:13.000000 ropt-0.2.1/.github/workflows/static-checks.yml
--rw-r--r--   0 runner    (1001) docker     (127)      763 2024-04-29 11:32:13.000000 ropt-0.2.1/.github/workflows/tests.yml
--rwxr-xr-x   0 runner    (1001) docker     (127)       59 2024-04-29 11:32:13.000000 ropt-0.2.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-29 11:32:13.000000 ropt-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3361 2024-04-29 11:32:19.555861 ropt-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-04-29 11:32:13.000000 ropt-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:32:19.531861 ropt-0.2.1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     3524 2024-04-29 11:32:13.000000 ropt-0.2.1/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:32:19.531861 ropt-0.2.1/docs/javascripts/
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-29 11:32:13.000000 ropt-0.2.1/docs/javascripts/mathjax.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:32:19.531861 ropt-0.2.1/docs/reference/
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-29 11:32:13.000000 ropt-0.2.1/docs/reference/enopt_config.md
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-29 11:32:13.000000 ropt-0.2.1/docs/reference/enums.md
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-04-29 11:32:13.000000 ropt-0.2.1/docs/reference/evaluator.md
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-29 11:32:13.000000 ropt-0.2.1/docs/reference/exceptions.md
--rw-r--r--   0 runner    (1001) docker     (127)      267 2024-04-29 11:32:13.000000 ropt-0.2.1/docs/reference/function_transforms.md
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-29 11:32:13.000000 ropt-0.2.1/docs/reference/optimization.md
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-29 11:32:13.000000 ropt-0.2.1/docs/reference/optimization_steps.md
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-29 11:32:13.000000 ropt-0.2.1/docs/reference/optimizer_backends.md
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-29 11:32:13.000000 ropt-0.2.1/docs/reference/plan_config.md
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-29 11:32:13.000000 ropt-0.2.1/docs/reference/plugins.md
--rw-r--r--   0 runner    (1001) docker     (127)      533 2024-04-29 11:32:13.000000 ropt-0.2.1/docs/reference/realization_filters.md
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-29 11:32:13.000000 ropt-0.2.1/docs/reference/reporting.md
--rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-04-29 11:32:13.000000 ropt-0.2.1/docs/reference/results.md
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-29 11:32:13.000000 ropt-0.2.1/docs/reference/sampler_backends.md
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-29 11:32:13.000000 ropt-0.2.1/docs/reference/utilities.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:32:19.531861 ropt-0.2.1/docs/usage/
--rw-r--r--   0 runner    (1001) docker     (127)     3765 2024-04-29 11:32:13.000000 ropt-0.2.1/docs/usage/robust_optimization.md
--rw-r--r--   0 runner    (1001) docker     (127)     3222 2024-04-29 11:32:13.000000 ropt-0.2.1/docs/usage/running.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:32:19.531861 ropt-0.2.1/examples/
--rw-r--r--   0 runner    (1001) docker     (127)     2821 2024-04-29 11:32:13.000000 ropt-0.2.1/examples/de_linear.py
--rw-r--r--   0 runner    (1001) docker     (127)     3023 2024-04-29 11:32:13.000000 ropt-0.2.1/examples/de_nonlinear.py
--rw-r--r--   0 runner    (1001) docker     (127)     3157 2024-04-29 11:32:13.000000 ropt-0.2.1/examples/rosenbrock_deterministic.py
--rw-r--r--   0 runner    (1001) docker     (127)     4323 2024-04-29 11:32:13.000000 ropt-0.2.1/examples/rosenbrock_ensemble.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:32:19.531861 ropt-0.2.1/examples/script_optimizer/
--rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-04-29 11:32:13.000000 ropt-0.2.1/examples/script_optimizer/rosenbrock.py
--rw-r--r--   0 runner    (1001) docker     (127)     2611 2024-04-29 11:32:13.000000 ropt-0.2.1/examples/script_optimizer/run.py
--rw-r--r--   0 runner    (1001) docker     (127)     2246 2024-04-29 11:32:13.000000 ropt-0.2.1/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2486 2024-04-29 11:32:13.000000 ropt-0.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 11:32:19.555861 ropt-0.2.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:32:19.527861 ropt-0.2.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:32:19.535861 ropt-0.2.1/src/ropt/
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-29 11:32:13.000000 ropt-0.2.1/src/ropt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:32:19.535861 ropt-0.2.1/src/ropt/apps/
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-29 11:32:13.000000 ropt-0.2.1/src/ropt/apps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17499 2024-04-29 11:32:13.000000 ropt-0.2.1/src/ropt/apps/_script_optimizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:32:19.535861 ropt-0.2.1/src/ropt/config/
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-29 11:32:13.000000 ropt-0.2.1/src/ropt/config/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:32:19.539861 ropt-0.2.1/src/ropt/config/enopt/
--rw-r--r--   0 runner    (1001) docker     (127)      993 2024-04-29 11:32:13.000000 ropt-0.2.1/src/ropt/config/enopt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      355 2024-04-29 11:32:13.000000 ropt-0.2.1/src/ropt/config/enopt/_enopt_base_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     9167 2024-04-29 11:32:13.000000 ropt-0.2.1/src/ropt/config/enopt/_enopt_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1997 2024-04-29 11:32:13.000000 ropt-0.2.1/src/ropt/config/enopt/_function_transform_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     6187 2024-04-29 11:32:13.000000 ropt-0.2.1/src/ropt/config/enopt/_gradient_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3401 2024-04-29 11:32:13.000000 ropt-0.2.1/src/ropt/config/enopt/_linear_constraints_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     5071 2024-04-29 11:32:13.000000 ropt-0.2.1/src/ropt/config/enopt/_nonlinear_constraints_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4514 2024-04-29 11:32:13.000000 ropt-0.2.1/src/ropt/config/enopt/_objective_functions_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4332 2024-04-29 11:32:13.000000 ropt-0.2.1/src/ropt/config/enopt/_optimizer_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2161 2024-04-29 11:32:13.000000 ropt-0.2.1/src/ropt/config/enopt/_realization_filter_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3833 2024-04-29 11:32:13.000000 ropt-0.2.1/src/ropt/config/enopt/_realizations_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2351 2024-04-29 11:32:13.000000 ropt-0.2.1/src/ropt/config/enopt/_sampler_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3890 2024-04-29 11:32:13.000000 ropt-0.2.1/src/ropt/config/enopt/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8285 2024-04-29 11:32:13.000000 ropt-0.2.1/src/ropt/config/enopt/_variables_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      952 2024-04-29 11:32:13.000000 ropt-0.2.1/src/ropt/config/enopt/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:32:19.539861 ropt-0.2.1/src/ropt/config/plan/
--rw-r--r--   0 runner    (1001) docker     (127)      688 2024-04-29 11:32:13.000000 ropt-0.2.1/src/ropt/config/plan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5115 2024-04-29 11:32:13.000000 ropt-0.2.1/src/ropt/config/plan/_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-29 11:32:13.000000 ropt-0.2.1/src/ropt/config/plan/_plan_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      827 2024-04-29 11:32:13.000000 ropt-0.2.1/src/ropt/config/plan/_step_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     5130 2024-04-29 11:32:13.000000 ropt-0.2.1/src/ropt/config/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5477 2024-04-29 11:32:13.000000 ropt-0.2.1/src/ropt/enums.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:32:19.539861 ropt-0.2.1/src/ropt/evaluator/
--rw-r--r--   0 runner    (1001) docker     (127)     2527 2024-04-29 11:32:13.000000 ropt-0.2.1/src/ropt/evaluator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7214 2024-04-29 11:32:13.000000 ropt-0.2.1/src/ropt/evaluator/_concurrent.py
--rw-r--r--   0 runner    (1001) docker     (127)    25967 2024-04-29 11:32:13.000000 ropt-0.2.1/src/ropt/evaluator/_ensemble_evaluator.py
--rw-r--r--   0 runner    (1001) docker     (127)     5969 2024-04-29 11:32:13.000000 ropt-0.2.1/src/ropt/evaluator/_evaluator.py
--rw-r--r--   0 runner    (1001) docker     (127)     8928 2024-04-29 11:32:13.000000 ropt-0.2.1/src/ropt/evaluator/_evaluator_results.py
--rw-r--r--   0 runner    (1001) docker     (127)     2207 2024-04-29 11:32:13.000000 ropt-0.2.1/src/ropt/evaluator/_function.py
--rw-r--r--   0 runner    (1001) docker     (127)     8461 2024-04-29 11:32:13.000000 ropt-0.2.1/src/ropt/evaluator/_gradient.py
--rw-r--r--   0 runner    (1001) docker     (127)      862 2024-04-29 11:32:13.000000 ropt-0.2.1/src/ropt/evaluator/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5297 2024-04-29 11:32:13.000000 ropt-0.2.1/src/ropt/evaluator/parsl.py
--rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-04-29 11:32:13.000000 ropt-0.2.1/src/ropt/events.py
--rw-r--r--   0 runner    (1001) docker     (127)      735 2024-04-29 11:32:13.000000 ropt-0.2.1/src/ropt/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:32:19.539861 ropt-0.2.1/src/ropt/optimization/
--rw-r--r--   0 runner    (1001) docker     (127)      433 2024-04-29 11:32:13.000000 ropt-0.2.1/src/ropt/optimization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2870 2024-04-29 11:32:13.000000 ropt-0.2.1/src/ropt/optimization/_bases.py
--rw-r--r--   0 runner    (1001) docker     (127)     4909 2024-04-29 11:32:13.000000 ropt-0.2.1/src/ropt/optimization/_ensemble_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)      771 2024-04-29 11:32:13.000000 ropt-0.2.1/src/ropt/optimization/_events.py
--rw-r--r--   0 runner    (1001) docker     (127)    10114 2024-04-29 11:32:13.000000 ropt-0.2.1/src/ropt/optimization/_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6893 2024-04-29 11:32:13.000000 ropt-0.2.1/src/ropt/optimization/_plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:32:19.539861 ropt-0.2.1/src/ropt/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)     1744 2024-04-29 11:32:13.000000 ropt-0.2.1/src/ropt/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5950 2024-04-29 11:32:13.000000 ropt-0.2.1/src/ropt/plugins/_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:32:19.543861 ropt-0.2.1/src/ropt/plugins/function_transform/
--rw-r--r--   0 runner    (1001) docker     (127)      210 2024-04-29 11:32:13.000000 ropt-0.2.1/src/ropt/plugins/function_transform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5528 2024-04-29 11:32:13.000000 ropt-0.2.1/src/ropt/plugins/function_transform/default.py
--rw-r--r--   0 runner    (1001) docker     (127)     2600 2024-04-29 11:32:13.000000 ropt-0.2.1/src/ropt/plugins/function_transform/protocol.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:32:19.543861 ropt-0.2.1/src/ropt/plugins/optimization_steps/
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-29 11:32:13.000000 ropt-0.2.1/src/ropt/plugins/optimization_steps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2911 2024-04-29 11:32:13.000000 ropt-0.2.1/src/ropt/plugins/optimization_steps/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1792 2024-04-29 11:32:13.000000 ropt-0.2.1/src/ropt/plugins/optimization_steps/default.py
--rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-04-29 11:32:13.000000 ropt-0.2.1/src/ropt/plugins/optimization_steps/enopt_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3890 2024-04-29 11:32:13.000000 ropt-0.2.1/src/ropt/plugins/optimization_steps/evaluator.py
--rw-r--r--   0 runner    (1001) docker     (127)      748 2024-04-29 11:32:13.000000 ropt-0.2.1/src/ropt/plugins/optimization_steps/label.py
--rw-r--r--   0 runner    (1001) docker     (127)     4570 2024-04-29 11:32:13.000000 ropt-0.2.1/src/ropt/plugins/optimization_steps/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)      905 2024-04-29 11:32:13.000000 ropt-0.2.1/src/ropt/plugins/optimization_steps/reset_tracker.py
--rw-r--r--   0 runner    (1001) docker     (127)     1630 2024-04-29 11:32:13.000000 ropt-0.2.1/src/ropt/plugins/optimization_steps/restart.py
--rw-r--r--   0 runner    (1001) docker     (127)     2949 2024-04-29 11:32:13.000000 ropt-0.2.1/src/ropt/plugins/optimization_steps/tracker.py
--rw-r--r--   0 runner    (1001) docker     (127)     1843 2024-04-29 11:32:13.000000 ropt-0.2.1/src/ropt/plugins/optimization_steps/update_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:32:19.543861 ropt-0.2.1/src/ropt/plugins/optimizer/
--rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-04-29 11:32:13.000000 ropt-0.2.1/src/ropt/plugins/optimizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4883 2024-04-29 11:32:13.000000 ropt-0.2.1/src/ropt/plugins/optimizer/protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)    20547 2024-04-29 11:32:13.000000 ropt-0.2.1/src/ropt/plugins/optimizer/scipy.py
--rw-r--r--   0 runner    (1001) docker     (127)     7969 2024-04-29 11:32:13.000000 ropt-0.2.1/src/ropt/plugins/optimizer/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:32:19.543861 ropt-0.2.1/src/ropt/plugins/realization_filter/
--rw-r--r--   0 runner    (1001) docker     (127)      521 2024-04-29 11:32:13.000000 ropt-0.2.1/src/ropt/plugins/realization_filter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15031 2024-04-29 11:32:13.000000 ropt-0.2.1/src/ropt/plugins/realization_filter/default.py
--rw-r--r--   0 runner    (1001) docker     (127)     2096 2024-04-29 11:32:13.000000 ropt-0.2.1/src/ropt/plugins/realization_filter/protocol.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:32:19.543861 ropt-0.2.1/src/ropt/plugins/sampler/
--rw-r--r--   0 runner    (1001) docker     (127)      641 2024-04-29 11:32:13.000000 ropt-0.2.1/src/ropt/plugins/sampler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3555 2024-04-29 11:32:13.000000 ropt-0.2.1/src/ropt/plugins/sampler/protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)     6798 2024-04-29 11:32:13.000000 ropt-0.2.1/src/ropt/plugins/sampler/scipy.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 11:32:13.000000 ropt-0.2.1/src/ropt/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:32:19.547861 ropt-0.2.1/src/ropt/report/
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-04-29 11:32:13.000000 ropt-0.2.1/src/ropt/report/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7603 2024-04-29 11:32:13.000000 ropt-0.2.1/src/ropt/report/_data_frame.py
--rw-r--r--   0 runner    (1001) docker     (127)     5295 2024-04-29 11:32:13.000000 ropt-0.2.1/src/ropt/report/_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     4065 2024-04-29 11:32:13.000000 ropt-0.2.1/src/ropt/report/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:32:19.547861 ropt-0.2.1/src/ropt/results/
--rw-r--r--   0 runner    (1001) docker     (127)     3953 2024-04-29 11:32:13.000000 ropt-0.2.1/src/ropt/results/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6147 2024-04-29 11:32:13.000000 ropt-0.2.1/src/ropt/results/_bound_constraints.py
--rw-r--r--   0 runner    (1001) docker     (127)     5792 2024-04-29 11:32:13.000000 ropt-0.2.1/src/ropt/results/_function_evaluations.py
--rw-r--r--   0 runner    (1001) docker     (127)     3571 2024-04-29 11:32:13.000000 ropt-0.2.1/src/ropt/results/_function_results.py
--rw-r--r--   0 runner    (1001) docker     (127)     4229 2024-04-29 11:32:13.000000 ropt-0.2.1/src/ropt/results/_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3377 2024-04-29 11:32:13.000000 ropt-0.2.1/src/ropt/results/_gradient_evaluations.py
--rw-r--r--   0 runner    (1001) docker     (127)     2879 2024-04-29 11:32:13.000000 ropt-0.2.1/src/ropt/results/_gradient_results.py
--rw-r--r--   0 runner    (1001) docker     (127)     1969 2024-04-29 11:32:13.000000 ropt-0.2.1/src/ropt/results/_gradients.py
--rw-r--r--   0 runner    (1001) docker     (127)     2571 2024-04-29 11:32:13.000000 ropt-0.2.1/src/ropt/results/_linear_constraints.py
--rw-r--r--   0 runner    (1001) docker     (127)     2684 2024-04-29 11:32:13.000000 ropt-0.2.1/src/ropt/results/_maximize.py
--rw-r--r--   0 runner    (1001) docker     (127)     4262 2024-04-29 11:32:13.000000 ropt-0.2.1/src/ropt/results/_nonlinear_constraints.py
--rw-r--r--   0 runner    (1001) docker     (127)     3509 2024-04-29 11:32:13.000000 ropt-0.2.1/src/ropt/results/_pandas.py
--rw-r--r--   0 runner    (1001) docker     (127)     2141 2024-04-29 11:32:13.000000 ropt-0.2.1/src/ropt/results/_realizations.py
--rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-04-29 11:32:13.000000 ropt-0.2.1/src/ropt/results/_result_field.py
--rw-r--r--   0 runner    (1001) docker     (127)     9252 2024-04-29 11:32:13.000000 ropt-0.2.1/src/ropt/results/_results.py
--rw-r--r--   0 runner    (1001) docker     (127)     3523 2024-04-29 11:32:13.000000 ropt-0.2.1/src/ropt/results/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4287 2024-04-29 11:32:13.000000 ropt-0.2.1/src/ropt/results/_xarray.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:32:19.547861 ropt-0.2.1/src/ropt/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-29 11:32:13.000000 ropt-0.2.1/src/ropt/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      712 2024-04-29 11:32:13.000000 ropt-0.2.1/src/ropt/utils/_misc.py
--rw-r--r--   0 runner    (1001) docker     (127)     5351 2024-04-29 11:32:13.000000 ropt-0.2.1/src/ropt/utils/scaling.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-29 11:32:19.000000 ropt-0.2.1/src/ropt/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:32:19.551861 ropt-0.2.1/src/ropt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3361 2024-04-29 11:32:19.000000 ropt-0.2.1/src/ropt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5057 2024-04-29 11:32:19.000000 ropt-0.2.1/src/ropt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 11:32:19.000000 ropt-0.2.1/src/ropt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-29 11:32:19.000000 ropt-0.2.1/src/ropt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-29 11:32:19.000000 ropt-0.2.1/src/ropt.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:32:19.551861 ropt-0.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 11:32:13.000000 ropt-0.2.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4505 2024-04-29 11:32:13.000000 ropt-0.2.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     3811 2024-04-29 11:32:13.000000 ropt-0.2.1/tests/test_concurrent.py
--rw-r--r--   0 runner    (1001) docker     (127)    25786 2024-04-29 11:32:13.000000 ropt-0.2.1/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     9209 2024-04-29 11:32:13.000000 ropt-0.2.1/tests/test_ensemble_gradient.py
--rw-r--r--   0 runner    (1001) docker     (127)     1775 2024-04-29 11:32:13.000000 ropt-0.2.1/tests/test_examples.py
--rw-r--r--   0 runner    (1001) docker     (127)     2185 2024-04-29 11:32:13.000000 ropt-0.2.1/tests/test_failed_realizations.py
--rw-r--r--   0 runner    (1001) docker     (127)     4205 2024-04-29 11:32:13.000000 ropt-0.2.1/tests/test_function_transforms.py
--rw-r--r--   0 runner    (1001) docker     (127)     5503 2024-04-29 11:32:13.000000 ropt-0.2.1/tests/test_netcdf.py
--rw-r--r--   0 runner    (1001) docker     (127)    43207 2024-04-29 11:32:13.000000 ropt-0.2.1/tests/test_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     7387 2024-04-29 11:32:13.000000 ropt-0.2.1/tests/test_pandas.py
--rw-r--r--   0 runner    (1001) docker     (127)     4626 2024-04-29 11:32:13.000000 ropt-0.2.1/tests/test_parsl.py
--rw-r--r--   0 runner    (1001) docker     (127)    27696 2024-04-29 11:32:13.000000 ropt-0.2.1/tests/test_realization_filters.py
--rw-r--r--   0 runner    (1001) docker     (127)     6652 2024-04-29 11:32:13.000000 ropt-0.2.1/tests/test_result_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     8616 2024-04-29 11:32:13.000000 ropt-0.2.1/tests/test_results.py
--rw-r--r--   0 runner    (1001) docker     (127)     5248 2024-04-29 11:32:13.000000 ropt-0.2.1/tests/test_results_data_frame.py
--rw-r--r--   0 runner    (1001) docker     (127)     6602 2024-04-29 11:32:13.000000 ropt-0.2.1/tests/test_samplers.py
--rw-r--r--   0 runner    (1001) docker     (127)    20785 2024-04-29 11:32:13.000000 ropt-0.2.1/tests/test_scipy_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)     4474 2024-04-29 11:32:13.000000 ropt-0.2.1/tests/test_scipy_samplers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3197 2024-04-29 11:32:13.000000 ropt-0.2.1/tests/test_xarray.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:21:08.564519 ropt-0.3.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:21:08.528518 ropt-0.3.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:21:08.536518 ropt-0.3.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-05-06 15:21:02.000000 ropt-0.3.0/.github/workflows/build-docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1708 2024-05-06 15:21:02.000000 ropt-0.3.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      999 2024-05-06 15:21:02.000000 ropt-0.3.0/.github/workflows/static-checks.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      763 2024-05-06 15:21:02.000000 ropt-0.3.0/.github/workflows/tests.yml
+-rwxr-xr-x   0 runner    (1001) docker     (127)       59 2024-05-06 15:21:02.000000 ropt-0.3.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-06 15:21:02.000000 ropt-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3360 2024-05-06 15:21:08.564519 ropt-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1802 2024-05-06 15:21:02.000000 ropt-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:21:08.536518 ropt-0.3.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     3499 2024-05-06 15:21:02.000000 ropt-0.3.0/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:21:08.536518 ropt-0.3.0/docs/javascripts/
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-05-06 15:21:02.000000 ropt-0.3.0/docs/javascripts/mathjax.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:21:08.540518 ropt-0.3.0/docs/reference/
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-05-06 15:21:02.000000 ropt-0.3.0/docs/reference/enopt_config.md
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-06 15:21:02.000000 ropt-0.3.0/docs/reference/enums.md
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-05-06 15:21:02.000000 ropt-0.3.0/docs/reference/evaluator.md
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-06 15:21:02.000000 ropt-0.3.0/docs/reference/exceptions.md
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-05-06 15:21:02.000000 ropt-0.3.0/docs/reference/function_transforms.md
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-06 15:21:02.000000 ropt-0.3.0/docs/reference/optimization.md
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-06 15:21:02.000000 ropt-0.3.0/docs/reference/optimization_steps.md
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-06 15:21:02.000000 ropt-0.3.0/docs/reference/optimizer_plugins.md
+-rw-r--r--   0 runner    (1001) docker     (127)      305 2024-05-06 15:21:02.000000 ropt-0.3.0/docs/reference/plan_config.md
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-06 15:21:02.000000 ropt-0.3.0/docs/reference/plugins.md
+-rw-r--r--   0 runner    (1001) docker     (127)      533 2024-05-06 15:21:02.000000 ropt-0.3.0/docs/reference/realization_filters.md
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-06 15:21:02.000000 ropt-0.3.0/docs/reference/reporting.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-05-06 15:21:02.000000 ropt-0.3.0/docs/reference/results.md
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-06 15:21:02.000000 ropt-0.3.0/docs/reference/sampler_plugins.md
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-06 15:21:02.000000 ropt-0.3.0/docs/reference/utilities.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:21:08.540518 ropt-0.3.0/docs/usage/
+-rw-r--r--   0 runner    (1001) docker     (127)     3756 2024-05-06 15:21:02.000000 ropt-0.3.0/docs/usage/robust_optimization.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3222 2024-05-06 15:21:02.000000 ropt-0.3.0/docs/usage/running.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:21:08.540518 ropt-0.3.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     2815 2024-05-06 15:21:02.000000 ropt-0.3.0/examples/de_linear.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3017 2024-05-06 15:21:02.000000 ropt-0.3.0/examples/de_nonlinear.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3157 2024-05-06 15:21:02.000000 ropt-0.3.0/examples/rosenbrock_deterministic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4323 2024-05-06 15:21:02.000000 ropt-0.3.0/examples/rosenbrock_ensemble.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:21:08.540518 ropt-0.3.0/examples/script_optimizer/
+-rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-05-06 15:21:02.000000 ropt-0.3.0/examples/script_optimizer/rosenbrock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2611 2024-05-06 15:21:02.000000 ropt-0.3.0/examples/script_optimizer/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2242 2024-05-06 15:21:02.000000 ropt-0.3.0/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3120 2024-05-06 15:21:02.000000 ropt-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 15:21:08.564519 ropt-0.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:21:08.532518 ropt-0.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:21:08.540518 ropt-0.3.0/src/ropt/
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-06 15:21:02.000000 ropt-0.3.0/src/ropt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:21:08.544518 ropt-0.3.0/src/ropt/apps/
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-06 15:21:02.000000 ropt-0.3.0/src/ropt/apps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17499 2024-05-06 15:21:02.000000 ropt-0.3.0/src/ropt/apps/_script_optimizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:21:08.544518 ropt-0.3.0/src/ropt/config/
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-06 15:21:02.000000 ropt-0.3.0/src/ropt/config/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:21:08.544518 ropt-0.3.0/src/ropt/config/enopt/
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-05-06 15:21:02.000000 ropt-0.3.0/src/ropt/config/enopt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-05-06 15:21:02.000000 ropt-0.3.0/src/ropt/config/enopt/_enopt_base_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9167 2024-05-06 15:21:02.000000 ropt-0.3.0/src/ropt/config/enopt/_enopt_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-05-06 15:21:02.000000 ropt-0.3.0/src/ropt/config/enopt/_function_transform_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6187 2024-05-06 15:21:02.000000 ropt-0.3.0/src/ropt/config/enopt/_gradient_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3401 2024-05-06 15:21:02.000000 ropt-0.3.0/src/ropt/config/enopt/_linear_constraints_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5071 2024-05-06 15:21:02.000000 ropt-0.3.0/src/ropt/config/enopt/_nonlinear_constraints_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4514 2024-05-06 15:21:02.000000 ropt-0.3.0/src/ropt/config/enopt/_objective_functions_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3986 2024-05-06 15:21:02.000000 ropt-0.3.0/src/ropt/config/enopt/_optimizer_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1568 2024-05-06 15:21:02.000000 ropt-0.3.0/src/ropt/config/enopt/_realization_filter_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3833 2024-05-06 15:21:02.000000 ropt-0.3.0/src/ropt/config/enopt/_realizations_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-05-06 15:21:02.000000 ropt-0.3.0/src/ropt/config/enopt/_sampler_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3890 2024-05-06 15:21:02.000000 ropt-0.3.0/src/ropt/config/enopt/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8241 2024-05-06 15:21:02.000000 ropt-0.3.0/src/ropt/config/enopt/_variables_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2024-05-06 15:21:02.000000 ropt-0.3.0/src/ropt/config/enopt/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:21:08.548518 ropt-0.3.0/src/ropt/config/plan/
+-rw-r--r--   0 runner    (1001) docker     (127)      633 2024-05-06 15:21:02.000000 ropt-0.3.0/src/ropt/config/plan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5115 2024-05-06 15:21:02.000000 ropt-0.3.0/src/ropt/config/plan/_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-05-06 15:21:02.000000 ropt-0.3.0/src/ropt/config/plan/_plan_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5130 2024-05-06 15:21:02.000000 ropt-0.3.0/src/ropt/config/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5477 2024-05-06 15:21:02.000000 ropt-0.3.0/src/ropt/enums.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:21:08.548518 ropt-0.3.0/src/ropt/evaluator/
+-rw-r--r--   0 runner    (1001) docker     (127)     2527 2024-05-06 15:21:02.000000 ropt-0.3.0/src/ropt/evaluator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11783 2024-05-06 15:21:02.000000 ropt-0.3.0/src/ropt/evaluator/_concurrent.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25390 2024-05-06 15:21:02.000000 ropt-0.3.0/src/ropt/evaluator/_ensemble_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5969 2024-05-06 15:21:02.000000 ropt-0.3.0/src/ropt/evaluator/_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8928 2024-05-06 15:21:02.000000 ropt-0.3.0/src/ropt/evaluator/_evaluator_results.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2231 2024-05-06 15:21:02.000000 ropt-0.3.0/src/ropt/evaluator/_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8509 2024-05-06 15:21:02.000000 ropt-0.3.0/src/ropt/evaluator/_gradient.py
+-rw-r--r--   0 runner    (1001) docker     (127)      862 2024-05-06 15:21:02.000000 ropt-0.3.0/src/ropt/evaluator/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5458 2024-05-06 15:21:02.000000 ropt-0.3.0/src/ropt/evaluator/parsl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-05-06 15:21:02.000000 ropt-0.3.0/src/ropt/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-05-06 15:21:02.000000 ropt-0.3.0/src/ropt/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:21:08.548518 ropt-0.3.0/src/ropt/optimization/
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-05-06 15:21:02.000000 ropt-0.3.0/src/ropt/optimization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2870 2024-05-06 15:21:02.000000 ropt-0.3.0/src/ropt/optimization/_bases.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4909 2024-05-06 15:21:02.000000 ropt-0.3.0/src/ropt/optimization/_ensemble_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      771 2024-05-06 15:21:02.000000 ropt-0.3.0/src/ropt/optimization/_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10052 2024-05-06 15:21:02.000000 ropt-0.3.0/src/ropt/optimization/_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6803 2024-05-06 15:21:02.000000 ropt-0.3.0/src/ropt/optimization/_plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:21:08.548518 ropt-0.3.0/src/ropt/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)     1733 2024-05-06 15:21:02.000000 ropt-0.3.0/src/ropt/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5860 2024-05-06 15:21:02.000000 ropt-0.3.0/src/ropt/plugins/_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:21:08.552518 ropt-0.3.0/src/ropt/plugins/function_transform/
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-05-06 15:21:02.000000 ropt-0.3.0/src/ropt/plugins/function_transform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6385 2024-05-06 15:21:02.000000 ropt-0.3.0/src/ropt/plugins/function_transform/default.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3104 2024-05-06 15:21:02.000000 ropt-0.3.0/src/ropt/plugins/function_transform/protocol.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:21:08.552518 ropt-0.3.0/src/ropt/plugins/optimization_steps/
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-06 15:21:02.000000 ropt-0.3.0/src/ropt/plugins/optimization_steps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2911 2024-05-06 15:21:02.000000 ropt-0.3.0/src/ropt/plugins/optimization_steps/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2780 2024-05-06 15:21:02.000000 ropt-0.3.0/src/ropt/plugins/optimization_steps/default.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-05-06 15:21:02.000000 ropt-0.3.0/src/ropt/plugins/optimization_steps/enopt_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3890 2024-05-06 15:21:02.000000 ropt-0.3.0/src/ropt/plugins/optimization_steps/evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      748 2024-05-06 15:21:02.000000 ropt-0.3.0/src/ropt/plugins/optimization_steps/label.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4570 2024-05-06 15:21:02.000000 ropt-0.3.0/src/ropt/plugins/optimization_steps/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-05-06 15:21:02.000000 ropt-0.3.0/src/ropt/plugins/optimization_steps/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)      905 2024-05-06 15:21:02.000000 ropt-0.3.0/src/ropt/plugins/optimization_steps/reset_tracker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1630 2024-05-06 15:21:02.000000 ropt-0.3.0/src/ropt/plugins/optimization_steps/restart.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2949 2024-05-06 15:21:02.000000 ropt-0.3.0/src/ropt/plugins/optimization_steps/tracker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1843 2024-05-06 15:21:02.000000 ropt-0.3.0/src/ropt/plugins/optimization_steps/update_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:21:08.552518 ropt-0.3.0/src/ropt/plugins/optimizer/
+-rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-05-06 15:21:02.000000 ropt-0.3.0/src/ropt/plugins/optimizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5345 2024-05-06 15:21:02.000000 ropt-0.3.0/src/ropt/plugins/optimizer/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20917 2024-05-06 15:21:02.000000 ropt-0.3.0/src/ropt/plugins/optimizer/scipy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7663 2024-05-06 15:21:02.000000 ropt-0.3.0/src/ropt/plugins/optimizer/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-06 15:21:02.000000 ropt-0.3.0/src/ropt/plugins/protocol.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:21:08.552518 ropt-0.3.0/src/ropt/plugins/realization_filter/
+-rw-r--r--   0 runner    (1001) docker     (127)      521 2024-05-06 15:21:02.000000 ropt-0.3.0/src/ropt/plugins/realization_filter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15928 2024-05-06 15:21:02.000000 ropt-0.3.0/src/ropt/plugins/realization_filter/default.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2587 2024-05-06 15:21:02.000000 ropt-0.3.0/src/ropt/plugins/realization_filter/protocol.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:21:08.552518 ropt-0.3.0/src/ropt/plugins/sampler/
+-rw-r--r--   0 runner    (1001) docker     (127)      641 2024-05-06 15:21:02.000000 ropt-0.3.0/src/ropt/plugins/sampler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4259 2024-05-06 15:21:02.000000 ropt-0.3.0/src/ropt/plugins/sampler/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7558 2024-05-06 15:21:02.000000 ropt-0.3.0/src/ropt/plugins/sampler/scipy.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 15:21:02.000000 ropt-0.3.0/src/ropt/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:21:08.556519 ropt-0.3.0/src/ropt/report/
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-06 15:21:02.000000 ropt-0.3.0/src/ropt/report/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7603 2024-05-06 15:21:02.000000 ropt-0.3.0/src/ropt/report/_data_frame.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5295 2024-05-06 15:21:02.000000 ropt-0.3.0/src/ropt/report/_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4065 2024-05-06 15:21:02.000000 ropt-0.3.0/src/ropt/report/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:21:08.556519 ropt-0.3.0/src/ropt/results/
+-rw-r--r--   0 runner    (1001) docker     (127)     3953 2024-05-06 15:21:02.000000 ropt-0.3.0/src/ropt/results/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6147 2024-05-06 15:21:02.000000 ropt-0.3.0/src/ropt/results/_bound_constraints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5792 2024-05-06 15:21:02.000000 ropt-0.3.0/src/ropt/results/_function_evaluations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3571 2024-05-06 15:21:02.000000 ropt-0.3.0/src/ropt/results/_function_results.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4229 2024-05-06 15:21:02.000000 ropt-0.3.0/src/ropt/results/_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3377 2024-05-06 15:21:02.000000 ropt-0.3.0/src/ropt/results/_gradient_evaluations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2879 2024-05-06 15:21:02.000000 ropt-0.3.0/src/ropt/results/_gradient_results.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1969 2024-05-06 15:21:02.000000 ropt-0.3.0/src/ropt/results/_gradients.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2571 2024-05-06 15:21:02.000000 ropt-0.3.0/src/ropt/results/_linear_constraints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2684 2024-05-06 15:21:02.000000 ropt-0.3.0/src/ropt/results/_maximize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4262 2024-05-06 15:21:02.000000 ropt-0.3.0/src/ropt/results/_nonlinear_constraints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3509 2024-05-06 15:21:02.000000 ropt-0.3.0/src/ropt/results/_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2141 2024-05-06 15:21:02.000000 ropt-0.3.0/src/ropt/results/_realizations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-05-06 15:21:02.000000 ropt-0.3.0/src/ropt/results/_result_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9252 2024-05-06 15:21:02.000000 ropt-0.3.0/src/ropt/results/_results.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3523 2024-05-06 15:21:02.000000 ropt-0.3.0/src/ropt/results/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4287 2024-05-06 15:21:02.000000 ropt-0.3.0/src/ropt/results/_xarray.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:21:08.560519 ropt-0.3.0/src/ropt/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-06 15:21:02.000000 ropt-0.3.0/src/ropt/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      712 2024-05-06 15:21:02.000000 ropt-0.3.0/src/ropt/utils/_misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5351 2024-05-06 15:21:02.000000 ropt-0.3.0/src/ropt/utils/scaling.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-06 15:21:08.000000 ropt-0.3.0/src/ropt/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:21:08.564519 ropt-0.3.0/src/ropt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3360 2024-05-06 15:21:08.000000 ropt-0.3.0/src/ropt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5133 2024-05-06 15:21:08.000000 ropt-0.3.0/src/ropt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 15:21:08.000000 ropt-0.3.0/src/ropt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-05-06 15:21:08.000000 ropt-0.3.0/src/ropt.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-06 15:21:08.000000 ropt-0.3.0/src/ropt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-06 15:21:08.000000 ropt-0.3.0/src/ropt.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:21:08.564519 ropt-0.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 15:21:02.000000 ropt-0.3.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4505 2024-05-06 15:21:02.000000 ropt-0.3.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5016 2024-05-06 15:21:02.000000 ropt-0.3.0/tests/test_concurrent.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25752 2024-05-06 15:21:02.000000 ropt-0.3.0/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9187 2024-05-06 15:21:02.000000 ropt-0.3.0/tests/test_ensemble_gradient.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1775 2024-05-06 15:21:02.000000 ropt-0.3.0/tests/test_examples.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2185 2024-05-06 15:21:02.000000 ropt-0.3.0/tests/test_failed_realizations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4205 2024-05-06 15:21:02.000000 ropt-0.3.0/tests/test_function_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5503 2024-05-06 15:21:02.000000 ropt-0.3.0/tests/test_netcdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44245 2024-05-06 15:21:02.000000 ropt-0.3.0/tests/test_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7387 2024-05-06 15:21:02.000000 ropt-0.3.0/tests/test_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4592 2024-05-06 15:21:02.000000 ropt-0.3.0/tests/test_parsl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27696 2024-05-06 15:21:02.000000 ropt-0.3.0/tests/test_realization_filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6618 2024-05-06 15:21:02.000000 ropt-0.3.0/tests/test_result_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8616 2024-05-06 15:21:02.000000 ropt-0.3.0/tests/test_results.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5214 2024-05-06 15:21:02.000000 ropt-0.3.0/tests/test_results_data_frame.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6969 2024-05-06 15:21:02.000000 ropt-0.3.0/tests/test_samplers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20607 2024-05-06 15:21:02.000000 ropt-0.3.0/tests/test_scipy_optimizers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4456 2024-05-06 15:21:02.000000 ropt-0.3.0/tests/test_scipy_samplers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3197 2024-05-06 15:21:02.000000 ropt-0.3.0/tests/test_xarray.py
```

### Comparing `ropt-0.2.1/.github/workflows/build-docs.yml` & `ropt-0.3.0/.github/workflows/build-docs.yml`

 * *Files identical despite different names*

### Comparing `ropt-0.2.1/.github/workflows/release.yml` & `ropt-0.3.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `ropt-0.2.1/.github/workflows/static-checks.yml` & `ropt-0.3.0/.github/workflows/static-checks.yml`

 * *Files identical despite different names*

### Comparing `ropt-0.2.1/.github/workflows/tests.yml` & `ropt-0.3.0/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `ropt-0.2.1/LICENSE` & `ropt-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ropt-0.2.1/PKG-INFO` & `ropt-0.3.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ropt
-Version: 0.2.1
+Version: 0.3.0
 Summary: The ropt ensemble optimizer module
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -50,16 +50,17 @@
 Detailed documentation and examples can be found in the online
 [manual](https://tno-ropt.github.io/ropt/).
 
 
 ## Dependencies
 `ropt` has been tested with Python versions 3.8-3.12.
 
-`ropt` requires one or more optimization backends to function. A backend based
-on optimizers included with [SciPy](https://scipy.org/) is installed by default.
+`ropt` requires one or more optimization plugins to function. By default, a
+plugin based on optimizers included with [SciPy](https://scipy.org/) is
+installed.
 
 
 ## Installation
 From PyPI:
 ```bash
 pip install ropt
 ```
```

### Comparing `ropt-0.2.1/README.md` & `ropt-0.3.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -8,16 +8,17 @@
 Detailed documentation and examples can be found in the online
 [manual](https://tno-ropt.github.io/ropt/).
 
 
 ## Dependencies
 `ropt` has been tested with Python versions 3.8-3.12.
 
-`ropt` requires one or more optimization backends to function. A backend based
-on optimizers included with [SciPy](https://scipy.org/) is installed by default.
+`ropt` requires one or more optimization plugins to function. By default, a
+plugin based on optimizers included with [SciPy](https://scipy.org/) is
+installed.
 
 
 ## Installation
 From PyPI:
 ```bash
 pip install ropt
 ```
```

### Comparing `ropt-0.2.1/docs/index.md` & `ropt-0.3.0/docs/index.md`

 * *Files 4% similar despite different names*

```diff
@@ -23,29 +23,30 @@
 
 - Robust optimization over an ensemble of models, i.e., optimizing the average
   of a set of objective functions. Alternative objectives can be implemented
   using plugins, for instance, to implement risk-aware optimization, such as
   Conditional Value at Risk (CVaR) or standard-deviation-based functions.
 - Support for black-box optimization of arbitrary functions.
 - Support for running complex optimization workflows, such as multiple runs with
-  different optimization settings or even different optimization algorithms.
+  different optimization settings or even different optimization methods.
 - Support for nested optimization, allowing sub-sets of the variables to be
   optimized by optimization workflows that run as part of the black-box function
   to be optimized.
-- An interface for running various continuous and discrete optimization
-  algorithms. By default, an optimization backend based on
-  [`scipy.optimize`](https://docs.scipy.org/doc/scipy/tutorial/optimize.html) is
-  included, but additional backends can be added via a plugin mechanism. The
-  most common options of these optimizers can be configured in a uniform manner,
-  although algorithm- or package-specific options can still be passed.
+- An interface for running various continuous and discrete optimization methods.
+  By default, optimizers from the
+  [`scipy.optimize`](https://docs.scipy.org/doc/scipy/tutorial/optimize.html)
+  package are included, but additional optimizers can be added via a plugin
+  mechanism. The most common options of these optimizers can be configured in a
+  uniform manner, although algorithm- or package-specific options can still be
+  passed.
 - Efficient estimation of gradients using a Stochastic Simplex Approximate
-  Gradient (StoSAG) approach. Additional sampler backends for generating
-  perturbed values for gradient estimation can be added via a plugin mechanism.
+  Gradient (StoSAG) approach. Additional samplers for generating perturbed
+  values for gradient estimation can be added via a plugin mechanism.
 - Support for linear and non-linear constraints, if supported by the chosen
-  optimization backend.
+  optimizer.
 - Flexible configuration of the optimization process using
   [`pydantic`](https://pydantic-docs.helpmanual.io/).
 - Support for tracking and processing optimization results generated during the
   optimization process.
 - Support for generating formatted tables of the results.
 - Optional support for exporting results as
   [`pandas`](https://pandas.pydata.org/) data frames or
```

### Comparing `ropt-0.2.1/docs/reference/evaluator.md` & `ropt-0.3.0/docs/reference/evaluator.md`

 * *Files identical despite different names*

### Comparing `ropt-0.2.1/docs/reference/realization_filters.md` & `ropt-0.3.0/docs/reference/realization_filters.md`

 * *Files identical despite different names*

### Comparing `ropt-0.2.1/docs/reference/results.md` & `ropt-0.3.0/docs/reference/results.md`

 * *Files identical despite different names*

### Comparing `ropt-0.2.1/docs/usage/robust_optimization.md` & `ropt-0.3.0/docs/usage/robust_optimization.md`

 * *Files 2% similar despite different names*

```diff
@@ -37,27 +37,27 @@
 factors. The evaluation of functions might be computationally expensive, and
 calculating their gradients analytically can be challenging or even impossible.
 For example, the functions may involve lengthy simulations of a physical process
 with numerous variables, utilizing numerical calculations that preclude
 straightforward analytical differentiation.
 
 `ropt` leverages standard optimization algorithms, such as those available in
-the [SciPy](https://www.scipy.org) package. These algorithms typically follow an
+the [SciPy](https://www.scipy.org) package. These methods typically follow an
 iterative approach, necessitating repeated assessments of the objective function
 and, in many cases, its gradient. Currently, it is assumed that the functions
 are not easily differentiated analytically. One of the core functions of `ropt`
 is to calculate gradients efficiently using stochastic methods.
 
 `ropt` is responsible for configuring and executing the optimization algorithm,
 building the overall function and gradient values from individual realizations,
 and monitoring both intermediate and final optimization results. It also offers
 the flexibility to delegate the actual calculations of functions to external
 code, for example, utilizing distributed resources like HPC clusters. `ropt`
 optionally provides its own code for this purpose.
 
 While many optimization scenarios involve a single run of a particular
-algorithm, there are cases where it proves beneficial to conduct multiple runs
+method, there are cases where it proves beneficial to conduct multiple runs
 using the same or different algorithms. For example, when dealing with a mix of
 continuous and discrete variables, it might be advantageous to employ different
-algorithms for each variable type. `ropt` facilitates this by offering a
+methods for each variable type. `ropt` facilitates this by offering a
 mechanism to run a workflow containing multiple optimizers, potentially of
 different types, in an alternating or nested fashion.
```

### Comparing `ropt-0.2.1/docs/usage/running.md` & `ropt-0.3.0/docs/usage/running.md`

 * *Files identical despite different names*

### Comparing `ropt-0.2.1/examples/de_linear.py` & `ropt-0.3.0/examples/de_linear.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Differential evaluation optimization example.
 
-This example uses the differential evolution algorithm to solve a discrete
+This example uses the differential evolution method to solve a discrete
 problem with a linear constraint.
 """
 
 from typing import Any, Dict
 
 import numpy as np
 from numpy.typing import NDArray
@@ -19,15 +19,15 @@
     "variables": {
         "initial_values": 2 * [0.0],
         "lower_bounds": [0.0, 0.0],
         "upper_bounds": [10.0, 10.0],
         "types": VariableType.INTEGER,
     },
     "optimizer": {
-        "algorithm": "differential_evolution",
+        "method": "differential_evolution",
         "options": {"integrality": [True, True], "seed": 4},
         "max_functions": 100,
         "parallel": True,
     },
     "linear_constraints": {
         "coefficients": [1.0, 1.0],
         "types": [ConstraintType.LE],
```

### Comparing `ropt-0.2.1/examples/de_nonlinear.py` & `ropt-0.3.0/examples/de_nonlinear.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Differential evaluation optimization example.
 
-This example uses the differential evolution algorithm to solve a discrete
+This example uses the differential evolution method to solve a discrete
 problem with a linear constraint, implemented as a non-linear constraint.
 """
 
 from typing import Any, Dict
 
 import numpy as np
 from numpy.typing import NDArray
@@ -19,15 +19,15 @@
     "variables": {
         "initial_values": 2 * [0.0],
         "types": VariableType.INTEGER,
         "lower_bounds": [0.0, 0.0],
         "upper_bounds": [10.0, 10.0],
     },
     "optimizer": {
-        "algorithm": "differential_evolution",
+        "method": "differential_evolution",
         "options": {"seed": 3},
         "max_functions": 100,
         "parallel": True,
     },
     "nonlinear_constraints": {
         "types": [ConstraintType.LE],
         "rhs_values": [10.0],
```

### Comparing `ropt-0.2.1/examples/rosenbrock_deterministic.py` & `ropt-0.3.0/examples/rosenbrock_deterministic.py`

 * *Files identical despite different names*

### Comparing `ropt-0.2.1/examples/rosenbrock_ensemble.py` & `ropt-0.3.0/examples/rosenbrock_ensemble.py`

 * *Files identical despite different names*

### Comparing `ropt-0.2.1/examples/script_optimizer/rosenbrock.py` & `ropt-0.3.0/examples/script_optimizer/rosenbrock.py`

 * *Files identical despite different names*

### Comparing `ropt-0.2.1/examples/script_optimizer/run.py` & `ropt-0.3.0/examples/script_optimizer/run.py`

 * *Files identical despite different names*

### Comparing `ropt-0.2.1/mkdocs.yml` & `ropt-0.3.0/mkdocs.yml`

 * *Files 7% similar despite different names*

```diff
@@ -65,15 +65,15 @@
       - "Optimization":
           - "Ensemble optimizer": reference/optimization.md
           - "Function evaluations": reference/evaluator.md
           - "Optimization results": reference/results.md
           - "Reporting": reference/reporting.md
       - "Plugins":
           - "Plugin manager": reference/plugins.md
-          - "Optimizer backends": reference/optimizer_backends.md
-          - "Sampler backends": reference/sampler_backends.md
+          - "Optimizer plugins": reference/optimizer_plugins.md
+          - "Sampler plugins": reference/sampler_plugins.md
           - "Realization filters": reference/realization_filters.md
           - "Function transforms": reference/function_transforms.md
           - "Optimization steps": reference/optimization_steps.md
       - "Enumerations": reference/enums.md
       - "Exceptions": reference/exceptions.md
       - "Utilities": reference/utilities.md
```

### Comparing `ropt-0.2.1/pyproject.toml` & `ropt-0.3.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -31,14 +31,29 @@
 [project.optional-dependencies]
 test = ["ruff", "mypy", "pytest", "pandas-stubs", "types-tabulate"]
 docs = ["mkdocs", "mkdocstrings[python]", "mkdocs-material", "mike"]
 pandas = ["pandas", "tabulate"]
 xarray = ["xarray", "netcdf4"]
 parsl = ["parsl"]
 
+[project.entry-points."ropt.plugins.optimizer"]
+scipy = "ropt.plugins.optimizer.scipy:SciPyOptimizerPlugin"
+
+[project.entry-points."ropt.plugins.sampler"]
+scipy = "ropt.plugins.sampler.scipy:SciPySamplerPlugin"
+
+[project.entry-points."ropt.plugins.realization_filter"]
+default = "ropt.plugins.realization_filter.default:DefaultRealizationFilterPlugin"
+
+[project.entry-points."ropt.plugins.function_transform"]
+default = "ropt.plugins.function_transform.default:DefaultFunctionTransformPlugin"
+
+[project.entry-points."ropt.plugins.optimization_step"]
+default = "ropt.plugins.optimization_steps.default:DefaultOptimizationStepsPlugin"
+
 [tool.setuptools.packages.find]
 where = ["src"]
 include = ["ropt"]
 
 [tool.setuptools.package-data]
 ropt = ["py.typed"]
```

### Comparing `ropt-0.2.1/src/ropt/apps/_script_optimizer.py` & `ropt-0.3.0/src/ropt/apps/_script_optimizer.py`

 * *Files identical despite different names*

### Comparing `ropt-0.2.1/src/ropt/config/enopt/__init__.py` & `ropt-0.3.0/src/ropt/config/enopt/__init__.py`

 * *Files identical despite different names*

### Comparing `ropt-0.2.1/src/ropt/config/enopt/_enopt_config.py` & `ropt-0.3.0/src/ropt/config/enopt/_enopt_config.py`

 * *Files identical despite different names*

### Comparing `ropt-0.2.1/src/ropt/config/enopt/_gradient_config.py` & `ropt-0.3.0/src/ropt/config/enopt/_gradient_config.py`

 * *Files identical despite different names*

### Comparing `ropt-0.2.1/src/ropt/config/enopt/_linear_constraints_config.py` & `ropt-0.3.0/src/ropt/config/enopt/_linear_constraints_config.py`

 * *Files identical despite different names*

### Comparing `ropt-0.2.1/src/ropt/config/enopt/_nonlinear_constraints_config.py` & `ropt-0.3.0/src/ropt/config/enopt/_nonlinear_constraints_config.py`

 * *Files identical despite different names*

### Comparing `ropt-0.2.1/src/ropt/config/enopt/_objective_functions_config.py` & `ropt-0.3.0/src/ropt/config/enopt/_objective_functions_config.py`

 * *Files identical despite different names*

### Comparing `ropt-0.2.1/src/ropt/config/enopt/_realization_filter_config.py` & `ropt-0.3.0/src/ropt/config/enopt/_realization_filter_config.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 """Configuration class for realization filters."""
 
 from __future__ import annotations
 
 from typing import Any, Dict
 
 from ._enopt_base_model import EnOptBaseModel
-from .constants import DEFAULT_REALIZATION_FILTER_BACKEND
 
 
 class RealizationFilterConfig(EnOptBaseModel):
     """The configuration class for realization filters.
 
     This class defines the configuration for realization filters, which are
     configured by the `realization_filters` field in an
@@ -20,27 +19,20 @@
     By default, the final objective and constraint functions and their gradients
     are calculated as a weighted function from all realizations. Realization
     filters are optionally used to change the weights of the individual
     realizations. For instance, this can be used to determine which subset of
     realizations should be used in calculating the final objective and
     constraint functions and their gradients by setting some weights to zero.
 
-    Filtering is performed by a realization filter backend, which provides the
-    methods that can be used to adjust the weights of the individual
-    realizations. The `backend` field is used to select the backend, which may
-    be either built-in or installed separately as a plugin. A backend may
-    implement multiple algorithms, and the `method` field determines which one
-    will be used. To further specify how such a method should function, the
-    `options` field can be used to pass a dictionary of key-value pairs. The
-    interpretation of these options depends on the backend and the chosen
+    The `method` field determines which method will be used to adjust the
+    weights of the individual realizations. To further specify how such a method
+    should function, the `options` field can be used to pass a dictionary of
+    key-value pairs. The interpretation of these options depends on the| chosen
     method.
 
     Attributes:
-        backend: The name of the realization filter backend (default:
-            [`DEFAULT_REALIZATION_FILTER_BACKEND`][ropt.config.enopt.constants.DEFAULT_REALIZATION_FILTER_BACKEND])
         method:  The realization filter method
         options: Options to be passed to the filter
     """
 
-    backend: str = DEFAULT_REALIZATION_FILTER_BACKEND
     method: str
     options: Dict[str, Any] = {}  # noqa: RUF012
```

### Comparing `ropt-0.2.1/src/ropt/config/enopt/_realizations_config.py` & `ropt-0.3.0/src/ropt/config/enopt/_realizations_config.py`

 * *Files identical despite different names*

### Comparing `ropt-0.2.1/src/ropt/config/enopt/_sampler_config.py` & `ropt-0.3.0/src/ropt/config/enopt/_sampler_config.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 """Configuration class for samplers."""
 
 from __future__ import annotations
 
-from typing import Any, Dict, Optional
+from typing import Any, Dict
 
 from ._enopt_base_model import EnOptBaseModel
-from .constants import DEFAULT_SAMPLER_BACKEND
 
 
 class SamplerConfig(EnOptBaseModel):
     """The sampler configuration class.
 
     This class defines the configuration for samplers, which are configured by
     the `samplers` field in an [`EnOptConfig`][ropt.config.enopt.EnOptConfig]
@@ -20,33 +19,27 @@
     the index of the sampler for each variable.
 
     Gradients are calculated from a set of perturbed variables, which may be
     deterministic or stochastic in nature. These perturbations are generally
     produced by sampler objects that produce perturbation values to add to the
     unperturbed variables.
 
-    Perturbation values are produced by a sampler backend, which provides the
-    methods that can be used. The `backend` field is used to select the backend,
-    which may be either built-in or installed separately as a plugin. A backend
-    may implement multiple algorithms, and the `method` field determines which
-    one will be used. To further specify how such a method should function, the
-    `options` field can be used to pass a dictionary of key-value pairs. The
-    interpretation of these options depends on the backend and the chosen
-    method.
+    Perturbation values are produced by a sampler, which provides the methods
+    that can be used. The `method` field determines which sampler method will be
+    used. To further specify how such a method should function, the `options`
+    field can be used to pass a dictionary of key-value pairs. The
+    interpretation of these options depends on the chosen method.
 
     By default, a different set of perturbed variables is generated for each
     realization. By setting the `shared` flag to `True`, the sampler can be
     directed to use the same set of perturbed values for each realization.
 
     Attributes:
-        backend: The name of the sampler backend (default:
-            [`DEFAULT_SAMPLER_BACKEND`][ropt.config.enopt.constants.DEFAULT_SAMPLER_BACKEND])
         method:  The sampler method
         options: Options to be passed to the sampler
         shared:  Whether perturbation values should be shared between realizations
                 (default: `False`)
     """
 
-    backend: str = DEFAULT_SAMPLER_BACKEND
-    method: Optional[str] = None
+    method: str = "scipy/default"
     options: Dict[str, Any] = {}  # noqa: RUF012
     shared: bool = False
```

### Comparing `ropt-0.2.1/src/ropt/config/enopt/_utils.py` & `ropt-0.3.0/src/ropt/config/enopt/_utils.py`

 * *Files identical despite different names*

### Comparing `ropt-0.2.1/src/ropt/config/enopt/_variables_config.py` & `ropt-0.3.0/src/ropt/config/enopt/_variables_config.py`

 * *Files 3% similar despite different names*

```diff
@@ -42,27 +42,26 @@
     number of variables, and the `initial_values`, `lower_bounds`, and
     `upper_bounds` fields are broadcasted accordingly. If `names` is not
     provided, these fields are broadcasted to each other, and their final size
     determines the number of variables.
 
     Info: Variable Names
         `ropt` does not use the names itself, and names can be of arbitrary
-        type, as long as they are unique. However, some optimization backends or
-        external code might need a string representation of each name, which can
-        be obtained using the
+        type, as long as they are unique. However, some optimizers or external
+        code might need a string representation of each name, which can be
+        obtained using the
         [`get_formatted_names`][ropt.config.enopt.VariablesConfig.get_formatted_names]
         method. The `delimiters` attribute is used by this method to convert the
         special case of names consisting of tuples of strings.
 
     The optional `types` field can be used to assign types to each variable,
     according to the [`VariableType`][ropt.enums.VariableType] enumeration. The
-    values can be used by the optimization backends to configure the algorithm
-    accordingly. If not provided, all variables are assumed to be continuous and
-    of real data type (corresponding to
-    [`VariableType.REAL`][ropt.enums.VariableType.REAL])
+    values can be used to configure the optimizer accordingly. If not provided,
+    all variables are assumed to be continuous and of real data type
+    (corresponding to [`VariableType.REAL`][ropt.enums.VariableType.REAL])
 
     The `offsets` and `scales` fields are optional: if given, they are
     broadcasted to the number of variables and used for scaling. The elements
     $x_i$ of `initial_values`, `lower_bounds`, and `upper_bounds` fields are
     rescaled by the elements $o_i$ and $s_i$ of `offsets` and `scales`: $(x_i -
     o_i) / s_i$.
```

### Comparing `ropt-0.2.1/src/ropt/config/plan/__init__.py` & `ropt-0.3.0/src/ropt/config/plan/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,18 +9,16 @@
     EvaluatorStepConfig,
     OptimizerStepConfig,
     RestartStepConfig,
     TrackerStepConfig,
     UpdateConfigStepConfig,
 )
 from ._plan_config import PlanConfig
-from ._step_config import StepConfig
 
 __all__ = [
     "EvaluatorStepConfig",
     "OptimizerStepConfig",
     "PlanConfig",
     "RestartStepConfig",
-    "StepConfig",
     "TrackerStepConfig",
     "UpdateConfigStepConfig",
 ]
```

### Comparing `ropt-0.2.1/src/ropt/config/plan/_config.py` & `ropt-0.3.0/src/ropt/config/plan/_config.py`

 * *Files identical despite different names*

### Comparing `ropt-0.2.1/src/ropt/config/utils.py` & `ropt-0.3.0/src/ropt/config/utils.py`

 * *Files identical despite different names*

### Comparing `ropt-0.2.1/src/ropt/enums.py` & `ropt-0.3.0/src/ropt/enums.py`

 * *Files identical despite different names*

### Comparing `ropt-0.2.1/src/ropt/evaluator/__init__.py` & `ropt-0.3.0/src/ropt/evaluator/__init__.py`

 * *Files identical despite different names*

### Comparing `ropt-0.2.1/src/ropt/evaluator/_ensemble_evaluator.py` & `ropt-0.3.0/src/ropt/evaluator/_ensemble_evaluator.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Any, Dict, Iterator, List, Optional, Tuple
+from typing import TYPE_CHECKING, Iterator, List, Optional, Tuple
 
 import numpy as np
 
 from ropt.results import (
     FunctionEvaluations,
     FunctionResults,
     Functions,
@@ -32,17 +32,17 @@
 
 if TYPE_CHECKING:
     from numpy.random import Generator
     from numpy.typing import NDArray
 
     from ropt.config.enopt import EnOptConfig
     from ropt.plugins import PluginManager
-    from ropt.plugins.function_transform.protocol import FunctionTransform
-    from ropt.plugins.realization_filter.protocol import RealizationFilter
-    from ropt.plugins.sampler.protocol import Sampler
+    from ropt.plugins.function_transform.protocol import FunctionTransformProtocol
+    from ropt.plugins.realization_filter.protocol import RealizationFilterProtocol
+    from ropt.plugins.sampler.protocol import SamplerProtocol
 
     from ._evaluator import Evaluator
 
 
 class EnsembleEvaluator:
     def __init__(  # noqa: PLR0913
         self,
@@ -114,15 +114,15 @@
                 self._evaluator,
                 variables,
                 active_objectives,
                 active_constraints,
             )
         )
 
-        # Gradient-based algorithms are currently not parallelized, and there is
+        # Gradient-based methods are currently not parallelized, and there is
         # only one function result. That function may be needed in a gradient
         # calculation, so it is cached here:
         self._cache_for_gradient = function_results[0]
 
         return function_results
 
     def _calculate_one_set_of_functions(
@@ -596,62 +596,45 @@
         assert self._config.nonlinear_constraints is not None
         if auto_scales is None:
             return self._config.nonlinear_constraints.scales
         return self._config.nonlinear_constraints.scales * auto_scales
 
     def _init_realization_filters(
         self, plugin_manager: PluginManager
-    ) -> List[RealizationFilter]:
-        backend_names = {
-            filter_config.backend for filter_config in self._config.realization_filters
-        }
-        backends = {
-            name: plugin_manager.get_backend("realization_filter", name)
-            for name in backend_names
-        }
+    ) -> List[RealizationFilterProtocol]:
         return [
-            backends[filter_config.backend](self._config, idx)
+            plugin_manager.get_plugin(
+                "realization_filter", method=filter_config.method
+            ).create(self._config, idx)
             for idx, filter_config in enumerate(self._config.realization_filters)
         ]
 
     def _init_function_transforms(
         self, plugin_manager: PluginManager
-    ) -> List[FunctionTransform]:
-        backend_names = {
-            transform_config.backend
-            for transform_config in self._config.function_transforms
-        }
-        backends = {
-            name: plugin_manager.get_backend("function_transform", name)
-            for name in backend_names
-        }
+    ) -> List[FunctionTransformProtocol]:
         return [
-            backends[transform_config.backend](self._config, idx)
+            plugin_manager.get_plugin(
+                "function_transform", method=transform_config.method
+            ).create(self._config, idx)
             for idx, transform_config in enumerate(self._config.function_transforms)
         ]
 
     def _init_samplers(
         self, rng: Generator, plugin_manager: PluginManager
-    ) -> List[Sampler]:
-        samplers: List[Sampler] = []
-        backends: Dict[str, Any] = {}
+    ) -> List[SamplerProtocol]:
+        samplers: List[SamplerProtocol] = []
         for idx, sampler_config in enumerate(self._config.samplers):
             variable_indices = _get_indices(
                 idx, self._config.gradient.samplers, self._config.variables.indices
             )
             if variable_indices is None or variable_indices.size:
-                if sampler_config.backend not in backends:
-                    backends[sampler_config.backend] = plugin_manager.get_backend(
-                        "sampler", sampler_config.backend
-                    )
-                samplers.append(
-                    backends[sampler_config.backend](
-                        self._config, idx, variable_indices, rng
-                    )
+                plugin = plugin_manager.get_plugin(
+                    "sampler", method=sampler_config.method
                 )
+                samplers.append(plugin.create(self._config, idx, variable_indices, rng))
         return samplers
 
 
 def _get_indices(
     idx: int,
     gradient_indices: Optional[NDArray[np.intc]],
     variable_indices: Optional[NDArray[np.intc]],
```

### Comparing `ropt-0.2.1/src/ropt/evaluator/_evaluator.py` & `ropt-0.3.0/src/ropt/evaluator/_evaluator.py`

 * *Files identical despite different names*

### Comparing `ropt-0.2.1/src/ropt/evaluator/_evaluator_results.py` & `ropt-0.3.0/src/ropt/evaluator/_evaluator_results.py`

 * *Files identical despite different names*

### Comparing `ropt-0.2.1/src/ropt/evaluator/_function.py` & `ropt-0.3.0/src/ropt/evaluator/_function.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from typing import List, Optional
 
 import numpy as np
 from numpy.typing import NDArray
 
 from ropt.config.enopt import EnOptConfig
-from ropt.plugins.function_transform.protocol import FunctionTransform
+from ropt.plugins.function_transform.protocol import FunctionTransformProtocol
 
 
 def _calculate_transformed_functions(  # noqa: PLR0913
     config: EnOptConfig,
-    function_transforms: List[FunctionTransform],
+    function_transforms: List[FunctionTransformProtocol],
     functions: NDArray[np.float64],
     realization_weights: Optional[NDArray[np.float64]],
     failed_realizations: NDArray[np.bool_],
     *,
     constraints: bool = False,
 ) -> NDArray[np.float64]:
     result: NDArray[np.float64] = np.empty(functions.shape[-1], dtype=np.float64)
@@ -39,15 +39,15 @@
         )
 
     return result
 
 
 def _add_transformed_functions(  # noqa: PLR0913
     config: EnOptConfig,
-    transform: FunctionTransform,
+    transform: FunctionTransformProtocol,
     functions: NDArray[np.float64],
     realization_weights: Optional[NDArray[np.float64]],
     failed_realizations: NDArray[np.bool_],
     mask: NDArray[np.bool_],
     result: NDArray[np.float64],
 ) -> None:
     for idx in np.where(mask)[0]:
```

### Comparing `ropt-0.2.1/src/ropt/evaluator/_gradient.py` & `ropt-0.3.0/src/ropt/evaluator/_gradient.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from typing import List, Optional
 
 import numpy as np
 from numpy.typing import NDArray
 
 from ropt.config.enopt import EnOptConfig, GradientConfig, VariablesConfig
 from ropt.enums import BoundaryType
-from ropt.plugins.function_transform.protocol import FunctionTransform
-from ropt.plugins.sampler.protocol import Sampler
+from ropt.plugins.function_transform.protocol import FunctionTransformProtocol
+from ropt.plugins.sampler.protocol import SamplerProtocol
 
 SVD_TOLERANCE = 0.999
 MIRROR_REPEAT = 3
 
 
 def _apply_bounds(
     variables: NDArray[np.float64],
@@ -63,15 +63,15 @@
     return result
 
 
 def _perturb_variables(
     variables: NDArray[np.float64],
     variables_config: VariablesConfig,
     gradient_config: GradientConfig,
-    samplers: List[Sampler],
+    samplers: List[SamplerProtocol],
 ) -> NDArray[np.float64]:
     if gradient_config.samplers is None:
         samples = samplers[0].generate_samples()
     else:
         # The results should be independent of the order of the samplers,
         # reordering would affect the random numbers they are based on. We
         # obtain a consistent order by running multiple samplers in the order
@@ -134,15 +134,15 @@
 
 def _calculate_gradient(  # noqa: PLR0913
     functions: NDArray[np.float64],
     delta_variables: NDArray[np.float64],
     delta_functions: NDArray[np.float64],
     failed_realizations: NDArray[np.bool_],
     weights: NDArray[np.float64],
-    transform: FunctionTransform,
+    transform: FunctionTransformProtocol,
     *,
     merge_realizations: bool,
 ) -> NDArray[np.float64]:
     weights = np.where(failed_realizations, 0.0, weights)
     weights /= weights.sum()
     if merge_realizations:
         gradients = _estimate_merged_gradient(delta_variables, delta_functions, weights)
@@ -150,15 +150,15 @@
         gradients = _estimate_gradients(delta_variables, delta_functions, weights)
     return transform.calculate_gradient(functions, gradients, weights)
 
 
 # : disable=too-many-arguments,too-many-locals
 def _calculate_transformed_gradients(  # noqa: PLR0913
     config: EnOptConfig,
-    function_transforms: List[FunctionTransform],
+    function_transforms: List[FunctionTransformProtocol],
     variables: NDArray[np.float64],
     functions: NDArray[np.float64],
     perturbed_variables: NDArray[np.float64],
     perturbed_functions: NDArray[np.float64],
     realization_weights: Optional[NDArray[np.float64]],
     failed_realizations: NDArray[np.bool_],
     *,
@@ -191,15 +191,15 @@
         )
 
     return gradients
 
 
 def _add_transformed_gradients(  # noqa: PLR0913
     config: EnOptConfig,
-    transform: FunctionTransform,
+    transform: FunctionTransformProtocol,
     delta_variables: NDArray[np.float64],
     functions: NDArray[np.float64],
     delta_functions: NDArray[np.float64],
     realization_weights: Optional[NDArray[np.float64]],
     failed_realizations: NDArray[np.bool_],
     mask: NDArray[np.bool_],
     gradients: NDArray[np.float64],
```

### Comparing `ropt-0.2.1/src/ropt/evaluator/_utils.py` & `ropt-0.3.0/src/ropt/evaluator/_utils.py`

 * *Files identical despite different names*

### Comparing `ropt-0.2.1/src/ropt/evaluator/parsl.py` & `ropt-0.3.0/src/ropt/evaluator/parsl.py`

 * *Files 4% similar despite different names*

```diff
@@ -63,25 +63,27 @@
         self,
         workflow: Callable[..., Any],
         *,
         monitor: Optional[Callable[..., Any]] = None,
         provider: Optional[ExecutionProvider] = None,
         max_threads: int = 4,
         retries: int = 0,
+        enable_cache: bool = True,
     ) -> None:
         """Create a parsl evaluator object.
 
         Args:
-            provider:    Parsl execution provider to use. By default `LocalProvider`
-            workflow:    Callback to start a single workflow run
-            monitor:     Monitor function
-            max_threads: Maximum number of threads for local execution. Defaults to 4
-            retries:     Number of retries upon failure of a task. Defaults to 0
+            provider:     Parsl execution provider to use. By default `LocalProvider`
+            workflow:     Callback to start a single workflow run
+            monitor:      Monitor function
+            max_threads:  Maximum number of threads for local execution. Defaults to 4
+            retries:      Number of retries upon failure of a task. Defaults to 0
+            enable_cache: If `True` enable function value caching.
         """
-        super().__init__()
+        super().__init__(enable_cache=enable_cache)
 
         self._batch_id: int
         self._variables: NDArray[np.float64]
         self._jobs: Dict[int, List[Task]] = {}
         self._workflow = workflow
         self._monitor = monitor
 
@@ -106,27 +108,28 @@
         )
 
     def launch(
         self,
         batch_id: int,
         variables: NDArray[np.float64],
         context: EvaluatorContext,
+        active: Optional[NDArray[np.bool_]],
     ) -> Dict[int, ConcurrentTask]:
         """Launch the parsl task.
 
         See the [ropt.evaluator.ConcurrentEvaluator][] abstract base class.
 
         # noqa
         """
         self._batch_id = batch_id
         self._variables = variables
         self._jobs = {
             job_idx: self._workflow(batch_id, job_idx, variables, context)
             for job_idx in range(variables.shape[0])
-            if context.active is None or context.active[job_idx]
+            if active is None or active[job_idx]
         }
         return {idx: futures[-1] for idx, futures in self._jobs.items()}
 
     def monitor(self) -> None:
         """Monitor the tasks of all jobs.
 
         See the [ropt.evaluator.ConcurrentEvaluator][] abstract base class.
```

### Comparing `ropt-0.2.1/src/ropt/events.py` & `ropt-0.3.0/src/ropt/events.py`

 * *Files identical despite different names*

### Comparing `ropt-0.2.1/src/ropt/exceptions.py` & `ropt-0.3.0/src/ropt/exceptions.py`

 * *Files identical despite different names*

### Comparing `ropt-0.2.1/src/ropt/optimization/_bases.py` & `ropt-0.3.0/src/ropt/optimization/_bases.py`

 * *Files identical despite different names*

### Comparing `ropt-0.2.1/src/ropt/optimization/_ensemble_optimizer.py` & `ropt-0.3.0/src/ropt/optimization/_ensemble_optimizer.py`

 * *Files identical despite different names*

### Comparing `ropt-0.2.1/src/ropt/optimization/_events.py` & `ropt-0.3.0/src/ropt/optimization/_events.py`

 * *Files identical despite different names*

### Comparing `ropt-0.2.1/src/ropt/optimization/_optimizer.py` & `ropt-0.3.0/src/ropt/optimization/_optimizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,17 +46,17 @@
 
         # Whether NaN values are allowed:
         self._allow_nan = False
 
     def start(self, variables: NDArray[np.float64]) -> OptimizerExitCode:
         self._fixed_variables = variables.copy()
 
-        optimizer = self._plugin_manager.get_backend(
-            "optimizer", self._enopt_config.optimizer.backend
-        )(self._enopt_config, self._optimizer_callback)
+        optimizer = self._plugin_manager.get_plugin(
+            "optimizer", method=self._enopt_config.optimizer.method
+        ).create(self._enopt_config, self._optimizer_callback)
         self._allow_nan = optimizer.allow_nan
 
         exit_code = OptimizerExitCode.OPTIMIZER_STEP_FINISHED
         try:
             optimizer.start(variables)
         except OptimizationAborted as exc:
             exit_code = exc.exit_code
@@ -80,15 +80,14 @@
         nested_results, aborted = self._optimizer_step.run_nested_plan(variables)
         if nested_results is not None:
             if aborted:
                 raise OptimizationAborted(exit_code=OptimizerExitCode.USER_ABORT)
             variables = nested_results.evaluations.variables.copy()
             self._fixed_variables = variables.copy()
 
-        # TODO: After a nested step, we may be able to re-use its result:
         results = self._run_evaluations(
             variables,
             compute_functions=return_functions,
             compute_gradients=return_gradients,
         )
 
         # Functions and gradients might need to be scaled:
```

### Comparing `ropt-0.2.1/src/ropt/optimization/_plan.py` & `ropt-0.3.0/src/ropt/optimization/_plan.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from ropt.optimization import BasicStep, LabelStep, TrackerStep
 from ropt.utils import update_dict
 
 if TYPE_CHECKING:
     import numpy as np
     from numpy.typing import NDArray
 
-    from ropt.config.plan import PlanConfig, StepConfig
+    from ropt.config.plan import PlanConfig
     from ropt.evaluator import Evaluator
     from ropt.plugins import PluginManager
     from ropt.results import FunctionResults, Results
 
     from ._events import OptimizationEventBroker
 
 
@@ -180,24 +180,23 @@
         assert self._enopt_config is not None
         assert self._enopt_config.original_inputs is not None
         self._enopt_config = EnOptConfig.model_validate(
             update_dict(self._enopt_config.original_inputs, updates)
         )
 
     def _create_steps(
-        self, plan_config: Tuple[StepConfig, ...]
+        self, plan_config: Tuple[Dict[str, Any], ...]
     ) -> Tuple[Tuple[Any, ...], Tuple[TrackerStep, ...]]:
-        backend_names = {step_config.backend for step_config in plan_config}
-        backends = {
-            name: self._context.plugin_manager.get_backend("optimization_step", name)
-            for name in backend_names
-        }
         all_steps = [
-            backends[config.backend](config, self._context, self)
-            for config in plan_config
+            self._context.plugin_manager.get_plugin(
+                "optimization_step", method=next(iter(step_config))
+            )
+            .create(self._context, self)
+            .get_step(step_config)
+            for step_config in plan_config
         ]
         steps: List[Any] = []
         trackers: List[TrackerStep] = []
         steps, trackers = [], []
         for step in all_steps:
             if isinstance(step, TrackerStep):
                 trackers.append(step)
```

### Comparing `ropt-0.2.1/src/ropt/plugins/__init__.py` & `ropt-0.3.0/src/ropt/plugins/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,37 +3,37 @@
 The core functionality of `ropt` can be extended through plugins, which can
 either be built-in, separately installed, or dynamically added at runtime.
 
 Various types of plugins provide specific functionalities. Currently, `ropt`
 supports the following plugin types:
 
 1. [`optimizer`][ropt.plugins.optimizer]:
-    Backends that implement specific optimization algorithms.
+    Plugins that implement specific optimization methods.
 2. [`sampler`][ropt.plugins.sampler]:
-    Backends responsible for generating perturbations.
+    Plugins responsible for generating perturbations.
 3. [`realization_filter`][ropt.plugins.realization_filter]:
     Filters used to determine subsets of realizations.
 4. [`function_transform`][ropt.plugins.function_transform]:
     Code used to compute objective and constraint values from realizations.
 5. [`optimization_step`][ropt.plugins.optimization_steps]:
     Steps evaluated within an optimization plan.
 
 Plugins are managed by the [`PluginManager`][ropt.plugins.PluginManager] class.
 They can be built-in, installed separately using the standard entry points
 mechanism, or added dynamically using the
-[`add_backends`][ropt.plugins.PluginManager.add_backends] method. Protocols or
+[`add_plugins`][ropt.plugins.PluginManager.add_plugins] method. Protocols or
 abstract classes define the interface that plugin code must adhere to in order
 to implement the required functionality.
 
 The plugin manager object provides the
-[`get_backend`][ropt.plugins.PluginManager.get_backend] method, which `ropt`
-uses to retrieve the necessary plugin based on its type and name. Given the
-plugin's type and name, this method returns a callable (either a class or a
-factory function) that `ropt` uses to instantiate the plugin when needed.
+[`get_plugin`][ropt.plugins.PluginManager.get_plugin] method, which `ropt` uses
+to retrieve the necessary plugin based on its type and name. Given the plugin's
+type and name, this method returns a callable (either a class or a factory
+function) that `ropt` uses to instantiate the plugin when needed.
 """
 
-from ._manager import BackendType, PluginManager
+from ._manager import PluginManager, PluginType
 
 __all__ = [
-    "BackendType",
+    "PluginType",
     "PluginManager",
 ]
```

### Comparing `ropt-0.2.1/src/ropt/plugins/_manager.py` & `ropt-0.3.0/src/ropt/plugins/_manager.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,156 +1,166 @@
 """The plugin manager."""
 
 from __future__ import annotations
 
 import contextlib
 import sys
 from functools import lru_cache
-from typing import Any, Dict, Literal
+from typing import TYPE_CHECKING, Any, Dict, Literal
 
 from ropt.exceptions import ConfigError
 
+if TYPE_CHECKING:
+    from ropt.plugins.protocol import PluginProtocol
+
 if sys.version_info >= (3, 10):
     from importlib.metadata import entry_points
 else:
     from importlib_metadata import entry_points
 
-BackendType = Literal[
+PluginType = Literal[
     "optimizer",
     "sampler",
     "realization_filter",
     "function_transform",
     "optimization_step",
 ]
 """ Plugin Types Supported by `ropt`
 
 `ropt` supports various types of plugins for different functionalities:
 
 `optimizer`:
-: These plugins implement optimizer backends providing optimization algorithms.
-  The default backend is `scipy`, utilizing the
+: These plugins implement optimizer plugins providing optimization methods.
+  The default plugin is `scipy`, utilizing the
   [`scipy.optimize`](https://docs.scipy.org/doc/scipy/reference/optimize.html)
   module.
 
 `sampler`:
-: These plugins implement sampler backends generating perturbations for
-  estimating gradients. By default, a backend based on
+: These plugins implement sampler plugins generating perturbations for
+  estimating gradients. By default, a plugin based on
   [`scipy.stats`](https://docs.scipy.org/doc/scipy/reference/stats.html) is
   installed:
 
 `realization_filter`:
 : These plugins implement filters for selecting a sub-set of realizations used
   in calculating objective or constraint functions and their gradients. The
-  default backend provides filters based on ranking and for CVaR optimization.
+  default plugin provides filters based on ranking and for CVaR optimization.
 
 `function_transform`:
 : These plugins implement the final objective and gradient from sets of
   objectives or constraints and their gradients for individual realizations. The
   default built-in plugin supports objectives defined by the mean or standard
   deviation of these values.
 
 `optimization_step`:
 : Optimization step plugins implement the steps evaluated during the execution
-  plan. The built-in backend offers a full set of steps for executing complex
+  plan. The built-in plugin offers a full set of steps for executing complex
   plans.
 """
 
 
 class PluginManager:
     """The plugin manager."""
 
     def __init__(self) -> None:
         """Initialize the plugin manager.
 
-        The plugin manager object is initialized with the built-in plugins and
-        all plugins installed via the entry points mechanism (see
+        The plugin manager object is initialized via the entry points mechanism
+        (see
         [`importlib.metadata`](https://docs.python.org/3/library/importlib.metadata.html)).
 
-        For instance, to install an additional optimizer backend, implemented in
+        For instance, to install an additional optimizer plugin, implemented in
         an independent package, and assuming installation via a `pyproject.toml`
         file, add the following:
 
         ```toml
         [project.entry-points."ropt.plugins.optimizer"]
-        my_optimizer = "my_optimizer_pkg.basic_backend:MyOptimizer"
+        my_optimizer = "my_optimizer_pkg.my_plugin:MyOptimizer"
         ```
 
         This will make the `MyOptimizer` class from the `my_optimizer_pkg`
         package available under the name `my_optimizer`.
 
-        Plugins can also be added dynamically using the add_backends method.
+        Plugins can also be added dynamically using the add_plugins method.
         """
-        # Not done globally to avoid circular imports:
-        import ropt.plugins.function_transform.default
-        import ropt.plugins.optimization_steps.default
-        import ropt.plugins.optimizer.scipy
-        import ropt.plugins.realization_filter.default
-        import ropt.plugins.sampler.scipy
-
-        # Built-in plugins, listed for all possible backend types:
-        self._backend_classes: Dict[BackendType, Dict[str, Any]] = {
-            "optimizer": {
-                "scipy": ropt.plugins.optimizer.scipy.SciPyOptimizer,
-            },
-            "sampler": {
-                "scipy": ropt.plugins.sampler.scipy.SciPySampler,
-            },
-            "realization_filter": {
-                "default": ropt.plugins.realization_filter.default.DefaultRealizationFilter,
-            },
-            "function_transform": {
-                "default": ropt.plugins.function_transform.default.DefaultFunctionTransform,
-            },
-            "optimization_step": {
-                "default": ropt.plugins.optimization_steps.default.get_step,
-            },
+        # Built-in plugins, listed for all possible plugin types:
+        self._plugins: Dict[PluginType, Dict[str, PluginProtocol]] = {
+            "optimizer": {},
+            "sampler": {},
+            "realization_filter": {},
+            "function_transform": {},
+            "optimization_step": {},
         }
 
-        for backend_type in self._backend_classes:
-            self.add_backends(backend_type, _from_entry_points(backend_type))
+        for plugin_type in self._plugins:
+            self.add_plugins(plugin_type, _from_entry_points(plugin_type))
 
-    def add_backends(self, backend_type: BackendType, backends: Dict[str, Any]) -> None:
-        """Add a backend at runtime.
+    def add_plugins(
+        self, plugin_type: PluginType, plugins: Dict[str, PluginProtocol]
+    ) -> None:
+        """Add a plugin at runtime.
 
-        This method adds one or more backends of a specific type to the plugin
-        manager. The `backends` argument maps the names of the new plugins to a
+        This method adds one or more plugins of a specific type to the plugin
+        manager. The `plugins` argument maps the names of the new plugins to a
         callable that creates the plugin. The callable can be any function or
         class that creates a plugin object.
 
         The plugin names are case-insensitive.
 
         Args:
-            backend_type: Type of the backend.
-            backends:     Dictionary of plugins.
+            plugin_type: Type of the plugin.
+            plugins:     Dictionary of plugins.
         """
-        for name, backend in backends.items():
+        for name, plugin in plugins.items():
             name_lower = name.lower()
-            if name_lower in self._backend_classes[backend_type]:
-                msg = f"Duplicate backend name: {name_lower}"
+            if name_lower in self._plugins[plugin_type]:
+                msg = f"Duplicate plugin name: {name_lower}"
+                raise ConfigError(msg)
+            self._plugins[plugin_type][name_lower] = plugin
+
+    def get_plugin(self, plugin_type: PluginType, method: str) -> Any:  # noqa: ANN401
+        """Retrieve a plugin by type and method name.
+
+        Args:
+            plugin_type: The type of the plugin to retrieve.
+            method:      The name of the method the plugin should provide.
+        """
+        plugin_name, sep, method_name = method.rpartition("/")
+
+        if sep == "/":
+            assert method_name != ""
+            plugin = self._plugins[plugin_type].get(plugin_name.lower())
+            if plugin is None:
+                msg = f"Plugin not found: {method}"
                 raise ConfigError(msg)
-            self._backend_classes[backend_type][name_lower] = backend
+            return plugin
+
+        for plugin in self._plugins[plugin_type].values():
+            if plugin.is_supported(method_name):
+                return plugin
 
-    def get_backend(self, backend_type: BackendType, plugin_name: str) -> Any:  # noqa: ANN401
-        """Retrieve a backend by type and plugin name.
+        msg = f"Method not found: {method}"
+        raise ConfigError(msg)
 
-        Given a type and plugin name, this method returns a callable that can be
-        used to create a plugin object.
+    def is_supported(self, plugin_type: PluginType, method: str) -> bool:
+        """Check if a method is supported.
 
         Args:
-            backend_type: The type of the backend to retrieve.
-            plugin_name:  The name of the plugin that implements the backend.
+            plugin_type: The type of the plugin to retrieve.
+            method:      The name of the method the plugin should provide.
         """
-        plugin = self._backend_classes[backend_type].get(plugin_name.lower())
-        if plugin is None:
-            backend_name = backend_type.replace("_", " ").capitalize()
-            msg = f"{backend_name} backend not supported: {plugin_name}"
-            raise ConfigError(msg)
-        return plugin
+        _, _, method_name = method.rpartition("/")
+        try:
+            plugin = self.get_plugin(plugin_type, method)
+        except ConfigError:
+            return False
+        return bool(plugin.is_supported(method_name))
 
 
 @lru_cache  # Without the cache, repeated calls are very slow
-def _from_entry_points(plugin_type: str) -> Dict[str, Any]:
-    plugins: Dict[str, Any] = {}
+def _from_entry_points(plugin_type: str) -> Dict[str, PluginProtocol]:
+    plugins: Dict[str, PluginProtocol] = {}
     for entry_point in entry_points().select(group=f"ropt.plugins.{plugin_type}"):
         with contextlib.suppress(ModuleNotFoundError):
-            plugins[entry_point.name] = entry_point.load()
+            plugin = entry_point.load()
+            plugins[entry_point.name] = plugin()
     return plugins
```

### Comparing `ropt-0.2.1/src/ropt/plugins/function_transform/default.py` & `ropt-0.3.0/src/ropt/plugins/function_transform/default.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,21 +5,23 @@
 import numpy as np
 from numpy.typing import NDArray
 
 from ropt.config.enopt import EnOptConfig
 from ropt.enums import OptimizerExitCode
 from ropt.exceptions import ConfigError, OptimizationAborted
 
+from .protocol import FunctionTranformPluginProtocol, FunctionTransformProtocol
+
 _MIN_STDDEV_REALIZATIONS = 2
 
 
-class DefaultFunctionTransform:
+class DefaultFunctionTransform(FunctionTransformProtocol):
     """The default function transform plugin.
 
-    This backend currently implements two methods:
+    This plugin currently implements two methods:
 
     `mean`:
     :  Calculate the combined functions as a weighted mean of the function
        values of each realization. Gradients are accordingly calculated as
        a weighted sum.
 
     `stddev`:
@@ -29,39 +31,38 @@
        deviation is always minimized.
     """
 
     def __init__(self, enopt_config: EnOptConfig, transform_index: int) -> None:
         """Initialize the function transform object.
 
         See the
-        [ropt.plugins.function_transform.protocol.FunctionTransform][]
+        [ropt.plugins.function_transform.protocol.FunctionTransformProtocol][]
         protocol.
 
         # noqa
         """
         self._enopt_config = enopt_config
         self._transform_config = enopt_config.function_transforms[transform_index]
-        if self._transform_config.method is None:
+        _, _, self._method = self._transform_config.method.lower().rpartition("/")
+        if self._method == "default":
             self._method = "mean"
-        else:
-            self._method = self._transform_config.method.lower()
         if self._method == "stddev" and self._enopt_config.gradient.merge_realizations:
             msg = (
                 "The stddev transform does not support merging "
                 "realizations in the gradient."
             )
             raise ConfigError(msg)
 
     def calculate_function(
         self, functions: NDArray[np.float64], weights: NDArray[np.float64]
     ) -> NDArray[np.float64]:
         """Calculate a function from function values for each realization.
 
         See the
-        [ropt.plugins.function_transform.protocol.FunctionTransform][]
+        [ropt.plugins.function_transform.protocol.FunctionTransformProtocol][]
         protocol.
 
         # noqa
         """
         transform_method = self._method
         if transform_method == "mean":
             return self._calculate_function_mean(functions, weights)
@@ -75,15 +76,15 @@
         functions: NDArray[np.float64],
         gradient: NDArray[np.float64],
         weights: NDArray[np.float64],
     ) -> NDArray[np.float64]:
         """Calculate a gradient from gradients of the realizations.
 
         See the
-        [ropt.plugins.function_transform.protocol.FunctionTransform][]
+        [ropt.plugins.function_transform.protocol.FunctionTransformProtocol][]
         protocol.
 
         # noqa
         """
         transform_method = self._method
         if transform_method == "mean":
             return self._calculate_gradient_mean(functions, gradient, weights)
@@ -146,7 +147,31 @@
         norm = float(np.count_nonzero(weights > 0))
         norm = norm / (norm - 1)
         mean = np.dot(functions, weights)
         stddev = np.sqrt(
             norm * np.dot((functions - mean[..., np.newaxis]) ** 2, weights)
         )
         return norm, mean, stddev
+
+
+class DefaultFunctionTransformPlugin(FunctionTranformPluginProtocol):
+    """Default filter transform plugin class."""
+
+    def create(
+        self, enopt_config: EnOptConfig, transform_index: int
+    ) -> DefaultFunctionTransform:
+        """Initialize the realization filter plugin.
+
+        See the [ropt.plugins.function_transform.protocol.FunctionTranformPluginProtocol][] protocol.
+
+        # noqa
+        """
+        return DefaultFunctionTransform(enopt_config, transform_index)
+
+    def is_supported(self, method: str) -> bool:
+        """Check if a method is supported.
+
+        See the [ropt.plugins.protocol.Plugin][] protocol.
+
+        # noqa
+        """
+        return method.lower() in {"default", "mean", "stddev"}
```

### Comparing `ropt-0.2.1/src/ropt/plugins/function_transform/protocol.py` & `ropt-0.3.0/src/ropt/plugins/function_transform/protocol.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 """This module defines the protocol to be followed by function transforms.
 
 Function transforms can be added via the plugin mechanism to implement
 additional ways to functions and gradient ensembles. Any object that follows the
-[`FunctionTransform`][ropt.plugins.function_transform.protocol.FunctionTransform]
+[`FunctionTransform`][ropt.plugins.function_transform.protocol.FunctionTransformProtocol]
 protocol may be installed as a plugin.
 """
 
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Protocol
 
+from ropt.plugins.protocol import PluginProtocol
+
 if TYPE_CHECKING:
     import numpy as np
     from numpy.typing import NDArray
 
     from ropt.config.enopt import EnOptConfig
 
 
-class FunctionTransform(Protocol):
+class FunctionTransformProtocol(Protocol):
     """Protocol class for function transforms."""
 
     def __init__(self, enopt_config: EnOptConfig, transform_index: int) -> None:
         """Initialize the function transform object.
 
         Args:
             enopt_config:    The configuration of the optimizer
@@ -66,7 +68,21 @@
             functions: The functions for each realization
             gradient:  The gradient for each realization
             weights:   The weight of each realization
 
         Returns:
             The expected gradients.
         """
+
+
+class FunctionTranformPluginProtocol(PluginProtocol, Protocol):
+    """The function transform plugin protocol."""
+
+    def create(
+        self, enopt_config: EnOptConfig, transform_index: int
+    ) -> FunctionTransformProtocol:
+        """Initialize the function transform object.
+
+        Args:
+            enopt_config:    The configuration of the optimizer
+            transform_index: The index of the transform to use
+        """
```

### Comparing `ropt-0.2.1/src/ropt/plugins/optimization_steps/_utils.py` & `ropt-0.3.0/src/ropt/plugins/optimization_steps/_utils.py`

 * *Files identical despite different names*

### Comparing `ropt-0.2.1/src/ropt/plugins/optimization_steps/default.py` & `ropt-0.3.0/src/ropt/plugins/optimization_steps/default.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 """This module implements the default optimization step plugin."""
 
-from typing import Any, Set
+from typing import Any, Dict
 
-from ropt.config.plan import StepConfig
 from ropt.exceptions import ConfigError
 from ropt.optimization import Plan, PlanContext
 
 from .enopt_config import DefaultEnOptConfigStep
 from .evaluator import DefaultEvaluatorStep
 from .label import DefaultLabelStep
 from .optimizer import DefaultOptimizerStep
+from .protocol import OptimizationStepsPluginProtocol, OptimizationStepsProtocol
 from .reset_tracker import DefaultResetTrackerStep
 from .restart import DefaultRestartStep
 from .tracker import DefaultTrackerStep
 from .update_config import DefaultUpdateConfigStep
 
 _FACTORIES = {
     "reset_tracker": DefaultResetTrackerStep,
@@ -23,36 +23,63 @@
     "tracker": DefaultTrackerStep,
     "restart": DefaultRestartStep,
     "optimizer": DefaultOptimizerStep,
     "evaluator": DefaultEvaluatorStep,
 }
 
 
-def get_step(config: StepConfig, context: PlanContext, plan: Plan) -> Any:  # noqa: ANN401
-    """Create a step object.
+class DefaultOptimizationSteps(OptimizationStepsProtocol):
+    """Default plugin for optimization steps."""
 
-    Args:
-        config:  The generic optimization step configuration
-        context: The context of the optimization plan execution
-        plan:    The plan that requires the step
-    """
-    assert config.model_extra is not None
-    keys = set(config.model_extra.keys())
-    if len(keys) > 1:
-        msg = f"Step type is ambiguous: {keys}"
-        raise ConfigError(msg)
-
-    for key, factory in _FACTORIES.items():
-        if key in keys:
-            return factory(config.model_extra[key], context, plan)
-
-    msg = f"Unknown step type: {keys.pop()}"
-    raise TypeError(msg)
-
-
-def get_default_steps() -> Set[str]:
-    """Return the default step types.
-
-    Returns:
-        A set of supported step type names.
-    """
-    return set(_FACTORIES.keys())
+    def __init__(self, context: PlanContext, plan: Plan) -> None:
+        """Create a default optimization step plugin.
+
+        Args:
+            context: The context of the running plan.
+            plan:    The current plan.
+        """
+        self._context = context
+        self._plan = plan
+
+    def get_step(self, config: Dict[str, Any]) -> Any:  # noqa: ANN401
+        """Get a step object.
+
+        Args:
+            config:  The generic optimization step configuration
+            context: The context of the optimization plan execution
+            plan:    The plan that requires the step
+        """
+        keys = set(config.keys())
+        if len(keys) > 1:
+            msg = f"Step type is ambiguous: {keys}"
+            raise ConfigError(msg)
+        key = keys.pop()
+
+        _, _, step_name = key.lower().rpartition("/")
+        factory = _FACTORIES.get(step_name)
+        if factory is not None:
+            return factory(config[key], self._context, self._plan)
+
+        msg = f"Unknown step type: {key}"
+        raise TypeError(msg)
+
+
+class DefaultOptimizationStepsPlugin(OptimizationStepsPluginProtocol):
+    """Default filter transform plugin class."""
+
+    def create(self, context: PlanContext, plan: Plan) -> DefaultOptimizationSteps:
+        """Initialize the realization filter plugin.
+
+        See the [ropt.plugins.optimization_steps.protocol.OptimizationStepsPlugin][] protocol.
+
+        # noqa
+        """
+        return DefaultOptimizationSteps(context, plan)
+
+    def is_supported(self, method: str) -> bool:
+        """Check if a method is supported.
+
+        See the [ropt.plugins.protocol.Plugin][] protocol.
+
+        # noqa
+        """
+        return method.lower() in _FACTORIES
```

### Comparing `ropt-0.2.1/src/ropt/plugins/optimization_steps/enopt_config.py` & `ropt-0.3.0/src/ropt/plugins/optimization_steps/enopt_config.py`

 * *Files identical despite different names*

### Comparing `ropt-0.2.1/src/ropt/plugins/optimization_steps/evaluator.py` & `ropt-0.3.0/src/ropt/plugins/optimization_steps/evaluator.py`

 * *Files identical despite different names*

### Comparing `ropt-0.2.1/src/ropt/plugins/optimization_steps/label.py` & `ropt-0.3.0/src/ropt/plugins/optimization_steps/label.py`

 * *Files identical despite different names*

### Comparing `ropt-0.2.1/src/ropt/plugins/optimization_steps/optimizer.py` & `ropt-0.3.0/src/ropt/plugins/optimization_steps/optimizer.py`

 * *Files identical despite different names*

### Comparing `ropt-0.2.1/src/ropt/plugins/optimization_steps/reset_tracker.py` & `ropt-0.3.0/src/ropt/plugins/optimization_steps/reset_tracker.py`

 * *Files identical despite different names*

### Comparing `ropt-0.2.1/src/ropt/plugins/optimization_steps/restart.py` & `ropt-0.3.0/src/ropt/plugins/optimization_steps/restart.py`

 * *Files identical despite different names*

### Comparing `ropt-0.2.1/src/ropt/plugins/optimization_steps/tracker.py` & `ropt-0.3.0/src/ropt/plugins/optimization_steps/tracker.py`

 * *Files identical despite different names*

### Comparing `ropt-0.2.1/src/ropt/plugins/optimization_steps/update_config.py` & `ropt-0.3.0/src/ropt/plugins/optimization_steps/update_config.py`

 * *Files identical despite different names*

### Comparing `ropt-0.2.1/src/ropt/plugins/optimizer/__init__.py` & `ropt-0.3.0/src/ropt/plugins/optimizer/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-"""Plugin functionality for adding optimization backends.
+"""Plugin functionality for adding optimization plugins.
 
 Optimization plugins are managed by a
 [`PluginManager`][ropt.plugins.PluginManager] object, which returns classes or
 factory functions to create objects that implement one or more optimization
-algorithms. These objects must adhere to the
-[`Optimizer`][ropt.plugins.optimizer.protocol.Optimizer] protocol. This protocol
-allows `ropt` to provide the optimizer with the callback used for evaluating
-functions and gradients and allows it to be started from an optimizer step in
-the optimization workflow.
+methods. These objects must adhere to the
+[`Optimizer`][ropt.plugins.optimizer.protocol.OptimizerProtocol] protocol. This
+protocol allows `ropt` to provide the optimizer with the callback used for
+evaluating functions and gradients and allows it to be started from an optimizer
+step in the optimization workflow.
 
 To support the implementation of the optimizer classes, the
 [`ropt.plugins.optimizer.utils`][ropt.plugins.optimizer.utils] module provides
 some utilities.
 
 Optimizers can be added via the plugin manager, by default the
-[`SciPyOptimizer`][ropt.plugins.optimizer.scipy.SciPyOptimizer] backend is
-installed which provides a number of algorithms from the
+[`SciPyOptimizer`][ropt.plugins.optimizer.scipy.SciPyOptimizer] plugin is
+installed which provides a number of methods from the
 [`scipy.optimize`](https://docs.scipy.org/doc/scipy/tutorial/optimize.html)
 package.
 """
```

### Comparing `ropt-0.2.1/src/ropt/plugins/optimizer/protocol.py` & `ropt-0.3.0/src/ropt/plugins/optimizer/protocol.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,34 +1,36 @@
-"""This module defines the protocol to be followed by optimization backends.
+"""This module defines the protocol to be followed by optimization plugins.
 
-Optimization backends can be added via the plugin mechanism to implement
-additional optimization algorithms. Any object that follows the
-[`Optimizer`][ropt.plugins.optimizer.protocol.Optimizer]
+Optimization plugins can be added via the plugin mechanism to implement
+additional optimization methods. Any object that follows the
+[`Optimizer`][ropt.plugins.optimizer.protocol.OptimizerProtocol]
 protocol may be installed as a plugin.
 """
 
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Protocol, Tuple
 
+from ropt.plugins.protocol import PluginProtocol
+
 if TYPE_CHECKING:
     import numpy as np
     from numpy.typing import NDArray
 
     from ropt.config.enopt import EnOptConfig
 
 
 class OptimizerCallback(Protocol):
     """Protocol for the optimizer callback.
 
     Optimization plugins implement optimizer classes according to the
-    [`Optimizer`][ropt.plugins.optimizer.protocol.Optimizer] protocol. Objects
-    of these classes are initialized with a callback function that follows the
-    call signature defined here. This callback should be used to request the
-    function and gradient evaluations that the optimizer needs.
+    [`Optimizer`][ropt.plugins.optimizer.protocol.OptimizerProtocol] protocol.
+    Objects of these classes are initialized with a callback function that
+    follows the call signature defined here. This callback should be used to
+    request the function and gradient evaluations that the optimizer needs.
     """
 
     def __call__(
         self,
         variables: NDArray[np.float64],
         /,
         *,
@@ -37,16 +39,16 @@
         allow_nan: bool = False,
     ) -> Tuple[NDArray[np.float64], NDArray[np.float64]]:
         """The signature of the optimizer callback.
 
         The optimizer callback expects a vector or matrix with variables to
         evaluate. Discrete optimizers may request function evaluations for
         multiple variable vectors, passed as the rows of a matrix.
-        Gradient-based algorithms may currently only pass a single variable
-        vector at a time.
+        Gradient-based methods may currently only pass a single variable vector
+        at a time.
 
         The `return_functions` and `return_gradients` flags determine whether
         functions and/or gradients are to be evaluated. The results are returned
         as a tuple of arrays, one for functions and constraints, the other for
         gradients. If one of `return_functions` or `return_gradients` is
         `False`, the corresponding result is an empty array.
 
@@ -74,15 +76,15 @@
             allow_nan:        If `True`, accept `NaN` values
 
         Returns:
             A tuple with function and gradient values.
         """
 
 
-class Optimizer(Protocol):
+class OptimizerProtocol(Protocol):
     """Protocol for optimizer classes.
 
     `ropt` employs plugins to implement optimizers that are called during an
     optimization workflow. Optimizers should adhere to the `Optimizer` protocol,
     which specifies the requirements for the class constructor (`__init__`) and
     also includes a `start` method used to initiate the optimization process.
     """
@@ -115,7 +117,21 @@
     @property
     def allow_nan(self) -> bool:
         """Return `True` if a `NaN` is a valid function value.
 
         Returns:
             `True` if `NaN` is allowed.
         """
+
+
+class OptimizerPluginProtocol(PluginProtocol, Protocol):
+    """Optimizer plugin protocol."""
+
+    def create(
+        self, config: EnOptConfig, optimizer_callback: OptimizerCallback
+    ) -> OptimizerProtocol:
+        """Create an optimizer.
+
+        Args:
+            config:             The optimizer configuration to used
+            optimizer_callback: The optimizer callback
+        """
```

### Comparing `ropt-0.2.1/src/ropt/plugins/optimizer/scipy.py` & `ropt-0.3.0/src/ropt/plugins/optimizer/scipy.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,20 +33,34 @@
 from ropt.enums import ConstraintType, VariableType
 from ropt.plugins.optimizer.utils import (
     create_output_path,
     filter_linear_constraints,
     validate_supported_constraints,
 )
 
-from .protocol import OptimizerCallback
+from .protocol import OptimizerCallback, OptimizerPluginProtocol, OptimizerProtocol
 
-# Default algorithm:
-_DEFAULT_ALGORITHM = "slsqp"
+_SUPPORTED_METHODS: Set[str] = {
+    name.lower()
+    for name in (
+        "Nelder-Mead",
+        "Powell",
+        "CG",
+        "BFGS",
+        "Newton-CG",
+        "L-BFGS-B",
+        "TNC",
+        "COBYLA",
+        "SLSQP",
+        "differential_evolution",
+    )
+}
 
-# Categorize the algorithms by the types of constraint they support or require.
+
+# Categorize the methods by the types of constraint they support or require.
 
 _CONSTRAINT_REQUIRES_BOUNDS = {
     "differential_evolution",
 }
 _CONSTRAINT_SUPPORT_BOUNDS = {
     name.lower()
     for name in [
@@ -67,33 +81,31 @@
 _CONSTRAINT_SUPPORT_NONLINEAR_EQ = {
     name.lower() for name in ["SLSQP", "differential_evolution"]
 }
 _CONSTRAINT_SUPPORT_NONLINEAR_INEQ = {
     name.lower() for name in ["COBYLA", "SLSQP", "differential_evolution"]
 }
 
-_SUPPORTS_PARALLELIZATION = {name.lower() for name in ["differential_evolution"]}
-
-# These algorithms do not use a gradient:
+# These methods do not use a gradient:
 _NO_GRADIENT = {
     name.lower()
     for name in ["Nelder-Mead", "Powell", "COBYLA", "differential_evolution"]
 }
 
 _OUTPUT_FILE = "optimizer_output"
 
 _ConstraintType = Union[
     str,
     Callable[..., float],
     Callable[..., NDArray[np.float64]],
 ]
 
 
-class SciPyOptimizer:
-    """Backend class for optimization via SciPy.
+class SciPyOptimizer(OptimizerProtocol):
+    """Plugin class for optimization via SciPy.
 
     This class implements several optimizers provided by SciPy in the
     [`scipy.optimize`](https://docs.scipy.org/doc/scipy/tutorial/optimize.html)
     package:
 
     - Nelder-Mead
     - Powell
@@ -102,18 +114,18 @@
     - Newton-CG
     - L-BFGS-B
     - TNC
     - COBYLA
     - SLSQP
     - differential_evolution
 
-    The optimizer to use is selected by setting the `algorithm` field in the
+    The optimizer to use is selected by setting the `method` field in the
     [`optimizer`][ropt.config.enopt.OptimizerConfig] field of
     [`EnOptConfig`][ropt.config.enopt.EnOptConfig] to the name of the algorithm.
-    Most of these algorithms support the general options set in the
+    Most of these methods support the general options set in the
     [`EnOptConfig`][ropt.config.enopt.EnOptConfig] object. However, specific
     options that are normally passed as arguments in the SciPy functions can be
     provided via the `options` dictionary in the configuration object. Consult
     the
     [`scipy.optimize`](https://docs.scipy.org/doc/scipy/tutorial/optimize.html)
     manual for details on these options.
 
@@ -129,30 +141,14 @@
         - The Nelder-Mead algorithm only supports bound constraints if SciPy
           version >= 1.7.
         - Some SciPy algorithms that require a Hessian or a Hessian-vector
           product are not supported. These include dogleg, trust-ncg,
           trust-exact, and trust-krylov.
     """
 
-    SUPPORTED_ALGORITHMS: ClassVar[Set[str]] = {
-        name.lower()
-        for name in (
-            "Nelder-Mead",
-            "Powell",
-            "CG",
-            "BFGS",
-            "Newton-CG",
-            "L-BFGS-B",
-            "TNC",
-            "COBYLA",
-            "SLSQP",
-            "differential_evolution",
-        )
-    }
-
     _supported_constraints: ClassVar[Dict[str, Set[str]]] = {
         "bounds": _CONSTRAINT_SUPPORT_BOUNDS,
         "linear:eq": _CONSTRAINT_SUPPORT_LINEAR_EQ,
         "linear:ineq": _CONSTRAINT_SUPPORT_LINEAR_INEQ,
         "nonlinear:eq": _CONSTRAINT_SUPPORT_NONLINEAR_EQ,
         "nonlinear:ineq": _CONSTRAINT_SUPPORT_NONLINEAR_INEQ,
     }
@@ -161,45 +157,40 @@
     }
 
     def __init__(
         self, config: EnOptConfig, optimizer_callback: OptimizerCallback
     ) -> None:
         """Initialize the optimizer implemented by the SciPy plugin.
 
-        See the [ropt.plugins.optimizer.protocol.Optimizer][] protocol.
+        See the [ropt.plugins.optimizer.protocol.OptimizerProtocol][] protocol.
 
         # noqa
         """
         self._optimizer_callback = optimizer_callback
         self._config = config
-        backend = self._config.optimizer.backend
-        if self._config.optimizer.algorithm is None:
-            self._algorithm = _DEFAULT_ALGORITHM
-        else:
-            self._algorithm = self._config.optimizer.algorithm.lower()
-        if (
-            self._algorithm is not None
-            and self._algorithm not in self.SUPPORTED_ALGORITHMS
-        ):
-            msg = f"{backend} optimizer method {self._algorithm} is not supported"
+        _, _, self._method = self._config.optimizer.method.lower().rpartition("/")
+        if self._method == "default":
+            self._method = "slsqp"
+        if self._method not in _SUPPORTED_METHODS:
+            msg = f"SciPy optimizer algorithm {self._method} is not supported"
             raise NotImplementedError(msg)
         validate_supported_constraints(
             self._config,
-            self._algorithm,
+            self._method,
             self._supported_constraints,
             self._required_constraints,
         )
         self._bounds = self._initialize_bounds()
 
         self._constraints: Union[
             Tuple[LinearConstraint, ...],
             List[Dict[str, _ConstraintType]],
         ]
 
-        if self._algorithm == "differential_evolution":
+        if self._method == "differential_evolution":
             self._constraints = (
                 self._initialize_linear_constraint_object()
                 + self._initialize_nonlinear_constraint_object()
             )
         else:
             self._constraints = (
                 self._initialize_linear_constraints()
@@ -211,15 +202,15 @@
         self._cached_function: Optional[NDArray[np.float64]] = None
         self._cached_gradient: Optional[NDArray[np.float64]] = None
         self._stdout: TextIO
 
     def start(self, initial_values: NDArray[np.float64]) -> None:
         """Start the optimization.
 
-        See the [ropt.plugins.optimizer.protocol.Optimizer][] protocol.
+        See the [ropt.plugins.optimizer.protocol.OptimizerProtocol][] protocol.
 
         # noqa
         """
         self._cached_variables = None
         self._cached_function = None
         self._cached_gradient = None
         self._parallel = False
@@ -235,15 +226,15 @@
         else:
             output_file = create_output_path(_OUTPUT_FILE, output_dir, suffix=".txt")
 
         self._stdout = sys.stdout
         with Path(output_file).open("a", encoding="utf-8") as output, redirect_stdout(
             output,
         ):
-            if self._algorithm == "differential_evolution":
+            if self._method == "differential_evolution":
                 if self._config.optimizer.parallel:
                     self._options["updating"] = "deferred"
                     self._options["workers"] = 1
                     self._parallel = True
                 differential_evolution(
                     func=self._function,
                     x0=initial_values,
@@ -254,30 +245,30 @@
                     **self._options,
                 )
             else:
                 minimize(
                     fun=self._function,
                     x0=initial_values,
                     tol=self._config.optimizer.tolerance,
-                    method=self._algorithm,
+                    method=self._method,
                     bounds=self._bounds,
-                    jac=(False if self._algorithm in _NO_GRADIENT else self._gradient),
+                    jac=(False if self._method in _NO_GRADIENT else self._gradient),
                     constraints=self._constraints,
                     options=self._options if self._options else None,
                 )
 
     @property
     def allow_nan(self) -> bool:
         """Whether NaN is allowed.
 
-        See the [ropt.plugins.optimizer.protocol.Optimizer][] protocol.
+        See the [ropt.plugins.optimizer.protocol.OptimizerProtocol][] protocol.
 
         # noqa
         """
-        return self._algorithm == "differential_evolution"
+        return self._method == "differential_evolution"
 
     def _initialize_bounds(self) -> Optional[Bounds]:
         if (
             np.isfinite(self._config.variables.lower_bounds).any()
             or np.isfinite(self._config.variables.upper_bounds).any()
         ):
             lower_bounds = self._config.variables.lower_bounds
@@ -376,15 +367,15 @@
 
         if self._config.nonlinear_constraints is None:
             return constraints
 
         for inx, constraint_type in enumerate(self._config.nonlinear_constraints.types):
             constr = "eq" if constraint_type == ConstraintType.EQ else "ineq"
             fun = partial(self._constraint_function, index=inx)
-            if self._algorithm == "cobyla":
+            if self._method == "cobyla":
                 constraints.append({"type": constr, "fun": fun})
             else:
                 jac = partial(self._constraint_gradient, index=inx)
                 constraints.append({"type": constr, "fun": fun, "jac": jac})
         return constraints
 
     def _initialize_nonlinear_constraint_object(
@@ -464,15 +455,15 @@
 
     def _get_function_or_gradient(
         self, variables: NDArray[np.float64], *, get_function: bool, get_gradient: bool
     ) -> Tuple[Optional[NDArray[np.float64]], Optional[NDArray[np.float64]]]:
         if self._parallel and variables.ndim > 1:
             variables = variables.T
 
-        if self._algorithm in _NO_GRADIENT:
+        if self._method in _NO_GRADIENT:
             get_gradient = False
 
         if (
             self._cached_variables is None
             or variables.shape != self._cached_variables.shape
             or not np.allclose(variables, self._cached_variables)
         ):
@@ -549,25 +540,49 @@
             return {}
         options = copy.deepcopy(self._config.optimizer.options)
         # The maximum number of iterations is passed as an option to ropt.
         # Setting maxiter directly as an entry in the options dict will also
         # work, but iterations will override it.
         iterations = self._config.optimizer.max_iterations
         if iterations is not None:
-            if self._algorithm == "tnc":
+            if self._method == "tnc":
                 options["maxfun"] = iterations
             else:
                 options["maxiter"] = iterations
         # We switch on display if there is an output folder.
         if self._config.optimizer.output_dir is not None:
             options["disp"] = True
 
         if (
-            self._algorithm == "differential_evolution"
+            self._method == "differential_evolution"
             and self._config.variables.types is not None
             and "integrality" not in options
         ):
             options["integrality"] = (
                 self._config.variables.types == VariableType.INTEGER
             )
 
         return options
+
+
+class SciPyOptimizerPlugin(OptimizerPluginProtocol):
+    """Default filter transform plugin class."""
+
+    def create(
+        self, config: EnOptConfig, optimizer_callback: OptimizerCallback
+    ) -> SciPyOptimizer:
+        """Initialize the optimizer plugin.
+
+        See the [ropt.plugins.optimizer.protocol.OptimizerPluginProtocol][] protocol.
+
+        # noqa
+        """
+        return SciPyOptimizer(config, optimizer_callback)
+
+    def is_supported(self, method: str) -> bool:
+        """Check if a method is supported.
+
+        See the [ropt.plugins.protocol.PluginProtocol][] protocol.
+
+        # noqa
+        """
+        return method.lower() in (_SUPPORTED_METHODS | {"default"})
```

### Comparing `ropt-0.2.1/src/ropt/plugins/optimizer/utils.py` & `ropt-0.3.0/src/ropt/plugins/optimizer/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Utility functions for use by optimization backend.
+"""Utility functions for use by optimizer plugins.
 
 This module provides utility functions to validate supported constraints, filter
 linear constraints, and to retrieve the list of supported optimizers.
 """
 
 from pathlib import Path
 from typing import Dict, Optional, Set
@@ -55,155 +55,149 @@
     "nonlinear:eq": "non-linear equality constraints",
     "nonlinear:ineq": "non-linear inequality constraints",
 }
 
 
 def validate_supported_constraints(
     config: EnOptConfig,
-    algorithm: str,
+    method: str,
     supported_constraints: Dict[str, Set[str]],
     required_constraints: Dict[str, Set[str]],
 ) -> None:
     """Check if the requested optimization features are supported or required.
 
     The keys of the supported_constraints and required_constraints dicts specify
     the type of the constraint as shown in the example below. The values are
-    sets of algorithm names that support or require the type of constraint
+    sets of method names that support or require the type of constraint
     specified by the key.
 
     For example:
     {
         "bounds": {"L-BFGS-B", "TNC", "SLSQP"},
         "linear:eq": {"SLSQP"},
         "linear:ineq": {"SLSQP"},
         "nonlinear:eq": {"SLSQP"},
         "nonlinear:ineq": {"SLSQP"},
     }
 
     Args:
         config:                The ensemble optimizer configuration object
-        algorithm:             The algorithm to check
+        method:                The method to check
         supported_constraints: Specify the supported constraints
         required_constraints:  Specify the required constraints
     """
-    _validate_bounds(config, algorithm, supported_constraints, required_constraints)
+    _validate_bounds(config, method, supported_constraints, required_constraints)
     _validate_linear_constraints(
-        config, algorithm, supported_constraints, required_constraints
+        config, method, supported_constraints, required_constraints
     )
     _validate_nonlinear_constraints(
-        config, algorithm, supported_constraints, required_constraints
+        config, method, supported_constraints, required_constraints
     )
 
 
-def _check_constraint(  # noqa: PLR0913
+def _check_constraint(
     constraint_type: str,
-    algorithm: str,
-    optimizer_name: str,
+    method: str,
     supported_constraints: Dict[str, Set[str]],
     required_constraints: Dict[str, Set[str]],
     *,
     have_constraint: bool,
 ) -> None:
     supported = {
         algo.lower() for algo in supported_constraints.get(constraint_type, set())
     }
     required = {
         algo.lower() for algo in required_constraints.get(constraint_type, set())
     }
     msg = _MESSAGES[constraint_type]
-    if have_constraint and algorithm.lower() not in supported:
-        msg = f"{optimizer_name} optimizer {algorithm} does not support {msg}"
+    if have_constraint and method.lower() not in supported:
+        msg = f"optimizer {method} does not support {msg}"
         raise NotImplementedError(msg)
-    if not have_constraint and algorithm.lower() in required:
-        msg = f"{optimizer_name} optimizer {algorithm} requires {msg}"
+    if not have_constraint and method.lower() in required:
+        msg = f"optimizer {method} requires {msg}"
         raise NotImplementedError(msg)
 
 
 def _validate_bounds(
     config: EnOptConfig,
-    algorithm: str,
+    method: str,
     supported_constraints: Dict[str, Set[str]],
     required_constraints: Dict[str, Set[str]],
 ) -> None:
     _check_constraint(
         "bounds",
-        algorithm,
-        config.optimizer.backend,
+        method,
         supported_constraints,
         required_constraints,
         have_constraint=bool(
             np.isfinite(config.variables.lower_bounds).any()
             or np.isfinite(config.variables.upper_bounds).any(),
         ),
     )
 
 
 def _validate_linear_constraints(
     config: EnOptConfig,
-    algorithm: str,
+    method: str,
     supported_constraints: Dict[str, Set[str]],
     required_constraints: Dict[str, Set[str]],
 ) -> None:
     linear_constraints = config.linear_constraints
     if linear_constraints is None:
         return
 
     if config.variables.indices is not None:
         linear_constraints = filter_linear_constraints(
             linear_constraints, config.variables.indices
         )
 
     _check_constraint(
         "linear:ineq",
-        algorithm,
-        config.optimizer.backend,
+        method,
         supported_constraints,
         required_constraints,
         have_constraint=bool(
             np.any(linear_constraints.types == ConstraintType.LE)
             or np.any(linear_constraints.types == ConstraintType.GE),
         ),
     )
 
     _check_constraint(
         "linear:eq",
-        algorithm,
-        config.optimizer.backend,
+        method,
         supported_constraints,
         required_constraints,
         have_constraint=bool(np.any(linear_constraints.types == ConstraintType.EQ)),
     )
 
 
 def _validate_nonlinear_constraints(
     config: EnOptConfig,
-    algorithm: str,
+    method: str,
     supported_constraints: Dict[str, Set[str]],
     required_constraints: Dict[str, Set[str]],
 ) -> None:
     nonlinear_constraints = config.nonlinear_constraints
     if nonlinear_constraints is None:
         return
 
     _check_constraint(
         "nonlinear:ineq",
-        algorithm,
-        config.optimizer.backend,
+        method,
         supported_constraints,
         required_constraints,
         have_constraint=bool(
             np.any(nonlinear_constraints.types == ConstraintType.LE)
             or np.any(nonlinear_constraints.types == ConstraintType.GE),
         ),
     )
 
     _check_constraint(
         "nonlinear:eq",
-        algorithm,
-        config.optimizer.backend,
+        method,
         supported_constraints,
         required_constraints,
         have_constraint=bool(
             np.any(nonlinear_constraints.types == ConstraintType.EQ),
         ),
     )
```

### Comparing `ropt-0.2.1/src/ropt/plugins/realization_filter/__init__.py` & `ropt-0.3.0/src/ropt/plugins/realization_filter/__init__.py`

 * *Files identical despite different names*

### Comparing `ropt-0.2.1/src/ropt/plugins/realization_filter/default.py` & `ropt-0.3.0/src/ropt/plugins/realization_filter/default.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 from numpy.typing import NDArray
 from pydantic import BaseModel, ConfigDict, Field, NonNegativeInt, StrictStr
 
 from ropt.config.enopt import EnOptConfig
 from ropt.enums import ConstraintType, OptimizerExitCode
 from ropt.exceptions import ConfigError, OptimizationAborted
 
+from .protocol import RealizationFilterPluginProtocol, RealizationFilterProtocol
+
 if sys.version_info >= (3, 9):
     from typing import Annotated
 else:
     from typing_extensions import Annotated
 
 
 class _ConfigBaseModel(BaseModel):
@@ -108,18 +110,18 @@
         percentile: The CVaR percentile
     """
 
     sort: Union[StrictStr, NonNegativeInt]
     percentile: Annotated[float, Field(gt=0.0, le=1.0)] = 0.5
 
 
-class DefaultRealizationFilter:
-    """The default realization filter backend class.
+class DefaultRealizationFilter(RealizationFilterProtocol):
+    """The default realization filter plugin class.
 
-    This backend currently implements four methods:
+    This plugin currently implements four methods:
 
     `sort-objective`:
     :  Filter realizations by selecting a range of objective values. This filter
        requires additional configuration using an options dict that can be
        parsed into a
        [`SortObjectiveOptions`][ropt.plugins.realization_filter.default.SortObjectiveOptions]
        class. This method sorts realizations according to the weighted sum of
@@ -156,81 +158,77 @@
        number of selected realizations is not an integer number.
     """
 
     def __init__(self, enopt_config: EnOptConfig, filter_index: int) -> None:  # D107
         """Initialize the realization filter plugin.
 
         See the
-        [ropt.plugins.realization_filter.protocol.RealizationFilter][]
+        [ropt.plugins.realization_filter.protocol.RealizationFilterProtocol][]
         protocol.
 
         # noqa
         """
         self._filter_config = enopt_config.realization_filters[filter_index]
         self._enopt_config = enopt_config
         self._filter_options: Union[
             SortObjectiveOptions,
             SortConstraintOptions,
             CVaRObjectiveOptions,
             CVaRConstraintOptions,
         ]
 
-        method = self._filter_config.method.lower()
+        _, _, self._method = self._filter_config.method.lower().rpartition("/")
         options = self._filter_config.options
         if enopt_config.objective_functions.weights.size > 1 and np.any(
             enopt_config.objective_functions.auto_scale
         ):
             msg = (
-                f"{method} does not support auto-scaling for "
+                f"{self._method} does not support auto-scaling for "
                 "multi-objective optimization"
             )
             raise ConfigError(msg)
 
-        if method == "sort-objective":
+        if self._method == "sort-objective":
             self._filter_options = SortObjectiveOptions.model_validate(options)
             self._check_range(self._filter_options)
-        elif method == "sort-constraint":
+        elif self._method == "sort-constraint":
             self._filter_options = SortConstraintOptions.model_validate(options)
             self._check_range(self._filter_options)
-        elif method == "cvar-objective":
+        elif self._method == "cvar-objective":
             self._filter_options = CVaRObjectiveOptions.model_validate(options)
-        elif method == "cvar-constraint":
+        elif self._method == "cvar-constraint":
             self._filter_options = CVaRConstraintOptions.model_validate(options)
         else:
-            msg = f"Realization filter not supported: {method}"
+            msg = f"Realization filter not supported: {self._method}"
             raise ConfigError(msg)
 
     def get_realization_weights(  # D107
         self,
         objectives: NDArray[np.float64],
         constraints: Optional[NDArray[np.float64]],
     ) -> NDArray[np.float64]:
         """Return the updated weights of the realizations.
 
         See the
-        [ropt.plugins.realization_filter.protocol.RealizationFilter][]
+        [ropt.plugins.realization_filter.protocol.RealizationFilterProtocol][]
         protocol.
 
         # noqa
         """
         weights = self._enopt_config.realizations.weights
-        if self._filter_config.method == "sort-objective":
+        if self._method == "sort-objective":
             weights = self._sort_objectives(objectives)
-        elif (
-            self._filter_config.method == "sort-constraint" and constraints is not None
-        ):
+        elif self._method == "sort-constraint" and constraints is not None:
             weights = self._sort_constraint(constraints)
-        elif self._filter_config.method == "cvar-objective":
+        elif self._method == "cvar-objective":
             weights = self._cvar_objectives(objectives)
-        elif (
-            self._filter_config.method == "cvar-constraint" and constraints is not None
-        ):
+        elif self._method == "cvar-constraint" and constraints is not None:
             weights = self._cvar_constraint(constraints)
         else:
-            msg = f"Realization filter not supported: {self._filter_config.method}"
+            msg = f"Realization filter not supported: {self._method}"
             raise ConfigError(msg)
 
         if not np.any(weights > 0):
             raise OptimizationAborted(exit_code=OptimizerExitCode.TOO_FEW_REALIZATIONS)
 
         return weights
 
@@ -378,7 +376,36 @@
         raise ValueError(msg) from exc
 
 
 def _get_indices(
     items: List[Union[str, int]], names: Optional[Tuple[str, ...]]
 ) -> Tuple[int, ...]:
     return tuple(_get_index(item, names) for item in items)
+
+
+class DefaultRealizationFilterPlugin(RealizationFilterPluginProtocol):
+    """Default realization filter plugin class."""
+
+    def create(
+        self, enopt_config: EnOptConfig, filter_index: int
+    ) -> DefaultRealizationFilter:
+        """Initialize the realization filter plugin.
+
+        See the [ropt.plugins.realization_filter.protocol.RealizationFilterPlugin][] protocol.
+
+        # noqa
+        """
+        return DefaultRealizationFilter(enopt_config, filter_index)
+
+    def is_supported(self, method: str) -> bool:
+        """Check if a method is supported.
+
+        See the [ropt.plugins.protocol.Plugin][] protocol.
+
+        # noqa
+        """
+        return method.lower() in {
+            "sort-objective",
+            "sort-constraint",
+            "cvar-objective",
+            "cvar-constraint",
+        }
```

### Comparing `ropt-0.2.1/src/ropt/plugins/realization_filter/protocol.py` & `ropt-0.3.0/src/ropt/plugins/realization_filter/protocol.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 """This module defines the protocol to be followed by realization filters.
 
 Realization filters can be added via the plugin mechanism to implement
 additional ways to filter the realizations that are used to calculate functions
 and gradients. Any object that follows the
-[`RealizationFilter`][ropt.plugins.realization_filter.protocol.RealizationFilter]
+[`RealizationFilter`][ropt.plugins.realization_filter.protocol.RealizationFilterProtocol]
 protocol may be installed as a plugin.
 """
 
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Optional, Protocol
 
+from ropt.plugins.protocol import PluginProtocol
+
 if TYPE_CHECKING:
     import numpy as np
     from numpy.typing import NDArray
 
     from ropt.config.enopt import EnOptConfig
 
 
-class RealizationFilter(Protocol):
+class RealizationFilterProtocol(Protocol):
     """Protocol for realization filter classes."""
 
     def __init__(self, enopt_config: EnOptConfig, filter_index: int) -> None:  # D107
         """Initialize the realization filter plugin.
 
         Args:
             enopt_config:    The configuration of the optimizer
@@ -52,7 +54,21 @@
         Args:
             objectives:  The objectives of all realizations
             constraints: The constraints for all realizations
 
         Returns:
             A vector of weights of the realizations.
         """
+
+
+class RealizationFilterPluginProtocol(PluginProtocol, Protocol):
+    """RealizationFilter plugin protocol."""
+
+    def create(
+        self, enopt_config: EnOptConfig, filter_index: int
+    ) -> RealizationFilterProtocol:
+        """Initialize the realization filter plugin.
+
+        Args:
+            enopt_config: The configuration of the optimizer
+            filter_index: The index of the transform to use
+        """
```

### Comparing `ropt-0.2.1/src/ropt/plugins/sampler/__init__.py` & `ropt-0.3.0/src/ropt/plugins/sampler/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,13 @@
-"""Plugin functionality for adding sampler backends.
+"""Plugin functionality for adding sampler plugins.
 
-Sampler plugins are managed by a
-[`PluginManager`][ropt.plugins.PluginManager] object, which returns classes or
-factory functions to create objects that implement one or more sampling
-algorithms to produce perturbations. These objects must adhere to the
-[`Sampler`][ropt.plugins.sampler.protocol.Sampler] protocol.
+Sampler plugins are managed by a [`PluginManager`][ropt.plugins.PluginManager]
+object, which returns classes or factory functions to create objects that
+implement one or more sampling methods to produce perturbations. These objects
+must adhere to the [`Sampler`][ropt.plugins.sampler.protocol.SamplerProtocol]
+protocol.
 
 Samplers can be added via the plugin manager, by default the
-[`SciPySampler`][ropt.plugins.sampler.scipy.SciPySampler] backend is
-installed which provides a number of algorithms from the
-[`scipy.stats`](https://docs.scipy.org/doc/scipy/reference/stats.html)
-package.
+[`SciPySampler`][ropt.plugins.sampler.scipy.SciPySampler] plugin is installed
+which provides a number of methods from the
+[`scipy.stats`](https://docs.scipy.org/doc/scipy/reference/stats.html) package.
 """
```

### Comparing `ropt-0.2.1/src/ropt/plugins/sampler/scipy.py` & `ropt-0.3.0/src/ropt/plugins/sampler/scipy.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,38 +1,42 @@
 """This module implements the SciPy sampler plugin."""
 
 import copy
 import warnings
-from typing import Any, ClassVar, Dict, Optional, Set, Tuple, Union
+from typing import Any, Dict, Optional, Set, Tuple, Union
 
 import numpy as np
 from numpy.random import Generator
 from numpy.typing import NDArray
 from scipy.stats import norm, rv_continuous, truncnorm, uniform
 from scipy.stats.qmc import Halton, LatinHypercube, QMCEngine, Sobol, scale
 
 from ropt.config.enopt import EnOptConfig
 
+from .protocol import SamplerPluginProtocol, SamplerProtocol
+
 _STATS_SAMPLERS: Dict[str, Any] = {
     "uniform": uniform,
     "norm": norm,
     "truncnorm": truncnorm,
 }
 
 _QMC_ENGINES = {
     "sobol": Sobol,
     "halton": Halton,
     "lhs": LatinHypercube,
 }
 
+_SUPPORTED_METHODS: Set[str] = set(_STATS_SAMPLERS.keys()) | set(_QMC_ENGINES.keys())
+
 
-class SciPySampler:
-    """Backend class for producing sampling values via SciPy.
+class SciPySampler(SamplerProtocol):
+    """Plugin class for producing sampling values via SciPy.
 
-    This backend implements the following sampling methods using the
+    This plugin implements the following sampling methods using the
     corresponding methods from the SciPy stats module:
 
     - Sampling from [probability
       distributions](https://docs.scipy.org/doc/scipy/reference/stats.html):
 
         `uniform`
         : Uniform distribution with a default range of [-1, 1].
@@ -59,55 +63,45 @@
     Specific options that are normally passed as arguments in the SciPy
     functions can be provided via the options dictionary in the configuration
     object. Consult the
     [`scipy.stats`](https://docs.scipy.org/doc/scipy/reference/stats.html)
     manual for details on these options.
     """
 
-    SUPPORTED_METHODS: ClassVar[Set[str]] = {
-        "uniform",
-        "norm",
-        "truncnorm",
-        "sobol",
-        "halton",
-        "lhs",
-    }
-
     def __init__(
         self,
         enopt_config: EnOptConfig,
         sampler_index: int,
         variable_indices: Optional[NDArray[np.intc]],
         rng: Generator,
     ) -> None:
         """Initialize the sampler object.
 
-        See the [ropt.plugins.sampler.protocol.Sampler][] protocol.
+        See the [ropt.plugins.sampler.protocol.SamplerProtocol][] protocol.
 
         # noqa
         """
         self._enopt_config = enopt_config
         self._sampler_config = enopt_config.samplers[sampler_index]
         self._variable_indices = variable_indices
-        if self._sampler_config.method is None:
+        _, _, self._method = self._sampler_config.method.lower().rpartition("/")
+        if self._method == "default":
             self._method = "norm"
-        else:
-            self._method = self._sampler_config.method.lower()
         self._rng = rng
         self._sampler: Union[rv_continuous, QMCEngine]
         self._options: Dict[str, Any]
-        if self._method not in self.SUPPORTED_METHODS:
-            msg = f"Method '{self._method}' is not implemented by the SciPy backend"
+        if self._method not in _SUPPORTED_METHODS:
+            msg = f"Method '{self._method}' is not implemented by the SciPy plugin"
             raise NotImplementedError(msg)
         self._sampler, self._options = self._init_sampler(self._sampler_config.options)
 
     def generate_samples(self) -> NDArray[np.float64]:
         """Generate a set of samples.
 
-        See the [ropt.plugins.sampler.protocol.Sampler][] protocol.
+        See the [ropt.plugins.sampler.protocol.SamplerProtocol][] protocol.
 
         # noqa
         """
         variable_count = self._enopt_config.variables.initial_values.size
         realization_count = self._enopt_config.realizations.weights.size
         perturbation_count = self._enopt_config.gradient.number_of_perturbations
 
@@ -193,7 +187,35 @@
 
         if self._method == "sobol":
             with warnings.catch_warnings():
                 warnings.simplefilter("ignore")
                 return _run_qmc_engine()
         else:
             return _run_qmc_engine()
+
+
+class SciPySamplerPlugin(SamplerPluginProtocol):
+    """Default sampler plugin class."""
+
+    def create(
+        self,
+        enopt_config: EnOptConfig,
+        sampler_index: int,
+        variable_indices: Optional[NDArray[np.intc]],
+        rng: Generator,
+    ) -> SciPySampler:
+        """Initialize the sampler plugin.
+
+        See the [ropt.plugins.sampler.protocol.SamplerPlugin][] protocol.
+
+        # noqa
+        """
+        return SciPySampler(enopt_config, sampler_index, variable_indices, rng)
+
+    def is_supported(self, method: str) -> bool:
+        """Check if a method is supported.
+
+        See the [ropt.plugins.protocol.Plugin][] protocol.
+
+        # noqa
+        """
+        return method.lower() in (_SUPPORTED_METHODS | {"default"})
```

### Comparing `ropt-0.2.1/src/ropt/report/__init__.py` & `ropt-0.3.0/src/ropt/report/__init__.py`

 * *Files identical despite different names*

### Comparing `ropt-0.2.1/src/ropt/report/_data_frame.py` & `ropt-0.3.0/src/ropt/report/_data_frame.py`

 * *Files identical despite different names*

### Comparing `ropt-0.2.1/src/ropt/report/_table.py` & `ropt-0.3.0/src/ropt/report/_table.py`

 * *Files identical despite different names*

### Comparing `ropt-0.2.1/src/ropt/report/_utils.py` & `ropt-0.3.0/src/ropt/report/_utils.py`

 * *Files identical despite different names*

### Comparing `ropt-0.2.1/src/ropt/results/__init__.py` & `ropt-0.3.0/src/ropt/results/__init__.py`

 * *Files identical despite different names*

### Comparing `ropt-0.2.1/src/ropt/results/_bound_constraints.py` & `ropt-0.3.0/src/ropt/results/_bound_constraints.py`

 * *Files identical despite different names*

### Comparing `ropt-0.2.1/src/ropt/results/_function_evaluations.py` & `ropt-0.3.0/src/ropt/results/_function_evaluations.py`

 * *Files identical despite different names*

### Comparing `ropt-0.2.1/src/ropt/results/_function_results.py` & `ropt-0.3.0/src/ropt/results/_function_results.py`

 * *Files identical despite different names*

### Comparing `ropt-0.2.1/src/ropt/results/_functions.py` & `ropt-0.3.0/src/ropt/results/_functions.py`

 * *Files identical despite different names*

### Comparing `ropt-0.2.1/src/ropt/results/_gradient_evaluations.py` & `ropt-0.3.0/src/ropt/results/_gradient_evaluations.py`

 * *Files identical despite different names*

### Comparing `ropt-0.2.1/src/ropt/results/_gradient_results.py` & `ropt-0.3.0/src/ropt/results/_gradient_results.py`

 * *Files identical despite different names*

### Comparing `ropt-0.2.1/src/ropt/results/_gradients.py` & `ropt-0.3.0/src/ropt/results/_gradients.py`

 * *Files identical despite different names*

### Comparing `ropt-0.2.1/src/ropt/results/_linear_constraints.py` & `ropt-0.3.0/src/ropt/results/_linear_constraints.py`

 * *Files identical despite different names*

### Comparing `ropt-0.2.1/src/ropt/results/_maximize.py` & `ropt-0.3.0/src/ropt/results/_maximize.py`

 * *Files identical despite different names*

### Comparing `ropt-0.2.1/src/ropt/results/_nonlinear_constraints.py` & `ropt-0.3.0/src/ropt/results/_nonlinear_constraints.py`

 * *Files identical despite different names*

### Comparing `ropt-0.2.1/src/ropt/results/_pandas.py` & `ropt-0.3.0/src/ropt/results/_pandas.py`

 * *Files identical despite different names*

### Comparing `ropt-0.2.1/src/ropt/results/_realizations.py` & `ropt-0.3.0/src/ropt/results/_realizations.py`

 * *Files identical despite different names*

### Comparing `ropt-0.2.1/src/ropt/results/_result_field.py` & `ropt-0.3.0/src/ropt/results/_result_field.py`

 * *Files identical despite different names*

### Comparing `ropt-0.2.1/src/ropt/results/_results.py` & `ropt-0.3.0/src/ropt/results/_results.py`

 * *Files identical despite different names*

### Comparing `ropt-0.2.1/src/ropt/results/_utils.py` & `ropt-0.3.0/src/ropt/results/_utils.py`

 * *Files identical despite different names*

### Comparing `ropt-0.2.1/src/ropt/results/_xarray.py` & `ropt-0.3.0/src/ropt/results/_xarray.py`

 * *Files identical despite different names*

### Comparing `ropt-0.2.1/src/ropt/utils/_misc.py` & `ropt-0.3.0/src/ropt/utils/_misc.py`

 * *Files identical despite different names*

### Comparing `ropt-0.2.1/src/ropt/utils/scaling.py` & `ropt-0.3.0/src/ropt/utils/scaling.py`

 * *Files identical despite different names*

### Comparing `ropt-0.2.1/src/ropt.egg-info/PKG-INFO` & `ropt-0.3.0/src/ropt.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ropt
-Version: 0.2.1
+Version: 0.3.0
 Summary: The ropt ensemble optimizer module
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -50,16 +50,17 @@
 Detailed documentation and examples can be found in the online
 [manual](https://tno-ropt.github.io/ropt/).
 
 
 ## Dependencies
 `ropt` has been tested with Python versions 3.8-3.12.
 
-`ropt` requires one or more optimization backends to function. A backend based
-on optimizers included with [SciPy](https://scipy.org/) is installed by default.
+`ropt` requires one or more optimization plugins to function. By default, a
+plugin based on optimizers included with [SciPy](https://scipy.org/) is
+installed.
 
 
 ## Installation
 From PyPI:
 ```bash
 pip install ropt
 ```
```

### Comparing `ropt-0.2.1/src/ropt.egg-info/SOURCES.txt` & `ropt-0.3.0/src/ropt.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -12,21 +12,21 @@
 docs/reference/enopt_config.md
 docs/reference/enums.md
 docs/reference/evaluator.md
 docs/reference/exceptions.md
 docs/reference/function_transforms.md
 docs/reference/optimization.md
 docs/reference/optimization_steps.md
-docs/reference/optimizer_backends.md
+docs/reference/optimizer_plugins.md
 docs/reference/plan_config.md
 docs/reference/plugins.md
 docs/reference/realization_filters.md
 docs/reference/reporting.md
 docs/reference/results.md
-docs/reference/sampler_backends.md
+docs/reference/sampler_plugins.md
 docs/reference/utilities.md
 docs/usage/robust_optimization.md
 docs/usage/running.md
 examples/de_linear.py
 examples/de_nonlinear.py
 examples/rosenbrock_deterministic.py
 examples/rosenbrock_ensemble.py
@@ -37,14 +37,15 @@
 src/ropt/events.py
 src/ropt/exceptions.py
 src/ropt/py.typed
 src/ropt/version.py
 src/ropt.egg-info/PKG-INFO
 src/ropt.egg-info/SOURCES.txt
 src/ropt.egg-info/dependency_links.txt
+src/ropt.egg-info/entry_points.txt
 src/ropt.egg-info/requires.txt
 src/ropt.egg-info/top_level.txt
 src/ropt/apps/__init__.py
 src/ropt/apps/_script_optimizer.py
 src/ropt/config/__init__.py
 src/ropt/config/utils.py
 src/ropt/config/enopt/__init__.py
@@ -61,15 +62,14 @@
 src/ropt/config/enopt/_sampler_config.py
 src/ropt/config/enopt/_utils.py
 src/ropt/config/enopt/_variables_config.py
 src/ropt/config/enopt/constants.py
 src/ropt/config/plan/__init__.py
 src/ropt/config/plan/_config.py
 src/ropt/config/plan/_plan_config.py
-src/ropt/config/plan/_step_config.py
 src/ropt/evaluator/__init__.py
 src/ropt/evaluator/_concurrent.py
 src/ropt/evaluator/_ensemble_evaluator.py
 src/ropt/evaluator/_evaluator.py
 src/ropt/evaluator/_evaluator_results.py
 src/ropt/evaluator/_function.py
 src/ropt/evaluator/_gradient.py
@@ -79,24 +79,26 @@
 src/ropt/optimization/_bases.py
 src/ropt/optimization/_ensemble_optimizer.py
 src/ropt/optimization/_events.py
 src/ropt/optimization/_optimizer.py
 src/ropt/optimization/_plan.py
 src/ropt/plugins/__init__.py
 src/ropt/plugins/_manager.py
+src/ropt/plugins/protocol.py
 src/ropt/plugins/function_transform/__init__.py
 src/ropt/plugins/function_transform/default.py
 src/ropt/plugins/function_transform/protocol.py
 src/ropt/plugins/optimization_steps/__init__.py
 src/ropt/plugins/optimization_steps/_utils.py
 src/ropt/plugins/optimization_steps/default.py
 src/ropt/plugins/optimization_steps/enopt_config.py
 src/ropt/plugins/optimization_steps/evaluator.py
 src/ropt/plugins/optimization_steps/label.py
 src/ropt/plugins/optimization_steps/optimizer.py
+src/ropt/plugins/optimization_steps/protocol.py
 src/ropt/plugins/optimization_steps/reset_tracker.py
 src/ropt/plugins/optimization_steps/restart.py
 src/ropt/plugins/optimization_steps/tracker.py
 src/ropt/plugins/optimization_steps/update_config.py
 src/ropt/plugins/optimizer/__init__.py
 src/ropt/plugins/optimizer/protocol.py
 src/ropt/plugins/optimizer/scipy.py
@@ -144,10 +146,10 @@
 tests/test_pandas.py
 tests/test_parsl.py
 tests/test_realization_filters.py
 tests/test_result_table.py
 tests/test_results.py
 tests/test_results_data_frame.py
 tests/test_samplers.py
-tests/test_scipy_backend.py
+tests/test_scipy_optimizers.py
 tests/test_scipy_samplers.py
 tests/test_xarray.py
```

### Comparing `ropt-0.2.1/tests/conftest.py` & `ropt-0.3.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ropt-0.2.1/tests/test_concurrent.py` & `ropt-0.3.0/tests/test_concurrent.py`

 * *Files 24% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 @pytest.fixture(name="enopt_config")
 def enopt_config_fixture() -> Dict[str, Any]:
     return {
         "variables": {
             "initial_values": [0.0, 0.0, 0.1],
         },
         "optimizer": {
-            "algorithm": "slsqp",
             "tolerance": 1e-5,
         },
         "objective_functions": {
             "weights": [0.75, 0.25],
         },
         "realizations": {
             "weights": [1.0] * 3,
@@ -55,46 +54,51 @@
         return cast(NDArray[np.float64], self.future.result())
 
 
 class ConcurrentTestEvaluator(ConcurrentEvaluator):
     def __init__(
         self, functions: Tuple[Callable[..., Any], ...], fail_index: int = -1
     ) -> None:
-        super().__init__()
+        super().__init__(enable_cache=True)
 
         self._executor = ThreadPoolExecutor(max_workers=4)
         self._functions = functions
         self._fail_index = fail_index
         self._tasks: Dict[int, ConcurrentTask]
         self.polling = 0.0
 
     def launch(
         self,
         batch_id: int,  # noqa: ARG002
         variables: NDArray[np.float64],
         context: EvaluatorContext,  # noqa: ARG002
+        active: Optional[NDArray[np.bool_]],
     ) -> Dict[int, ConcurrentTask]:
         self._tasks = {
             idx: TaskTestEvaluator(
                 future=self._executor.submit(
                     _run_functions,
                     self._functions,
                     variables[idx, :],
                     self._fail_index == idx,
                 ),
             )
             for idx in range(variables.shape[0])
+            if active is None or active[idx]
         }
         return self._tasks
 
     def monitor(self) -> None:
         for idx, task in self._tasks.items():
             if task.future.exception() is not None:
                 print(f"error in evaluation {idx}")  # noqa: T201
 
+    def disable_functions(self) -> None:
+        self._functions = (lambda _0, _1: 0.0, lambda _0, _1: 0.0)
+
 
 def test_concurrent(enopt_config: Any, test_functions: Any) -> None:
     evaluator = ConcurrentTestEvaluator(test_functions)
     optimizer = EnsembleOptimizer(evaluator)
     results = optimizer.start_optimization(
         plan=[
             {"config": enopt_config},
@@ -118,7 +122,38 @@
             {"tracker": {"id": "optimum", "source": "opt"}},
         ],
     )
     assert results is not None
     assert np.allclose(results.evaluations.variables, [0.0, 0.0, 0.5], atol=0.02)
     captured = capsys.readouterr()
     assert "error in evaluation 2" in captured.out
+
+
+def test_concurrent_cache(enopt_config: Any, test_functions: Any) -> None:
+    evaluator = ConcurrentTestEvaluator(test_functions)
+
+    optimizer = EnsembleOptimizer(evaluator)
+    results1 = optimizer.start_optimization(
+        plan=[
+            {"config": enopt_config},
+            {"optimizer": {"id": "opt"}},
+            {"tracker": {"id": "optimum", "source": "opt"}},
+        ],
+    )
+    assert results1 is not None
+    assert np.allclose(results1.evaluations.variables, [0.0, 0.0, 0.5], atol=0.02)
+
+    # Disable the functions, not the evaluator fully relies on its cache:
+    evaluator.disable_functions()
+
+    optimizer = EnsembleOptimizer(evaluator)
+    results2 = optimizer.start_optimization(
+        plan=[
+            {"config": enopt_config},
+            {"optimizer": {"id": "opt"}},
+            {"tracker": {"id": "optimum", "source": "opt"}},
+        ],
+    )
+    assert results2 is not None
+    assert np.all(
+        np.equal(results1.evaluations.variables, results2.evaluations.variables)
+    )
```

### Comparing `ropt-0.2.1/tests/test_config.py` & `ropt-0.3.0/tests/test_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,16 +22,15 @@
         "variables": {
             "initial_values": np.array([1, 2]),
         },
         "objective_functions": {
             "weights": [1.0],
         },
         "optimizer": {
-            "backend": "test",
-            "algorithm": "dummy",
+            "method": "dummy",
         },
     }
 
 
 def test_check_variable_names() -> None:
     config = {"names": ["a", "b"], "initial_values": np.array([1, 2])}
     variables = VariablesConfig.model_validate(config)
```

### Comparing `ropt-0.2.1/tests/test_ensemble_gradient.py` & `ropt-0.3.0/tests/test_ensemble_gradient.py`

 * *Files 1% similar despite different names*

```diff
@@ -258,15 +258,15 @@
     ]
 
     config_dict = {
         "variables": {
             "initial_values": [0.0] * len(variables),
             "lower_bounds": 0.0,
         },
-        "optimizer": {"backend": "test", "algorithm": "opt"},
+        "optimizer": {"method": "opt"},
         "objective_functions": {"weights": [1.0]},
         "gradient": {"number_of_perturbations": 10, "perturbation_magnitudes": 0.05},
     }
 
     config = EnOptConfig.model_validate(config_dict)
     sampler = SciPySampler(config, 0, None, default_rng(123))
     perturbations = _perturb_variables(
```

### Comparing `ropt-0.2.1/tests/test_examples.py` & `ropt-0.3.0/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `ropt-0.2.1/tests/test_failed_realizations.py` & `ropt-0.3.0/tests/test_failed_realizations.py`

 * *Files identical despite different names*

### Comparing `ropt-0.2.1/tests/test_function_transforms.py` & `ropt-0.3.0/tests/test_function_transforms.py`

 * *Files identical despite different names*

### Comparing `ropt-0.2.1/tests/test_netcdf.py` & `ropt-0.3.0/tests/test_netcdf.py`

 * *Files identical despite different names*

### Comparing `ropt-0.2.1/tests/test_optimizer.py` & `ropt-0.3.0/tests/test_optimizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,39 @@
+from __future__ import annotations
+
 from copy import deepcopy
 from functools import partial
-from typing import Any, Dict, List, Optional, Tuple, cast
+from typing import TYPE_CHECKING, Any, Dict, List, Optional, Tuple, cast
 
 import numpy as np
 import pytest
 from numpy.typing import NDArray
 
 from ropt.config.enopt import EnOptConfig
 from ropt.config.enopt.constants import DEFAULT_SEED
-from ropt.config.plan import StepConfig
 from ropt.enums import ConstraintType, EventType, OptimizerExitCode
-from ropt.events import OptimizationEvent
 from ropt.exceptions import ConfigError
 from ropt.optimization import EnsembleOptimizer, Plan, PlanContext
 from ropt.plugins import PluginManager
 from ropt.plugins.optimization_steps.evaluator import DefaultEvaluatorStep
+from ropt.plugins.optimization_steps.protocol import (
+    OptimizationStepsPluginProtocol,
+    OptimizationStepsProtocol,
+)
 from ropt.report import ResultsDataFrame
 from ropt.results import FunctionResults, GradientResults
 
+if TYPE_CHECKING:
+    from ropt.events import OptimizationEvent
+
 
 @pytest.fixture(name="enopt_config")
 def enopt_config_fixture() -> Dict[str, Any]:
     return {
         "optimizer": {
-            "algorithm": "slsqp",
             "tolerance": 1e-5,
             "max_functions": 20,
         },
         "variables": {
             "initial_values": [0.0, 0.0, 0.1],
         },
         "objective_functions": {
@@ -607,15 +613,14 @@
     enopt_config["variables"]["initial_values"] = [0.0, 0.2, 0.1]
 
     opt_config1 = {
         "speculative": True,
         "max_functions": 4,
     }
     opt_config2 = {
-        "algorithm": "slsqp",
         "speculative": True,
         "max_functions": 3,
     }
 
     enopt_config1 = deepcopy(enopt_config)
     enopt_config1["variables"]["indices"] = [0, 2]
     enopt_config1["optimizer"] = opt_config1
@@ -702,15 +707,15 @@
     assert results is not None
     assert np.allclose(results.evaluations.variables, [0.0, 0.0, 0.5], atol=0.02)
     assert completed_functions == 25
 
 
 def test_parallelize(enopt_config: Any, evaluator: Any) -> None:
     enopt_config["optimizer"] = {
-        "algorithm": "differential_evolution",
+        "method": "differential_evolution",
         "max_iterations": 10,
         "options": {"seed": 123, "tol": 1e-10},
     }
     enopt_config["variables"]["lower_bounds"] = [0.15, 0.0, 0.0]
     enopt_config["variables"]["upper_bounds"] = [0.5, 0.5, 0.2]
     enopt_config["variables"]["initial_values"][0] = 0.2
 
@@ -1035,32 +1040,50 @@
             {"restart": {"max_restarts": 1}},
         ]
     )
 
     assert reporter.frame["metadata.restart"].to_list() == 3 * [0] + 3 * [1]
 
 
-class ModifyConfig:
+class ModifyConfigStep:
     def __init__(
         self,
-        _0: StepConfig,
+        _0: Dict[str, Any],
         _1: PlanContext,
         plan: Plan,
         weights: NDArray[np.float64],
     ) -> None:
         self._plan = plan
         self._weights = weights
 
     def run(self, _: Optional[NDArray[np.float64]]) -> bool:
         self._plan.update_enopt_config(
             {"objective_functions": {"weights": self._weights}}
         )
         return False
 
 
+class ModifyConfig(OptimizationStepsProtocol):
+    def __init__(self, context: PlanContext, plan: Plan) -> None:
+        self._context = context
+        self._plan = plan
+
+    def get_step(self, config: Dict[str, Any]) -> Any:
+        weights = config["modify"]["weights"]
+        return ModifyConfigStep(config, self._context, self._plan, weights)
+
+
+class ModifyConfigPlugin(OptimizationStepsPluginProtocol):
+    def create(self, context: PlanContext, plan: Plan) -> ModifyConfig:
+        return ModifyConfig(context, plan)
+
+    def is_supported(self, method: str) -> bool:
+        return method in {"modify"}
+
+
 def test_modify_enopt_in_plan(enopt_config: Any, evaluator: Any) -> None:
     weights = enopt_config["objective_functions"]["weights"]
     enopt_config["objective_functions"]["weights"] = [1, 1]
     optimizer = EnsembleOptimizer(evaluator())
     results = optimizer.start_optimization(
         plan=[
             {"config": enopt_config},
@@ -1068,103 +1091,113 @@
             {"tracker": {"id": "optimum", "source": "opt"}},
         ],
     )
     assert results is not None
     assert not np.allclose(results.evaluations.variables, [0.0, 0.0, 0.5], atol=0.02)
 
     plugin_manager = PluginManager()
-    plugin_manager.add_backends(
+    plugin_manager.add_plugins(
         "optimization_step",
-        {
-            "modify_backend": lambda config, context, plan: ModifyConfig(
-                config, context, plan, weights
-            )
-        },
+        {"modify_plugin": ModifyConfigPlugin()},
     )
 
     optimizer = EnsembleOptimizer(evaluator(), plugin_manager=plugin_manager)
     results = optimizer.start_optimization(
         plan=[
             {"config": enopt_config},
-            {"backend": "modify_backend", "type": "default"},
+            {"modify": {"weights": weights}},
             {"optimizer": {"id": "opt"}},
             {"tracker": {"id": "optimum", "source": "opt"}},
         ],
     )
     assert results is not None
     assert np.allclose(results.evaluations.variables, [0.0, 0.0, 0.5], atol=0.02)
 
 
-class EvaluatorWithProcess(DefaultEvaluatorStep):
+class EvaluatorWithProcessStep(DefaultEvaluatorStep):
     def __init__(
         self,
         config: Dict[str, Any],
         context: PlanContext,
         plan: Plan,
-        completed: List[FunctionResults],
     ) -> None:
         super().__init__(config, context, plan)
-        self._completed = completed
+        self._completed = config["completed"]
 
     def process(self, results: FunctionResults) -> None:
         self._completed.append(results)
 
 
-@pytest.mark.parametrize("backend", ["default", "evaluator_backend"])
+class EvaluatorWithProcess((OptimizationStepsProtocol)):
+    def __init__(self, context: PlanContext, plan: Plan) -> None:
+        self._context = context
+        self._plan = plan
+
+    def get_step(self, config: Dict[str, Any]) -> Any:
+        return EvaluatorWithProcessStep(
+            config["evaluator_with_process"], self._context, self._plan
+        )
+
+
+class EvaluatorWithProcessPlugin(OptimizationStepsPluginProtocol):
+    def create(self, context: PlanContext, plan: Plan) -> EvaluatorWithProcess:
+        return EvaluatorWithProcess(context, plan)
+
+    def is_supported(self, _: str) -> bool:
+        return True
+
+
+@pytest.mark.parametrize("method", ["evaluator", "evaluator_with_process"])
 @pytest.mark.parametrize("init_from", [None, "last", "optimum"])
 def test_evaluator_step(
-    enopt_config: Any, evaluator: Any, init_from: str, backend: str
+    enopt_config: Any, evaluator: Any, init_from: str, method: str
 ) -> None:
     completed: List[FunctionResults] = []
 
     def _track_evaluations(event: OptimizationEvent) -> None:
         assert event.results is not None
         nonlocal completed
         completed += [
             item for item in event.results if isinstance(item, FunctionResults)
         ]
 
     enopt_config["optimizer"]["speculative"] = True
     enopt_config["optimizer"]["max_functions"] = 4
 
     plugin_manager = PluginManager()
-    if backend == "evaluator_backend":
-        plugin_manager.add_backends(
+    if method == "evaluator_with_process":
+        plugin_manager.add_plugins(
             "optimization_step",
-            {
-                "evaluator_backend": lambda config, context, plan: EvaluatorWithProcess(
-                    config.model_extra["evaluator"], context, plan, completed
-                )
-            },
+            {"evaluator_plugin": EvaluatorWithProcessPlugin()},
         )
 
     optimizer = EnsembleOptimizer(evaluator(), plugin_manager=plugin_manager)
     optimizer.add_observer(EventType.FINISHED_EVALUATION, _track_evaluations)
-    if backend == "default":
+    if method == "evaluator":
         optimizer.add_observer(EventType.FINISHED_EVALUATOR_STEP, _track_evaluations)
 
     plan = [
         {"config": enopt_config},
         {"optimizer": {"id": "opt"}},
     ]
     if init_from is None:
-        plan.append({"backend": backend, "evaluator": {}})
+        plan.append({method: {"completed": completed}})
     elif init_from == "last":
         plan.extend(
             [
                 {"tracker": {"id": "last", "source": "opt", "type": "last_result"}},
                 {"update_config": {"initial_variables": "last"}},
-                {"backend": backend, "evaluator": {}},
+                {method: {"completed": completed}},
             ]
         )
     else:
         plan.extend(
             [
                 {"update_config": {"initial_variables": "optimum"}},
-                {"backend": backend, "evaluator": {}},
+                {method: {"completed": completed}},
             ]
         )
     plan.append({"tracker": {"id": "optimum", "source": "opt"}})
     results = optimizer.start_optimization(plan=plan)
 
     from_map = {None: 0, "last": 3, "optimum": 2}
```

### Comparing `ropt-0.2.1/tests/test_pandas.py` & `ropt-0.3.0/tests/test_pandas.py`

 * *Files identical despite different names*

### Comparing `ropt-0.2.1/tests/test_parsl.py` & `ropt-0.3.0/tests/test_parsl.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,15 +28,14 @@
 @pytest.fixture(name="enopt_config")
 def enopt_config_fixture() -> Dict[str, Any]:
     return {
         "variables": {
             "initial_values": [0.0, 0.0, 0.1],
         },
         "optimizer": {
-            "algorithm": "slsqp",
             "max_functions": 3,
         },
         "objective_functions": {
             "weights": [0.75, 0.25],
         },
         "realizations": {
             "weights": [1.0] * 3,
```

### Comparing `ropt-0.2.1/tests/test_realization_filters.py` & `ropt-0.3.0/tests/test_realization_filters.py`

 * *Files identical despite different names*

### Comparing `ropt-0.2.1/tests/test_result_table.py` & `ropt-0.3.0/tests/test_result_table.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 pd = pytest.importorskip("pandas")
 
 
 @pytest.fixture(name="enopt_config")
 def enopt_config_fixture() -> Dict[str, Any]:
     return {
         "optimizer": {
-            "algorithm": "slsqp",
             "tolerance": 1e-5,
             "speculative": True,
             "max_functions": 3,
         },
         "variables": {
             "initial_values": [0.0, 0.0, 0.1],
             "upper_bounds": 1.0,
```

### Comparing `ropt-0.2.1/tests/test_results.py` & `ropt-0.3.0/tests/test_results.py`

 * *Files identical despite different names*

### Comparing `ropt-0.2.1/tests/test_results_data_frame.py` & `ropt-0.3.0/tests/test_results_data_frame.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 pd = pytest.importorskip("pandas")
 
 
 @pytest.fixture(name="enopt_config")
 def enopt_config_fixture() -> Dict[str, Any]:
     return {
         "optimizer": {
-            "algorithm": "slsqp",
             "tolerance": 1e-5,
             "speculative": True,
             "max_functions": 3,
         },
         "variables": {
             "initial_values": [0.0, 0.0, 0.1],
             "upper_bounds": 1.0,
```

### Comparing `ropt-0.2.1/tests/test_samplers.py` & `ropt-0.3.0/tests/test_samplers.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,36 +1,38 @@
+from __future__ import annotations
+
 import copy
-from typing import Any, Dict, List, Optional
+from typing import TYPE_CHECKING, Any, Dict, List, Optional
 
 import numpy as np
 import pytest
 from numpy.random import Generator, default_rng
-from numpy.typing import NDArray
 
 from ropt.config.enopt import EnOptConfig
 from ropt.evaluator._gradient import _perturb_variables
 from ropt.exceptions import ConfigError
 from ropt.optimization import EnsembleOptimizer
 from ropt.plugins import PluginManager
-from ropt.plugins.sampler.protocol import Sampler
+
+if TYPE_CHECKING:
+    from numpy.typing import NDArray
 
 
 @pytest.fixture(name="enopt_config")
 def enopt_config_fixture() -> Dict[str, Any]:
     return {
         "optimizer": {
             "tolerance": 0.005,
             "max_functions": 4,
         },
         "objective_functions": {
             "weights": [0.75, 0.24],
         },
         "samplers": [
             {
-                "backend": "mocked",
                 "method": "test",
             },
         ],
         "gradient": {
             "number_of_perturbations": 3,
             "perturbation_magnitudes": 0.01,
         },
@@ -38,15 +40,15 @@
             "initial_values": [0, 0, 0],
             "upper_bounds": 1.0,
             "lower_bounds": -1.0,
         },
     }
 
 
-class MockedSampler(Sampler):
+class MockedSampler:
     def __init__(
         self,
         enopt_config: EnOptConfig,
         sampler_index: int,
         variable_indices: Optional[NDArray[np.intc]],
         _: Generator,
     ) -> None:
@@ -80,14 +82,28 @@
             samples *= self._sampler.options["scale"]
         for idx in range(samples.shape[0]):
             diag = np.diag(samples[idx, ...])
             samples[idx, ...] = np.diag(diag)
         return samples
 
 
+class MockedSamplerPlugin:
+    def create(
+        self,
+        enopt_config: EnOptConfig,
+        sampler_index: int,
+        variable_indices: Optional[NDArray[np.intc]],
+        rng: Generator,
+    ) -> MockedSampler:
+        return MockedSampler(enopt_config, sampler_index, variable_indices, rng)
+
+    def is_supported(self, method: str) -> bool:
+        return method.lower() in {"test"}
+
+
 def test_sampler_simple(enopt_config: Any) -> None:
     enopt_config["gradient"]["number_of_perturbations"] = 3
     rng = default_rng(123)
     config = EnOptConfig.model_validate(enopt_config)
     sampler = MockedSampler(config, 0, None, rng)
 
     perturbed_variables = _perturb_variables(
@@ -172,19 +188,19 @@
         results1.evaluations.variables,
         results2.evaluations.variables,
     )
 
 
 def test_sampler_plugin(enopt_config: Any, evaluator: Any) -> None:
     optimizer = EnsembleOptimizer(evaluator())
-    with pytest.raises(ConfigError, match="Sampler backend not supported: mocked"):
+    with pytest.raises(ConfigError, match="Method not found: test"):
         optimizer.start_optimization(plan=[{"config": enopt_config}, {"optimizer": {}}])
 
     plugin_manager = PluginManager()
-    plugin_manager.add_backends("sampler", {"mocked": MockedSampler})
+    plugin_manager.add_plugins("sampler", {"mocked": MockedSamplerPlugin()})
     optimizer = EnsembleOptimizer(evaluator(), plugin_manager)
     result = optimizer.start_optimization(
         plan=[
             {"config": enopt_config},
             {"optimizer": {"id": "opt"}},
             {"tracker": {"id": "optimum", "source": "opt"}},
         ],
```

### Comparing `ropt-0.2.1/tests/test_scipy_backend.py` & `ropt-0.3.0/tests/test_scipy_optimizers.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from ropt.plugins.optimizer.scipy import (
     _CONSTRAINT_REQUIRES_BOUNDS,
     _CONSTRAINT_SUPPORT_BOUNDS,
     _CONSTRAINT_SUPPORT_LINEAR_EQ,
     _CONSTRAINT_SUPPORT_LINEAR_INEQ,
     _CONSTRAINT_SUPPORT_NONLINEAR_EQ,
     _CONSTRAINT_SUPPORT_NONLINEAR_INEQ,
-    SciPyOptimizer,
+    _SUPPORTED_METHODS,
 )
 
 
 @pytest.fixture(name="enopt_config")
 def enopt_config_fixture() -> Dict[str, Any]:
     return {
         "variables": {
@@ -35,18 +35,18 @@
         "gradient": {
             "perturbation_magnitudes": 0.01,
         },
     }
 
 
 @pytest.mark.parametrize(
-    "method", sorted(SciPyOptimizer.SUPPORTED_ALGORITHMS - _CONSTRAINT_REQUIRES_BOUNDS)
+    "method", sorted(_SUPPORTED_METHODS - _CONSTRAINT_REQUIRES_BOUNDS)
 )
 def test_scipy_unconstrained(enopt_config: Any, method: str, evaluator: Any) -> None:
-    enopt_config["optimizer"]["algorithm"] = method
+    enopt_config["optimizer"]["method"] = method
 
     optimizer = EnsembleOptimizer(evaluator())
     result = optimizer.start_optimization(
         plan=[
             {"config": enopt_config},
             {"optimizer": {"id": "opt"}},
             {"tracker": {"id": "optimum", "source": "opt"}},
@@ -55,112 +55,112 @@
     assert result is not None
     # Some methods are supported, but not reliable in this test.
     if method != "newton-cg":
         assert np.allclose(result.evaluations.variables, [0.0, 0.0, 0.5], atol=0.02)
 
 
 @pytest.mark.parametrize(
-    "method", sorted(SciPyOptimizer.SUPPORTED_ALGORITHMS - _CONSTRAINT_SUPPORT_BOUNDS)
+    "method", sorted(_SUPPORTED_METHODS - _CONSTRAINT_SUPPORT_BOUNDS)
 )
 def test_scipy_unsupported_constraints_bounds(
     enopt_config: Any, method: str, evaluator: Any
 ) -> None:
-    enopt_config["optimizer"]["algorithm"] = method
+    enopt_config["optimizer"]["method"] = method
     enopt_config["variables"]["lower_bounds"] = [0.1, -np.inf, -np.inf]
     optimizer = EnsembleOptimizer(evaluator())
     with pytest.raises(NotImplementedError, match="does not support bound constraints"):
         optimizer.start_optimization(plan=[{"config": enopt_config}, {"optimizer": {}}])
 
 
 @pytest.mark.parametrize("method", sorted(_CONSTRAINT_REQUIRES_BOUNDS))
 def test_scipy_required_constraints_bounds(
     enopt_config: Any, method: str, evaluator: Any
 ) -> None:
-    enopt_config["optimizer"]["algorithm"] = method
+    enopt_config["optimizer"]["method"] = method
     optimizer = EnsembleOptimizer(evaluator())
     with pytest.raises(NotImplementedError, match="requires bound constraints"):
         optimizer.start_optimization(plan=[{"config": enopt_config}, {"optimizer": {}}])
 
 
 @pytest.mark.parametrize(
     "method",
-    sorted(SciPyOptimizer.SUPPORTED_ALGORITHMS - _CONSTRAINT_SUPPORT_LINEAR_EQ),
+    sorted(_SUPPORTED_METHODS - _CONSTRAINT_SUPPORT_LINEAR_EQ),
 )
 def test_scipy_unsupported_constraints_linear_eq(
     enopt_config: Any, method: str, evaluator: Any
 ) -> None:
-    enopt_config["optimizer"]["algorithm"] = method
+    enopt_config["optimizer"]["method"] = method
     enopt_config["linear_constraints"] = {
         "coefficients": [[1.0, 0.0, 1.0]],
         "rhs_values": 1.0,
         "types": [ConstraintType.EQ],
     }
     optimizer = EnsembleOptimizer(evaluator())
     with pytest.raises(
         NotImplementedError, match="does not support linear equality constraints"
     ):
         optimizer.start_optimization(plan=[{"config": enopt_config}, {"optimizer": {}}])
 
 
 @pytest.mark.parametrize(
     "method",
-    sorted(SciPyOptimizer.SUPPORTED_ALGORITHMS - _CONSTRAINT_SUPPORT_LINEAR_INEQ),
+    sorted(_SUPPORTED_METHODS - _CONSTRAINT_SUPPORT_LINEAR_INEQ),
 )
 @pytest.mark.parametrize("bound_type", [ConstraintType.LE, ConstraintType.GE])
 def test_scipy_unsupported_constraints_linear_ineq(
     enopt_config: Any,
     method: str,
     bound_type: ConstraintType,
     evaluator: Any,
 ) -> None:
-    enopt_config["optimizer"]["algorithm"] = method
+    enopt_config["optimizer"]["method"] = method
     enopt_config["linear_constraints"] = {
         "coefficients": [[1.0, 0.0, 1.0]],
         "rhs_values": 0.4 if bound_type == ConstraintType.LE else -0.4,
         "types": [bound_type],
     }
     optimizer = EnsembleOptimizer(evaluator())
     with pytest.raises(
         NotImplementedError, match="does not support linear inequality constraints"
     ):
         optimizer.start_optimization(plan=[{"config": enopt_config}, {"optimizer": {}}])
 
 
 @pytest.mark.parametrize(
     "method",
-    sorted(SciPyOptimizer.SUPPORTED_ALGORITHMS - _CONSTRAINT_SUPPORT_NONLINEAR_EQ),
+    sorted(_SUPPORTED_METHODS - _CONSTRAINT_SUPPORT_NONLINEAR_EQ),
 )
 def test_scipy_unsupported_constraints_nonlinear_eq(
     enopt_config: Any, method: str, evaluator: Any
 ) -> None:
-    enopt_config["optimizer"]["algorithm"] = method
+    enopt_config["optimizer"]["method"] = method
     enopt_config["nonlinear_constraints"] = {
         "rhs_values": 1.0,
         "types": [ConstraintType.EQ],
     }
 
     optimizer = EnsembleOptimizer(evaluator())
     with pytest.raises(
         NotImplementedError, match="does not support non-linear equality constraints"
     ):
         optimizer.start_optimization(plan=[{"config": enopt_config}, {"optimizer": {}}])
 
 
 @pytest.mark.parametrize(
     "method",
-    sorted(SciPyOptimizer.SUPPORTED_ALGORITHMS - _CONSTRAINT_SUPPORT_NONLINEAR_INEQ),
+    sorted(_SUPPORTED_METHODS - _CONSTRAINT_SUPPORT_NONLINEAR_INEQ),
 )
 @pytest.mark.parametrize("bound_type", [ConstraintType.LE, ConstraintType.GE])
 def test_scipy_unsupported_constraints_nonlinear_ineq(
     enopt_config: Any,
     method: str,
     bound_type: ConstraintType,
     evaluator: Any,
 ) -> None:
-    enopt_config["optimizer"]["algorithm"] = method
+    enopt_config["optimizer"]["method"] = method
     enopt_config["nonlinear_constraints"] = {
         "rhs_values": 0.4 if bound_type == ConstraintType.LE else -0.0,
         "types": [bound_type],
     }
     optimizer = EnsembleOptimizer(evaluator())
     with pytest.raises(
         NotImplementedError, match="does not support non-linear inequality constraints"
@@ -168,15 +168,15 @@
         optimizer.start_optimization(plan=[{"config": enopt_config}, {"optimizer": {}}])
 
 
 @pytest.mark.parametrize("method", sorted(_CONSTRAINT_SUPPORT_BOUNDS))
 def test_scipy_bound_constraints(
     enopt_config: Any, method: str, evaluator: Any
 ) -> None:
-    enopt_config["optimizer"]["algorithm"] = method
+    enopt_config["optimizer"]["method"] = method
     enopt_config["variables"]["lower_bounds"] = [0.15, 0.0, 0.0]
     enopt_config["variables"]["upper_bounds"] = [0.5, 0.5, 0.2]
     enopt_config["variables"]["initial_values"][0] = 0.2
 
     if method == "differential_evolution":
         enopt_config["optimizer"]["options"] = {"seed": 123}
     optimizer = EnsembleOptimizer(evaluator())
@@ -191,15 +191,15 @@
     if method != "differential_evolution":
         assert np.allclose(result.evaluations.variables, [0.15, 0.0, 0.2], atol=0.02)
 
 
 def test_scipy_bound_constraints_differential_evolution(
     enopt_config: Any, evaluator: Any, test_functions: Any
 ) -> None:
-    enopt_config["optimizer"]["algorithm"] = "differential_evolution"
+    enopt_config["optimizer"]["method"] = "differential_evolution"
     enopt_config["variables"]["lower_bounds"] = [0.15, 0.0, 0.0]
     enopt_config["variables"]["upper_bounds"] = [0.5, 0.5, 0.2]
     enopt_config["variables"]["initial_values"][0] = 0.2
     enopt_config["optimizer"]["options"] = {"seed": 123}
     enopt_config["realizations"] = {"realization_min_success": 0}
     optimizer = EnsembleOptimizer(evaluator())
     result1 = optimizer.start_optimization(
@@ -240,15 +240,15 @@
 @pytest.mark.parametrize("method", sorted(_CONSTRAINT_SUPPORT_LINEAR_EQ))
 def test_scipy_eq_linear_constraints(
     enopt_config: Any, method: str, evaluator: Any
 ) -> None:
     if method in _CONSTRAINT_SUPPORT_BOUNDS:
         enopt_config["variables"]["lower_bounds"] = [-1.0, -1.0, -1.0]
         enopt_config["variables"]["upper_bounds"] = [1.0, 1.0, 1.0]
-    enopt_config["optimizer"]["algorithm"] = method
+    enopt_config["optimizer"]["method"] = method
     enopt_config["linear_constraints"] = {
         "coefficients": [[1, 0, 1], [0, 1, 1]],
         "rhs_values": [1.0, 0.75],
         "types": [ConstraintType.EQ, ConstraintType.EQ],
     }
 
     optimizer = EnsembleOptimizer(evaluator())
@@ -267,15 +267,15 @@
 @pytest.mark.parametrize("method", sorted(_CONSTRAINT_SUPPORT_LINEAR_INEQ))
 def test_scipy_ge_linear_constraints(
     enopt_config: Any, method: str, evaluator: Any
 ) -> None:
     if method in _CONSTRAINT_SUPPORT_BOUNDS:
         enopt_config["variables"]["lower_bounds"] = [-1.0, -1.0, -1.0]
         enopt_config["variables"]["upper_bounds"] = [1.0, 1.0, 1.0]
-    enopt_config["optimizer"]["algorithm"] = method
+    enopt_config["optimizer"]["method"] = method
     enopt_config["linear_constraints"] = {
         "coefficients": [[-1, 0, -1]],
         "rhs_values": -0.4,
         "types": [ConstraintType.GE],
     }
 
     optimizer = EnsembleOptimizer(evaluator())
@@ -294,15 +294,15 @@
 @pytest.mark.parametrize("method", sorted(_CONSTRAINT_SUPPORT_LINEAR_INEQ))
 def test_scipy_le_linear_constraints(
     enopt_config: Any, method: str, evaluator: Any
 ) -> None:
     if method in _CONSTRAINT_SUPPORT_BOUNDS:
         enopt_config["variables"]["lower_bounds"] = [-1.0, -1.0, -1.0]
         enopt_config["variables"]["upper_bounds"] = [1.0, 1.0, 1.0]
-    enopt_config["optimizer"]["algorithm"] = method
+    enopt_config["optimizer"]["method"] = method
     enopt_config["linear_constraints"] = {
         "coefficients": [[1, 0, 1]],
         "rhs_values": 0.4,
         "types": [ConstraintType.LE],
     }
 
     optimizer = EnsembleOptimizer(evaluator())
@@ -321,15 +321,15 @@
 @pytest.mark.parametrize("method", sorted(_CONSTRAINT_SUPPORT_LINEAR_INEQ))
 def test_scipy_le_ge_linear_constraints(
     enopt_config: Any, method: str, evaluator: Any
 ) -> None:
     if method in _CONSTRAINT_SUPPORT_BOUNDS:
         enopt_config["variables"]["lower_bounds"] = [-1.0, -1.0, -1.0]
         enopt_config["variables"]["upper_bounds"] = [1.0, 1.0, 1.0]
-    enopt_config["optimizer"]["algorithm"] = method
+    enopt_config["optimizer"]["method"] = method
     enopt_config["linear_constraints"] = {
         "coefficients": [[1, 0, 1], [-1, 0, -1]],
         "rhs_values": [0.4, -0.4],
         "types": [ConstraintType.LE, ConstraintType.GE],
     }
 
     optimizer = EnsembleOptimizer(evaluator())
@@ -347,15 +347,15 @@
 
 @pytest.mark.parametrize("method", sorted(_CONSTRAINT_SUPPORT_NONLINEAR_EQ))
 def test_scipy_eq_nonlinear_constraints(
     enopt_config: Any, method: str, evaluator: Any, test_functions: Any
 ) -> None:
     enopt_config["variables"]["lower_bounds"] = [-1.0, -1.0, -1.0]
     enopt_config["variables"]["upper_bounds"] = [1.0, 1.0, 1.0]
-    enopt_config["optimizer"]["algorithm"] = method
+    enopt_config["optimizer"]["method"] = method
     enopt_config["nonlinear_constraints"] = {
         "rhs_values": 1.0,
         "types": [ConstraintType.EQ],
     }
 
     test_functions = (
         *test_functions,
@@ -389,15 +389,15 @@
     bound_type: ConstraintType,
     evaluator: Any,
     test_functions: Any,
 ) -> None:
     if method in _CONSTRAINT_SUPPORT_BOUNDS:
         enopt_config["variables"]["lower_bounds"] = [-1.0, -1.0, -1.0]
         enopt_config["variables"]["upper_bounds"] = [1.0, 1.0, 1.0]
-    enopt_config["optimizer"]["algorithm"] = method
+    enopt_config["optimizer"]["method"] = method
     enopt_config["nonlinear_constraints"] = {
         "rhs_values": 0.4 if bound_type == ConstraintType.LE else -0.4,
         "types": [bound_type],
     }
 
     weight = 1.0 if bound_type == ConstraintType.LE else -1.0
     test_functions = (
@@ -429,15 +429,15 @@
 ) -> None:
     # These constraints together force the first two variables to be zero,
     # while the last one is free to fit the function.
     if method in _CONSTRAINT_SUPPORT_BOUNDS:
         enopt_config["variables"]["lower_bounds"] = [-1.0, -1.0, -1.0]
         enopt_config["variables"]["upper_bounds"] = [1.0, 1.0, 1.0]
     enopt_config["variables"]["lower_bounds"] = 0.0
-    enopt_config["optimizer"]["algorithm"] = method
+    enopt_config["optimizer"]["method"] = method
 
     enopt_config["nonlinear_constraints"] = {
         "rhs_values": [0.4, 0.0],
         "types": [ConstraintType.GE, ConstraintType.EQ],
     }
 
     test_functions = (
@@ -460,15 +460,15 @@
     # some methods are supported, but not reliable in this test.
     if method != "differential_evolution":
         assert result is not None
         assert np.allclose(result.evaluations.variables, [0.0, 0.0, 0.5], atol=0.02)
 
 
 def test_scipy_options(enopt_config: Any, evaluator: Any) -> None:
-    enopt_config["optimizer"]["algorithm"] = "Nelder-Mead"
+    enopt_config["optimizer"]["method"] = "Nelder-Mead"
     enopt_config["optimizer"]["options"] = {"maxfev": 10}
 
     optimizer = EnsembleOptimizer(evaluator())
     result = optimizer.start_optimization(
         plan=[
             {"config": enopt_config},
             {"optimizer": {"id": "opt"}},
@@ -478,20 +478,20 @@
 
     # The correct result should not be found now:
     assert result is not None
     assert pytest.approx(result.evaluations.variables[2], abs=0.025) != 0.5
 
 
 @pytest.mark.parametrize(
-    "method", sorted(SciPyOptimizer.SUPPORTED_ALGORITHMS - _CONSTRAINT_REQUIRES_BOUNDS)
+    "method", sorted(_SUPPORTED_METHODS - _CONSTRAINT_REQUIRES_BOUNDS)
 )
 def test_scipy_split_evaluations(
     enopt_config: Any, method: str, evaluator: Any
 ) -> None:
-    enopt_config["optimizer"]["algorithm"] = method
+    enopt_config["optimizer"]["method"] = method
     enopt_config["optimizer"]["split_evaluations"] = True
 
     optimizer = EnsembleOptimizer(evaluator())
     result = optimizer.start_optimization(
         plan=[
             {"config": enopt_config},
             {"optimizer": {"id": "opt"}},
@@ -499,15 +499,15 @@
         ],
     )
     assert result is not None
     # Some methods are supported, but not reliable in this test.
     if method != "newton-cg":
         assert np.allclose(result.evaluations.variables, [0.0, 0.0, 0.5], atol=0.02)
 
-    enopt_config["optimizer"]["algorithm"] = method
+    enopt_config["optimizer"]["method"] = method
     enopt_config["optimizer"]["speculative"] = True
     enopt_config["optimizer"]["split_evaluations"] = True
 
     optimizer = EnsembleOptimizer(evaluator())
     result = optimizer.start_optimization(
         plan=[
             {"config": enopt_config},
@@ -521,15 +521,15 @@
         assert np.allclose(result.evaluations.variables, [0.0, 0.0, 0.5], atol=0.02)
 
 
 @pytest.mark.parametrize("speculative", [True, False])
 def test_scipy_speculative(
     enopt_config: Any, evaluator: Any, speculative: bool
 ) -> None:
-    enopt_config["optimizer"]["algorithm"] = "slsqp"
+    enopt_config["optimizer"]["method"] = "slsqp"
     enopt_config["optimizer"]["speculative"] = speculative
 
     def _observer(event: OptimizationEvent) -> None:
         assert event.results is not None
         assert len(event.results) == 2 if speculative else 1
 
     optimizer = EnsembleOptimizer(evaluator())
@@ -545,15 +545,15 @@
     assert np.allclose(result.evaluations.variables, [0.0, 0.0, 0.5], atol=0.02)
 
 
 def test_scipy_output_dir(tmp_path: Path, enopt_config: Any, evaluator: Any) -> None:
     output_dir = tmp_path / "outputdir"
     output_dir.mkdir()
     enopt_config["optimizer"]["output_dir"] = output_dir
-    enopt_config["optimizer"]["algorithm"] = "slsqp"
+    enopt_config["optimizer"]["method"] = "slsqp"
     enopt_config["optimizer"]["max_functions"] = 1
     optimizer = EnsembleOptimizer(evaluator())
     optimizer.start_optimization(
         plan=[
             {"config": enopt_config},
             {"optimizer": {"id": "opt"}},
             {"tracker": {"id": "optimum", "source": "opt"}},
```

### Comparing `ropt-0.2.1/tests/test_scipy_samplers.py` & `ropt-0.3.0/tests/test_scipy_samplers.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 import numpy as np
 import pytest
 
 from ropt.enums import EventType
 from ropt.events import OptimizationEvent
 from ropt.optimization import EnsembleOptimizer
-from ropt.plugins.sampler.scipy import SciPySampler
+from ropt.plugins.sampler.scipy import _SUPPORTED_METHODS
 from ropt.results import GradientResults
 
 if TYPE_CHECKING:
     from numpy.typing import NDArray
 
 
 @pytest.fixture(name="enopt_config")
@@ -29,15 +29,15 @@
         },
         "gradient": {
             "perturbation_magnitudes": 0.01,
         },
     }
 
 
-@pytest.mark.parametrize("method", sorted(SciPySampler.SUPPORTED_METHODS))
+@pytest.mark.parametrize("method", sorted(_SUPPORTED_METHODS))
 def test_scipy_samplers_unconstrained(
     enopt_config: Any, method: str, evaluator: Any
 ) -> None:
     enopt_config["samplers"] = [{"method": method}]
     optimizer = EnsembleOptimizer(evaluator())
     results = optimizer.start_optimization(
         plan=[
@@ -66,15 +66,15 @@
     )
     assert result is not None
     assert pytest.approx(result.evaluations.variables[0]) != 0.0
     assert pytest.approx(result.evaluations.variables[1]) == 0.1
     assert pytest.approx(result.evaluations.variables[2]) != 0.5
 
 
-@pytest.mark.parametrize("method", sorted(SciPySampler.SUPPORTED_METHODS))
+@pytest.mark.parametrize("method", sorted(_SUPPORTED_METHODS))
 def test_scipy_samplers_shared(enopt_config: Any, method: str, evaluator: Any) -> None:
     enopt_config["realizations"] = {"weights": [1.0, 1.0]}
     enopt_config["samplers"] = [{"method": method}]
 
     perturbations: Dict[str, NDArray[np.float64]] = {}
 
     def _observer(event: OptimizationEvent, tag: str) -> None:
```

### Comparing `ropt-0.2.1/tests/test_xarray.py` & `ropt-0.3.0/tests/test_xarray.py`

 * *Files identical despite different names*

