# Comparing `tmp/blackjax-1.1.1.tar.gz` & `tmp/blackjax-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blackjax-1.1.1.tar", last modified: Wed Feb 21 10:51:07 2024, max compression
+gzip compressed data, was "blackjax-1.2.0.tar", last modified: Mon May  6 16:18:53 2024, max compression
```

## Comparing `blackjax-1.1.1.tar` & `blackjax-1.2.0.tar`

### file list

```diff
@@ -1,177 +1,177 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 10:51:07.729128 blackjax-1.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-02-21 10:50:57.000000 blackjax-1.1.1/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 10:51:07.701128 blackjax-1.1.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 10:51:07.705128 blackjax-1.1.1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)     2317 2024-02-21 10:50:57.000000 blackjax-1.1.1/.github/ISSUE_TEMPLATE/bug_report.yml
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-02-21 10:50:57.000000 blackjax-1.1.1/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (127)      753 2024-02-21 10:50:57.000000 blackjax-1.1.1/.github/ISSUE_TEMPLATE/enhancement.md
--rw-r--r--   0 runner    (1001) docker     (127)      721 2024-02-21 10:50:57.000000 blackjax-1.1.1/.github/ISSUE_TEMPLATE/meeting.md
--rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-02-21 10:50:57.000000 blackjax-1.1.1/.github/ISSUE_TEMPLATE/sampler_proposal.md
--rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-02-21 10:50:57.000000 blackjax-1.1.1/.github/PULL_REQUEST_TEMPLATE.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 10:51:07.705128 blackjax-1.1.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-02-21 10:50:57.000000 blackjax-1.1.1/.github/workflows/benchmark.yml
--rw-r--r--   0 runner    (1001) docker     (127)      542 2024-02-21 10:50:57.000000 blackjax-1.1.1/.github/workflows/build_documentation.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1615 2024-02-21 10:50:57.000000 blackjax-1.1.1/.github/workflows/nightly.yml
--rw-r--r--   0 runner    (1001) docker     (127)      785 2024-02-21 10:50:57.000000 blackjax-1.1.1/.github/workflows/publish_documentation.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1652 2024-02-21 10:50:57.000000 blackjax-1.1.1/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-02-21 10:50:57.000000 blackjax-1.1.1/.github/workflows/schedule-meeting.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-02-21 10:50:57.000000 blackjax-1.1.1/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-02-21 10:50:57.000000 blackjax-1.1.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      618 2024-02-21 10:50:57.000000 blackjax-1.1.1/.gitlint
--rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-02-21 10:50:57.000000 blackjax-1.1.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-02-21 10:50:57.000000 blackjax-1.1.1/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3381 2024-02-21 10:50:57.000000 blackjax-1.1.1/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)     2324 2024-02-21 10:50:57.000000 blackjax-1.1.1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     4371 2024-02-21 10:50:57.000000 blackjax-1.1.1/GOVERNANCE.md
--rw-r--r--   0 runner    (1001) docker     (127)    11354 2024-02-21 10:50:57.000000 blackjax-1.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-02-21 10:50:57.000000 blackjax-1.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      513 2024-02-21 10:50:57.000000 blackjax-1.1.1/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     6580 2024-02-21 10:51:07.729128 blackjax-1.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5106 2024-02-21 10:50:57.000000 blackjax-1.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 10:51:07.705128 blackjax-1.1.1/blackjax/
--rw-r--r--   0 runner    (1001) docker     (127)     2236 2024-02-21 10:50:57.000000 blackjax-1.1.1/blackjax/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-02-21 10:51:07.000000 blackjax-1.1.1/blackjax/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 10:51:07.709128 blackjax-1.1.1/blackjax/adaptation/
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-02-21 10:50:57.000000 blackjax-1.1.1/blackjax/adaptation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      847 2024-02-21 10:50:57.000000 blackjax-1.1.1/blackjax/adaptation/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    17208 2024-02-21 10:50:57.000000 blackjax-1.1.1/blackjax/adaptation/chees_adaptation.py
--rw-r--r--   0 runner    (1001) docker     (127)     7640 2024-02-21 10:50:57.000000 blackjax-1.1.1/blackjax/adaptation/mass_matrix.py
--rw-r--r--   0 runner    (1001) docker     (127)    10235 2024-02-21 10:50:57.000000 blackjax-1.1.1/blackjax/adaptation/mclmc_adaptation.py
--rw-r--r--   0 runner    (1001) docker     (127)    10582 2024-02-21 10:50:57.000000 blackjax-1.1.1/blackjax/adaptation/meads_adaptation.py
--rw-r--r--   0 runner    (1001) docker     (127)     7649 2024-02-21 10:50:57.000000 blackjax-1.1.1/blackjax/adaptation/pathfinder_adaptation.py
--rw-r--r--   0 runner    (1001) docker     (127)     9600 2024-02-21 10:50:57.000000 blackjax-1.1.1/blackjax/adaptation/step_size.py
--rw-r--r--   0 runner    (1001) docker     (127)    16488 2024-02-21 10:50:57.000000 blackjax-1.1.1/blackjax/adaptation/window_adaptation.py
--rw-r--r--   0 runner    (1001) docker     (127)     5100 2024-02-21 10:50:57.000000 blackjax-1.1.1/blackjax/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     7915 2024-02-21 10:50:57.000000 blackjax-1.1.1/blackjax/diagnostics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 10:51:07.709128 blackjax-1.1.1/blackjax/mcmc/
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-02-21 10:50:57.000000 blackjax-1.1.1/blackjax/mcmc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9062 2024-02-21 10:50:57.000000 blackjax-1.1.1/blackjax/mcmc/barker.py
--rw-r--r--   0 runner    (1001) docker     (127)     1590 2024-02-21 10:50:57.000000 blackjax-1.1.1/blackjax/mcmc/diffusions.py
--rw-r--r--   0 runner    (1001) docker     (127)     7125 2024-02-21 10:50:57.000000 blackjax-1.1.1/blackjax/mcmc/dynamic_hmc.py
--rw-r--r--   0 runner    (1001) docker     (127)     9336 2024-02-21 10:50:57.000000 blackjax-1.1.1/blackjax/mcmc/elliptical_slice.py
--rw-r--r--   0 runner    (1001) docker     (127)    10856 2024-02-21 10:50:57.000000 blackjax-1.1.1/blackjax/mcmc/ghmc.py
--rw-r--r--   0 runner    (1001) docker     (127)    11218 2024-02-21 10:50:57.000000 blackjax-1.1.1/blackjax/mcmc/hmc.py
--rw-r--r--   0 runner    (1001) docker     (127)    16461 2024-02-21 10:50:57.000000 blackjax-1.1.1/blackjax/mcmc/integrators.py
--rw-r--r--   0 runner    (1001) docker     (127)     5922 2024-02-21 10:50:57.000000 blackjax-1.1.1/blackjax/mcmc/mala.py
--rw-r--r--   0 runner    (1001) docker     (127)     8668 2024-02-21 10:50:57.000000 blackjax-1.1.1/blackjax/mcmc/marginal_latent_gaussian.py
--rw-r--r--   0 runner    (1001) docker     (127)     5902 2024-02-21 10:50:57.000000 blackjax-1.1.1/blackjax/mcmc/mclmc.py
--rw-r--r--   0 runner    (1001) docker     (127)    11000 2024-02-21 10:50:57.000000 blackjax-1.1.1/blackjax/mcmc/metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)    11258 2024-02-21 10:50:57.000000 blackjax-1.1.1/blackjax/mcmc/nuts.py
--rw-r--r--   0 runner    (1001) docker     (127)    12177 2024-02-21 10:50:57.000000 blackjax-1.1.1/blackjax/mcmc/periodic_orbital.py
--rw-r--r--   0 runner    (1001) docker     (127)     8602 2024-02-21 10:50:57.000000 blackjax-1.1.1/blackjax/mcmc/proposal.py
--rw-r--r--   0 runner    (1001) docker     (127)    16186 2024-02-21 10:50:57.000000 blackjax-1.1.1/blackjax/mcmc/random_walk.py
--rw-r--r--   0 runner    (1001) docker     (127)     3304 2024-02-21 10:50:57.000000 blackjax-1.1.1/blackjax/mcmc/rmhmc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3847 2024-02-21 10:50:57.000000 blackjax-1.1.1/blackjax/mcmc/termination.py
--rw-r--r--   0 runner    (1001) docker     (127)    22957 2024-02-21 10:50:57.000000 blackjax-1.1.1/blackjax/mcmc/trajectory.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 10:51:07.713128 blackjax-1.1.1/blackjax/optimizers/
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-02-21 10:50:57.000000 blackjax-1.1.1/blackjax/optimizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4491 2024-02-21 10:50:57.000000 blackjax-1.1.1/blackjax/optimizers/dual_averaging.py
--rw-r--r--   0 runner    (1001) docker     (127)    11581 2024-02-21 10:50:57.000000 blackjax-1.1.1/blackjax/optimizers/lbfgs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3468 2024-02-21 10:50:57.000000 blackjax-1.1.1/blackjax/progress_bar.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 10:51:07.713128 blackjax-1.1.1/blackjax/sgmcmc/
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-02-21 10:50:57.000000 blackjax-1.1.1/blackjax/sgmcmc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8932 2024-02-21 10:50:57.000000 blackjax-1.1.1/blackjax/sgmcmc/csgld.py
--rw-r--r--   0 runner    (1001) docker     (127)     3953 2024-02-21 10:50:57.000000 blackjax-1.1.1/blackjax/sgmcmc/diffusions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4376 2024-02-21 10:50:57.000000 blackjax-1.1.1/blackjax/sgmcmc/gradients.py
--rw-r--r--   0 runner    (1001) docker     (127)     4766 2024-02-21 10:50:57.000000 blackjax-1.1.1/blackjax/sgmcmc/sghmc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3907 2024-02-21 10:50:57.000000 blackjax-1.1.1/blackjax/sgmcmc/sgld.py
--rw-r--r--   0 runner    (1001) docker     (127)     4776 2024-02-21 10:50:57.000000 blackjax-1.1.1/blackjax/sgmcmc/sgnht.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 10:51:07.713128 blackjax-1.1.1/blackjax/smc/
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-02-21 10:50:57.000000 blackjax-1.1.1/blackjax/smc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5559 2024-02-21 10:50:57.000000 blackjax-1.1.1/blackjax/smc/adaptive_tempered.py
--rw-r--r--   0 runner    (1001) docker     (127)     5033 2024-02-21 10:50:57.000000 blackjax-1.1.1/blackjax/smc/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2576 2024-02-21 10:50:57.000000 blackjax-1.1.1/blackjax/smc/ess.py
--rw-r--r--   0 runner    (1001) docker     (127)     5784 2024-02-21 10:50:57.000000 blackjax-1.1.1/blackjax/smc/inner_kernel_tuning.py
--rw-r--r--   0 runner    (1001) docker     (127)     4871 2024-02-21 10:50:57.000000 blackjax-1.1.1/blackjax/smc/resampling.py
--rw-r--r--   0 runner    (1001) docker     (127)     2493 2024-02-21 10:50:57.000000 blackjax-1.1.1/blackjax/smc/solver.py
--rw-r--r--   0 runner    (1001) docker     (127)     6830 2024-02-21 10:50:57.000000 blackjax-1.1.1/blackjax/smc/tempered.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 10:51:07.713128 blackjax-1.1.1/blackjax/smc/tuning/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-21 10:50:57.000000 blackjax-1.1.1/blackjax/smc/tuning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1576 2024-02-21 10:50:57.000000 blackjax-1.1.1/blackjax/smc/tuning/from_kernel_info.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1368 2024-02-21 10:50:57.000000 blackjax-1.1.1/blackjax/smc/tuning/from_particles.py
--rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-02-21 10:50:57.000000 blackjax-1.1.1/blackjax/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     7311 2024-02-21 10:50:57.000000 blackjax-1.1.1/blackjax/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 10:51:07.717128 blackjax-1.1.1/blackjax/vi/
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-02-21 10:50:57.000000 blackjax-1.1.1/blackjax/vi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5583 2024-02-21 10:50:57.000000 blackjax-1.1.1/blackjax/vi/meanfield_vi.py
--rw-r--r--   0 runner    (1001) docker     (127)     9040 2024-02-21 10:50:57.000000 blackjax-1.1.1/blackjax/vi/pathfinder.py
--rw-r--r--   0 runner    (1001) docker     (127)     7276 2024-02-21 10:50:57.000000 blackjax-1.1.1/blackjax/vi/schrodinger_follmer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5600 2024-02-21 10:50:57.000000 blackjax-1.1.1/blackjax/vi/svgd.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 10:51:07.729128 blackjax-1.1.1/blackjax.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6580 2024-02-21 10:51:07.000000 blackjax-1.1.1/blackjax.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4227 2024-02-21 10:51:07.000000 blackjax-1.1.1/blackjax.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-21 10:51:07.000000 blackjax-1.1.1/blackjax.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-02-21 10:51:07.000000 blackjax-1.1.1/blackjax.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-02-21 10:51:07.000000 blackjax-1.1.1/blackjax.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-02-21 10:50:57.000000 blackjax-1.1.1/codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 10:51:07.717128 blackjax-1.1.1/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 10:51:07.717128 blackjax-1.1.1/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)   161829 2024-02-21 10:50:57.000000 blackjax-1.1.1/docs/_static/blackjax.png
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-02-21 10:50:57.000000 blackjax-1.1.1/docs/_static/custom.css
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-02-21 10:50:57.000000 blackjax-1.1.1/docs/bib.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4301 2024-02-21 10:50:57.000000 blackjax-1.1.1/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 10:51:07.717128 blackjax-1.1.1/docs/examples/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 10:51:07.725128 blackjax-1.1.1/docs/examples/data/
--rw-r--r--   0 runner    (1001) docker     (127)     4864 2024-02-21 10:50:57.000000 blackjax-1.1.1/docs/examples/data/blackjax.png
--rw-r--r--   0 runner    (1001) docker     (127)    63251 2024-02-21 10:50:57.000000 blackjax-1.1.1/docs/examples/data/google.csv
--rw-r--r--   0 runner    (1001) docker     (127)     6030 2024-02-21 10:50:57.000000 blackjax-1.1.1/docs/examples/howto_custom_gradients.md
--rw-r--r--   0 runner    (1001) docker     (127)    12029 2024-02-21 10:50:57.000000 blackjax-1.1.1/docs/examples/howto_metropolis_within_gibbs.md
--rw-r--r--   0 runner    (1001) docker     (127)     6164 2024-02-21 10:50:57.000000 blackjax-1.1.1/docs/examples/howto_other_frameworks.md
--rw-r--r--   0 runner    (1001) docker     (127)     5518 2024-02-21 10:50:57.000000 blackjax-1.1.1/docs/examples/howto_reproduce_the_blackjax_image.md
--rw-r--r--   0 runner    (1001) docker     (127)     9833 2024-02-21 10:50:57.000000 blackjax-1.1.1/docs/examples/howto_sample_multiple_chains.md
--rw-r--r--   0 runner    (1001) docker     (127)     6722 2024-02-21 10:50:57.000000 blackjax-1.1.1/docs/examples/howto_use_aesara.md
--rw-r--r--   0 runner    (1001) docker     (127)     5248 2024-02-21 10:50:57.000000 blackjax-1.1.1/docs/examples/howto_use_numpyro.md
--rw-r--r--   0 runner    (1001) docker     (127)     6122 2024-02-21 10:50:57.000000 blackjax-1.1.1/docs/examples/howto_use_oryx.md
--rw-r--r--   0 runner    (1001) docker     (127)     3357 2024-02-21 10:50:57.000000 blackjax-1.1.1/docs/examples/howto_use_pymc.md
--rw-r--r--   0 runner    (1001) docker     (127)     4641 2024-02-21 10:50:57.000000 blackjax-1.1.1/docs/examples/howto_use_tfp.md
--rw-r--r--   0 runner    (1001) docker     (127)     5844 2024-02-21 10:50:57.000000 blackjax-1.1.1/docs/examples/quickstart.md
--rw-r--r--   0 runner    (1001) docker     (127)  4461357 2024-02-21 10:50:57.000000 blackjax-1.1.1/docs/examples/scatter.gif
--rw-r--r--   0 runner    (1001) docker     (127)     3165 2024-02-21 10:50:57.000000 blackjax-1.1.1/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)    13273 2024-02-21 10:50:57.000000 blackjax-1.1.1/docs/refs.bib
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-02-21 10:50:57.000000 blackjax-1.1.1/jupytex.toml
--rw-r--r--   0 runner    (1001) docker     (127)      249 2024-02-21 10:50:57.000000 blackjax-1.1.1/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (127)     1753 2024-02-21 10:50:57.000000 blackjax-1.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-02-21 10:50:57.000000 blackjax-1.1.1/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-02-21 10:50:57.000000 blackjax-1.1.1/requirements-doc.txt
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-02-21 10:50:57.000000 blackjax-1.1.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      403 2024-02-21 10:51:07.729128 blackjax-1.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 10:51:07.725128 blackjax-1.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-21 10:50:57.000000 blackjax-1.1.1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 10:51:07.725128 blackjax-1.1.1/tests/adaptation/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-21 10:50:57.000000 blackjax-1.1.1/tests/adaptation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2232 2024-02-21 10:50:57.000000 blackjax-1.1.1/tests/adaptation/test_adaptation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1683 2024-02-21 10:50:57.000000 blackjax-1.1.1/tests/adaptation/test_mass_matrix.py
--rw-r--r--   0 runner    (1001) docker     (127)     1798 2024-02-21 10:50:57.000000 blackjax-1.1.1/tests/adaptation/test_step_size.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 10:51:07.729128 blackjax-1.1.1/tests/mcmc/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-21 10:50:57.000000 blackjax-1.1.1/tests/mcmc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1722 2024-02-21 10:50:57.000000 blackjax-1.1.1/tests/mcmc/test_barker.py
--rw-r--r--   0 runner    (1001) docker     (127)    13030 2024-02-21 10:50:57.000000 blackjax-1.1.1/tests/mcmc/test_integrators.py
--rw-r--r--   0 runner    (1001) docker     (127)     2427 2024-02-21 10:50:57.000000 blackjax-1.1.1/tests/mcmc/test_latent_gaussian.py
--rw-r--r--   0 runner    (1001) docker     (127)     5983 2024-02-21 10:50:57.000000 blackjax-1.1.1/tests/mcmc/test_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     2350 2024-02-21 10:50:57.000000 blackjax-1.1.1/tests/mcmc/test_proposal.py
--rw-r--r--   0 runner    (1001) docker     (127)     5777 2024-02-21 10:50:57.000000 blackjax-1.1.1/tests/mcmc/test_random_walk_without_chex.py
--rw-r--r--   0 runner    (1001) docker     (127)    28460 2024-02-21 10:50:57.000000 blackjax-1.1.1/tests/mcmc/test_sampling.py
--rw-r--r--   0 runner    (1001) docker     (127)    11043 2024-02-21 10:50:57.000000 blackjax-1.1.1/tests/mcmc/test_trajectory.py
--rw-r--r--   0 runner    (1001) docker     (127)     1409 2024-02-21 10:50:57.000000 blackjax-1.1.1/tests/mcmc/test_uturn.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 10:51:07.729128 blackjax-1.1.1/tests/optimizers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-21 10:50:57.000000 blackjax-1.1.1/tests/optimizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5827 2024-02-21 10:50:57.000000 blackjax-1.1.1/tests/optimizers/test_optimizers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2907 2024-02-21 10:50:57.000000 blackjax-1.1.1/tests/optimizers/test_pathfinder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 10:51:07.729128 blackjax-1.1.1/tests/smc/
--rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-02-21 10:50:57.000000 blackjax-1.1.1/tests/smc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13177 2024-02-21 10:50:57.000000 blackjax-1.1.1/tests/smc/test_inner_kernel_tuning.py
--rw-r--r--   0 runner    (1001) docker     (127)     3175 2024-02-21 10:50:57.000000 blackjax-1.1.1/tests/smc/test_kernel_compatibility.py
--rw-r--r--   0 runner    (1001) docker     (127)     2190 2024-02-21 10:50:57.000000 blackjax-1.1.1/tests/smc/test_resampling.py
--rw-r--r--   0 runner    (1001) docker     (127)     3833 2024-02-21 10:50:57.000000 blackjax-1.1.1/tests/smc/test_smc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3658 2024-02-21 10:50:57.000000 blackjax-1.1.1/tests/smc/test_smc_ess.py
--rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-02-21 10:50:57.000000 blackjax-1.1.1/tests/smc/test_solver.py
--rw-r--r--   0 runner    (1001) docker     (127)     6631 2024-02-21 10:50:57.000000 blackjax-1.1.1/tests/smc/test_tempered_smc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2334 2024-02-21 10:50:57.000000 blackjax-1.1.1/tests/test_benchmarks.py
--rw-r--r--   0 runner    (1001) docker     (127)     3913 2024-02-21 10:50:57.000000 blackjax-1.1.1/tests/test_compilation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2620 2024-02-21 10:50:57.000000 blackjax-1.1.1/tests/test_diagnostics.py
--rw-r--r--   0 runner    (1001) docker     (127)     1540 2024-02-21 10:50:57.000000 blackjax-1.1.1/tests/test_util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 10:51:07.729128 blackjax-1.1.1/tests/vi/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-21 10:50:57.000000 blackjax-1.1.1/tests/vi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1542 2024-02-21 10:50:57.000000 blackjax-1.1.1/tests/vi/test_meanfield_vi.py
--rw-r--r--   0 runner    (1001) docker     (127)     2842 2024-02-21 10:50:57.000000 blackjax-1.1.1/tests/vi/test_schrodinger_follmer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3185 2024-02-21 10:50:57.000000 blackjax-1.1.1/tests/vi/test_svgd.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:18:53.177889 blackjax-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-06 16:18:44.000000 blackjax-1.2.0/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:18:53.149889 blackjax-1.2.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:18:53.149889 blackjax-1.2.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)     2317 2024-05-06 16:18:44.000000 blackjax-1.2.0/.github/ISSUE_TEMPLATE/bug_report.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-06 16:18:44.000000 blackjax-1.2.0/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      753 2024-05-06 16:18:44.000000 blackjax-1.2.0/.github/ISSUE_TEMPLATE/enhancement.md
+-rw-r--r--   0 runner    (1001) docker     (127)      721 2024-05-06 16:18:44.000000 blackjax-1.2.0/.github/ISSUE_TEMPLATE/meeting.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-05-06 16:18:44.000000 blackjax-1.2.0/.github/ISSUE_TEMPLATE/sampler_proposal.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-05-06 16:18:44.000000 blackjax-1.2.0/.github/PULL_REQUEST_TEMPLATE.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:18:53.153889 blackjax-1.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-05-06 16:18:44.000000 blackjax-1.2.0/.github/workflows/benchmark.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      542 2024-05-06 16:18:44.000000 blackjax-1.2.0/.github/workflows/build_documentation.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1616 2024-05-06 16:18:44.000000 blackjax-1.2.0/.github/workflows/nightly.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      782 2024-05-06 16:18:44.000000 blackjax-1.2.0/.github/workflows/publish_documentation.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-05-06 16:18:44.000000 blackjax-1.2.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-06 16:18:44.000000 blackjax-1.2.0/.github/workflows/schedule-meeting.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-05-06 16:18:44.000000 blackjax-1.2.0/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-05-06 16:18:44.000000 blackjax-1.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-05-06 16:18:44.000000 blackjax-1.2.0/.gitlint
+-rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-05-06 16:18:44.000000 blackjax-1.2.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-05-06 16:18:44.000000 blackjax-1.2.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3381 2024-05-06 16:18:44.000000 blackjax-1.2.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2324 2024-05-06 16:18:44.000000 blackjax-1.2.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4371 2024-05-06 16:18:44.000000 blackjax-1.2.0/GOVERNANCE.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11354 2024-05-06 16:18:44.000000 blackjax-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-06 16:18:44.000000 blackjax-1.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-05-06 16:18:44.000000 blackjax-1.2.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     6582 2024-05-06 16:18:53.177889 blackjax-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5108 2024-05-06 16:18:44.000000 blackjax-1.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:18:53.153889 blackjax-1.2.0/blackjax/
+-rw-r--r--   0 runner    (1001) docker     (127)     5330 2024-05-06 16:18:44.000000 blackjax-1.2.0/blackjax/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-06 16:18:53.000000 blackjax-1.2.0/blackjax/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:18:53.157889 blackjax-1.2.0/blackjax/adaptation/
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-06 16:18:44.000000 blackjax-1.2.0/blackjax/adaptation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      847 2024-05-06 16:18:44.000000 blackjax-1.2.0/blackjax/adaptation/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17121 2024-05-06 16:18:44.000000 blackjax-1.2.0/blackjax/adaptation/chees_adaptation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7640 2024-05-06 16:18:44.000000 blackjax-1.2.0/blackjax/adaptation/mass_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10236 2024-05-06 16:18:44.000000 blackjax-1.2.0/blackjax/adaptation/mclmc_adaptation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10582 2024-05-06 16:18:44.000000 blackjax-1.2.0/blackjax/adaptation/meads_adaptation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7576 2024-05-06 16:18:44.000000 blackjax-1.2.0/blackjax/adaptation/pathfinder_adaptation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9557 2024-05-06 16:18:44.000000 blackjax-1.2.0/blackjax/adaptation/step_size.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16440 2024-05-06 16:18:44.000000 blackjax-1.2.0/blackjax/adaptation/window_adaptation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5100 2024-05-06 16:18:44.000000 blackjax-1.2.0/blackjax/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7915 2024-05-06 16:18:44.000000 blackjax-1.2.0/blackjax/diagnostics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:18:53.157889 blackjax-1.2.0/blackjax/mcmc/
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-05-06 16:18:44.000000 blackjax-1.2.0/blackjax/mcmc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8885 2024-05-06 16:18:44.000000 blackjax-1.2.0/blackjax/mcmc/barker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1590 2024-05-06 16:18:44.000000 blackjax-1.2.0/blackjax/mcmc/diffusions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6891 2024-05-06 16:18:44.000000 blackjax-1.2.0/blackjax/mcmc/dynamic_hmc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9133 2024-05-06 16:18:44.000000 blackjax-1.2.0/blackjax/mcmc/elliptical_slice.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10649 2024-05-06 16:18:44.000000 blackjax-1.2.0/blackjax/mcmc/ghmc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11017 2024-05-06 16:18:44.000000 blackjax-1.2.0/blackjax/mcmc/hmc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16461 2024-05-06 16:18:44.000000 blackjax-1.2.0/blackjax/mcmc/integrators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5775 2024-05-06 16:18:44.000000 blackjax-1.2.0/blackjax/mcmc/mala.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8430 2024-05-06 16:18:44.000000 blackjax-1.2.0/blackjax/mcmc/marginal_latent_gaussian.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5741 2024-05-06 16:18:44.000000 blackjax-1.2.0/blackjax/mcmc/mclmc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11000 2024-05-06 16:18:44.000000 blackjax-1.2.0/blackjax/mcmc/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11050 2024-05-06 16:18:44.000000 blackjax-1.2.0/blackjax/mcmc/nuts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11963 2024-05-06 16:18:44.000000 blackjax-1.2.0/blackjax/mcmc/periodic_orbital.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8602 2024-05-06 16:18:44.000000 blackjax-1.2.0/blackjax/mcmc/proposal.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15645 2024-05-06 16:18:44.000000 blackjax-1.2.0/blackjax/mcmc/random_walk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3098 2024-05-06 16:18:44.000000 blackjax-1.2.0/blackjax/mcmc/rmhmc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3847 2024-05-06 16:18:44.000000 blackjax-1.2.0/blackjax/mcmc/termination.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22915 2024-05-06 16:18:44.000000 blackjax-1.2.0/blackjax/mcmc/trajectory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:18:53.161889 blackjax-1.2.0/blackjax/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-06 16:18:44.000000 blackjax-1.2.0/blackjax/optimizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4491 2024-05-06 16:18:44.000000 blackjax-1.2.0/blackjax/optimizers/dual_averaging.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11581 2024-05-06 16:18:44.000000 blackjax-1.2.0/blackjax/optimizers/lbfgs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2843 2024-05-06 16:18:44.000000 blackjax-1.2.0/blackjax/progress_bar.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:18:53.161889 blackjax-1.2.0/blackjax/sgmcmc/
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-06 16:18:44.000000 blackjax-1.2.0/blackjax/sgmcmc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8691 2024-05-06 16:18:44.000000 blackjax-1.2.0/blackjax/sgmcmc/csgld.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3953 2024-05-06 16:18:44.000000 blackjax-1.2.0/blackjax/sgmcmc/diffusions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4376 2024-05-06 16:18:44.000000 blackjax-1.2.0/blackjax/sgmcmc/gradients.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4545 2024-05-06 16:18:44.000000 blackjax-1.2.0/blackjax/sgmcmc/sghmc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3702 2024-05-06 16:18:44.000000 blackjax-1.2.0/blackjax/sgmcmc/sgld.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4549 2024-05-06 16:18:44.000000 blackjax-1.2.0/blackjax/sgmcmc/sgnht.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:18:53.161889 blackjax-1.2.0/blackjax/smc/
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-06 16:18:44.000000 blackjax-1.2.0/blackjax/smc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5311 2024-05-06 16:18:44.000000 blackjax-1.2.0/blackjax/smc/adaptive_tempered.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5535 2024-05-06 16:18:44.000000 blackjax-1.2.0/blackjax/smc/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2576 2024-05-06 16:18:44.000000 blackjax-1.2.0/blackjax/smc/ess.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5501 2024-05-06 16:18:44.000000 blackjax-1.2.0/blackjax/smc/inner_kernel_tuning.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4871 2024-05-06 16:18:44.000000 blackjax-1.2.0/blackjax/smc/resampling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2493 2024-05-06 16:18:44.000000 blackjax-1.2.0/blackjax/smc/solver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6640 2024-05-06 16:18:44.000000 blackjax-1.2.0/blackjax/smc/tempered.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:18:53.161889 blackjax-1.2.0/blackjax/smc/tuning/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 16:18:44.000000 blackjax-1.2.0/blackjax/smc/tuning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1576 2024-05-06 16:18:44.000000 blackjax-1.2.0/blackjax/smc/tuning/from_kernel_info.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1368 2024-05-06 16:18:44.000000 blackjax-1.2.0/blackjax/smc/tuning/from_particles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-05-06 16:18:44.000000 blackjax-1.2.0/blackjax/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7311 2024-05-06 16:18:44.000000 blackjax-1.2.0/blackjax/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:18:53.161889 blackjax-1.2.0/blackjax/vi/
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-06 16:18:44.000000 blackjax-1.2.0/blackjax/vi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5386 2024-05-06 16:18:44.000000 blackjax-1.2.0/blackjax/vi/meanfield_vi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8871 2024-05-06 16:18:44.000000 blackjax-1.2.0/blackjax/vi/pathfinder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7101 2024-05-06 16:18:44.000000 blackjax-1.2.0/blackjax/vi/schrodinger_follmer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5494 2024-05-06 16:18:44.000000 blackjax-1.2.0/blackjax/vi/svgd.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:18:53.177889 blackjax-1.2.0/blackjax.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6582 2024-05-06 16:18:53.000000 blackjax-1.2.0/blackjax.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4227 2024-05-06 16:18:53.000000 blackjax-1.2.0/blackjax.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 16:18:53.000000 blackjax-1.2.0/blackjax.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-06 16:18:53.000000 blackjax-1.2.0/blackjax.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-06 16:18:53.000000 blackjax-1.2.0/blackjax.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-05-06 16:18:44.000000 blackjax-1.2.0/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:18:53.165889 blackjax-1.2.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:18:53.165889 blackjax-1.2.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)   161829 2024-05-06 16:18:44.000000 blackjax-1.2.0/docs/_static/blackjax.png
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-06 16:18:44.000000 blackjax-1.2.0/docs/_static/custom.css
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-06 16:18:44.000000 blackjax-1.2.0/docs/bib.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4301 2024-05-06 16:18:44.000000 blackjax-1.2.0/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:18:53.165889 blackjax-1.2.0/docs/examples/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:18:53.173889 blackjax-1.2.0/docs/examples/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     4864 2024-05-06 16:18:44.000000 blackjax-1.2.0/docs/examples/data/blackjax.png
+-rw-r--r--   0 runner    (1001) docker     (127)    63251 2024-05-06 16:18:44.000000 blackjax-1.2.0/docs/examples/data/google.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     6030 2024-05-06 16:18:44.000000 blackjax-1.2.0/docs/examples/howto_custom_gradients.md
+-rw-r--r--   0 runner    (1001) docker     (127)    12029 2024-05-06 16:18:44.000000 blackjax-1.2.0/docs/examples/howto_metropolis_within_gibbs.md
+-rw-r--r--   0 runner    (1001) docker     (127)     6164 2024-05-06 16:18:44.000000 blackjax-1.2.0/docs/examples/howto_other_frameworks.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5494 2024-05-06 16:18:44.000000 blackjax-1.2.0/docs/examples/howto_reproduce_the_blackjax_image.md
+-rw-r--r--   0 runner    (1001) docker     (127)     9833 2024-05-06 16:18:44.000000 blackjax-1.2.0/docs/examples/howto_sample_multiple_chains.md
+-rw-r--r--   0 runner    (1001) docker     (127)     6722 2024-05-06 16:18:44.000000 blackjax-1.2.0/docs/examples/howto_use_aesara.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5248 2024-05-06 16:18:44.000000 blackjax-1.2.0/docs/examples/howto_use_numpyro.md
+-rw-r--r--   0 runner    (1001) docker     (127)     6122 2024-05-06 16:18:44.000000 blackjax-1.2.0/docs/examples/howto_use_oryx.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3357 2024-05-06 16:18:44.000000 blackjax-1.2.0/docs/examples/howto_use_pymc.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4641 2024-05-06 16:18:44.000000 blackjax-1.2.0/docs/examples/howto_use_tfp.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5844 2024-05-06 16:18:44.000000 blackjax-1.2.0/docs/examples/quickstart.md
+-rw-r--r--   0 runner    (1001) docker     (127)  4461357 2024-05-06 16:18:44.000000 blackjax-1.2.0/docs/examples/scatter.gif
+-rw-r--r--   0 runner    (1001) docker     (127)     3255 2024-05-06 16:18:44.000000 blackjax-1.2.0/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)    13273 2024-05-06 16:18:44.000000 blackjax-1.2.0/docs/refs.bib
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-06 16:18:44.000000 blackjax-1.2.0/jupytex.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-05-06 16:18:44.000000 blackjax-1.2.0/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     1753 2024-05-06 16:18:44.000000 blackjax-1.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-06 16:18:44.000000 blackjax-1.2.0/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-05-06 16:18:44.000000 blackjax-1.2.0/requirements-doc.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-06 16:18:44.000000 blackjax-1.2.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2024-05-06 16:18:53.177889 blackjax-1.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:18:53.173889 blackjax-1.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 16:18:44.000000 blackjax-1.2.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:18:53.173889 blackjax-1.2.0/tests/adaptation/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 16:18:44.000000 blackjax-1.2.0/tests/adaptation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2225 2024-05-06 16:18:44.000000 blackjax-1.2.0/tests/adaptation/test_adaptation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1683 2024-05-06 16:18:44.000000 blackjax-1.2.0/tests/adaptation/test_mass_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1798 2024-05-06 16:18:44.000000 blackjax-1.2.0/tests/adaptation/test_step_size.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:18:53.177889 blackjax-1.2.0/tests/mcmc/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 16:18:44.000000 blackjax-1.2.0/tests/mcmc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1722 2024-05-06 16:18:44.000000 blackjax-1.2.0/tests/mcmc/test_barker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13030 2024-05-06 16:18:44.000000 blackjax-1.2.0/tests/mcmc/test_integrators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2427 2024-05-06 16:18:44.000000 blackjax-1.2.0/tests/mcmc/test_latent_gaussian.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5983 2024-05-06 16:18:44.000000 blackjax-1.2.0/tests/mcmc/test_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2350 2024-05-06 16:18:44.000000 blackjax-1.2.0/tests/mcmc/test_proposal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5777 2024-05-06 16:18:44.000000 blackjax-1.2.0/tests/mcmc/test_random_walk_without_chex.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29756 2024-05-06 16:18:44.000000 blackjax-1.2.0/tests/mcmc/test_sampling.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10911 2024-05-06 16:18:44.000000 blackjax-1.2.0/tests/mcmc/test_trajectory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1409 2024-05-06 16:18:44.000000 blackjax-1.2.0/tests/mcmc/test_uturn.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:18:53.177889 blackjax-1.2.0/tests/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 16:18:44.000000 blackjax-1.2.0/tests/optimizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5827 2024-05-06 16:18:44.000000 blackjax-1.2.0/tests/optimizers/test_optimizers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2907 2024-05-06 16:18:44.000000 blackjax-1.2.0/tests/optimizers/test_pathfinder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:18:53.177889 blackjax-1.2.0/tests/smc/
+-rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-05-06 16:18:44.000000 blackjax-1.2.0/tests/smc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13930 2024-05-06 16:18:44.000000 blackjax-1.2.0/tests/smc/test_inner_kernel_tuning.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4212 2024-05-06 16:18:44.000000 blackjax-1.2.0/tests/smc/test_kernel_compatibility.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2190 2024-05-06 16:18:44.000000 blackjax-1.2.0/tests/smc/test_resampling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4922 2024-05-06 16:18:44.000000 blackjax-1.2.0/tests/smc/test_smc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3658 2024-05-06 16:18:44.000000 blackjax-1.2.0/tests/smc/test_smc_ess.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-05-06 16:18:44.000000 blackjax-1.2.0/tests/smc/test_solver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6852 2024-05-06 16:18:44.000000 blackjax-1.2.0/tests/smc/test_tempered_smc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2334 2024-05-06 16:18:44.000000 blackjax-1.2.0/tests/test_benchmarks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3897 2024-05-06 16:18:44.000000 blackjax-1.2.0/tests/test_compilation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2620 2024-05-06 16:18:44.000000 blackjax-1.2.0/tests/test_diagnostics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1531 2024-05-06 16:18:44.000000 blackjax-1.2.0/tests/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:18:53.177889 blackjax-1.2.0/tests/vi/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 16:18:44.000000 blackjax-1.2.0/tests/vi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-05-06 16:18:44.000000 blackjax-1.2.0/tests/vi/test_meanfield_vi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2862 2024-05-06 16:18:44.000000 blackjax-1.2.0/tests/vi/test_schrodinger_follmer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3185 2024-05-06 16:18:44.000000 blackjax-1.2.0/tests/vi/test_svgd.py
```

### Comparing `blackjax-1.1.1/.github/ISSUE_TEMPLATE/bug_report.yml` & `blackjax-1.2.0/.github/ISSUE_TEMPLATE/bug_report.yml`

 * *Files identical despite different names*

### Comparing `blackjax-1.1.1/.github/ISSUE_TEMPLATE/enhancement.md` & `blackjax-1.2.0/.github/ISSUE_TEMPLATE/enhancement.md`

 * *Files identical despite different names*

### Comparing `blackjax-1.1.1/.github/ISSUE_TEMPLATE/meeting.md` & `blackjax-1.2.0/.github/ISSUE_TEMPLATE/meeting.md`

 * *Files identical despite different names*

### Comparing `blackjax-1.1.1/.github/ISSUE_TEMPLATE/sampler_proposal.md` & `blackjax-1.2.0/.github/ISSUE_TEMPLATE/sampler_proposal.md`

 * *Files identical despite different names*

### Comparing `blackjax-1.1.1/.github/PULL_REQUEST_TEMPLATE.md` & `blackjax-1.2.0/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `blackjax-1.1.1/.github/workflows/benchmark.yml` & `blackjax-1.2.0/.github/workflows/benchmark.yml`

 * *Files identical despite different names*

### Comparing `blackjax-1.1.1/.github/workflows/build_documentation.yml` & `blackjax-1.2.0/.github/workflows/build_documentation.yml`

 * *Files identical despite different names*

### Comparing `blackjax-1.1.1/.github/workflows/nightly.yml` & `blackjax-1.2.0/.github/workflows/nightly.yml`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     runs-on: ubuntu-latest
     steps:
     - uses: actions/checkout@v3
       with:
         fetch-depth: 0
     - uses: actions/setup-python@v4
       with:
-        python-version: 3.9
+        python-version: 3.11
     - name: Update pyproject.toml
       # Taken from https://github.com/aesara-devs/aesara/pull/1375
       run: |
         curl -sSLf https://github.com/TomWright/dasel/releases/download/v2.0.2/dasel_linux_amd64 \
           -L -o /tmp/dasel && chmod +x /tmp/dasel
         /tmp/dasel put -f pyproject.toml project.name -v blackjax-nightly
         /tmp/dasel put -f pyproject.toml tool.setuptools_scm.version_scheme -v post-release
```

### Comparing `blackjax-1.1.1/.github/workflows/publish_documentation.yml` & `blackjax-1.2.0/.github/workflows/publish_documentation.yml`

 * *Files 3% similar despite different names*

```diff
@@ -10,18 +10,18 @@
     runs-on: ubuntu-latest
     steps:
       - name: Checkout the branch
         uses: actions/checkout@v3
         with:
           persist-credentials: false
 
-      - name: Set up Python 3.9
+      - name: Set up Python
         uses: actions/setup-python@v4
         with:
-          python-version: 3.9
+          python-version: 3.11
 
       - name: Build the documentation with Sphinx
         run: |
           pip install -r requirements-doc.txt
           sphinx-build -b html docs docs/build/html
 
       - name: Publish the documentation
```

### Comparing `blackjax-1.1.1/.github/workflows/release.yml` & `blackjax-1.2.0/.github/workflows/release.yml`

 * *Files 8% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     name: Build and publish on PyPi
     runs-on: ubuntu-latest
     steps:
     - uses: actions/checkout@v3
     - name: Set up Python
       uses: actions/setup-python@v4
       with:
-        python-version: 3.9
+        python-version: 3.11
     - name: Build sdist and wheel
       run: |
         python -m pip install -U pip
         python -m pip install build
         python -m build
     - name: Check that the package version matches the Release name
       run: |
@@ -47,13 +47,13 @@
     name: Test install from PyPi
     needs: release-job
     runs-on: ubuntu-latest
     steps:
     - name: Set up Python
       uses: actions/setup-python@v4
       with:
-        python-version: 3.9
+        python-version: 3.11
     - name: Give PyPI some time to update the index
       run: sleep 240
     - name: Attempt install from PyPI
       run: |
         pip install blackjax==${GITHUB_REF:10}
```

### Comparing `blackjax-1.1.1/.github/workflows/test.yml` & `blackjax-1.2.0/.github/workflows/test.yml`

 * *Files 3% similar despite different names*

```diff
@@ -10,25 +10,25 @@
   style:
     name: Check the code style
     runs-on: ubuntu-latest
     steps:
     - uses: actions/checkout@v3
     - uses: actions/setup-python@v4
       with:
-        python-version: 3.9
+        python-version: 3.11
     - uses: pre-commit/action@v3.0.0
 
   test:
     name: Run tests for Python ${{ matrix.python-version }}
     runs-on: ubuntu-latest
     needs:
       - style
     strategy:
       matrix:
-        python-version: [ '3.9', '3.11']
+        python-version: ['3.11', '3.12']
     steps:
     - uses: actions/checkout@v3
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v4
       with:
         python-version: ${{ matrix.python-version }}
     - name: Set up test environment
```

### Comparing `blackjax-1.1.1/.gitignore` & `blackjax-1.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `blackjax-1.1.1/.gitlint` & `blackjax-1.2.0/.gitlint`

 * *Files identical despite different names*

### Comparing `blackjax-1.1.1/.pre-commit-config.yaml` & `blackjax-1.2.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `blackjax-1.1.1/CODE_OF_CONDUCT.md` & `blackjax-1.2.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `blackjax-1.1.1/CONTRIBUTING.md` & `blackjax-1.2.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `blackjax-1.1.1/GOVERNANCE.md` & `blackjax-1.2.0/GOVERNANCE.md`

 * *Files identical despite different names*

### Comparing `blackjax-1.1.1/LICENSE` & `blackjax-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `blackjax-1.1.1/Makefile` & `blackjax-1.2.0/Makefile`

 * *Files identical despite different names*

### Comparing `blackjax-1.1.1/PKG-INFO` & `blackjax-1.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blackjax
-Version: 1.1.1
+Version: 1.2.0
 Summary: Flexible and fast sampling in Python
 Author-email: The Blackjax team <remi@thetypicalset.com>
 License: Apache License 2.0
 Project-URL: homepage, https://github.com/blackjax-devs/blackjax
 Project-URL: documentation, https://blackjax-devs.github.io/blackjax/
 Project-URL: repository, https://github.com/blackjax-devs/blackjax
 Keywords: probability,machine learning,statistics,mcmc,sampling
@@ -114,16 +114,16 @@
 
 # Initialize the state
 initial_position = {"loc": 1., "scale": 2.}
 state = nuts.init(initial_position)
 
 # Iterate
 rng_key = jax.random.key(0)
-for _ in range(100):
-    rng_key, nuts_key = jax.random.split(rng_key)
+for step in range(100):
+    nuts_key = jax.random.fold_in(rng_key, step)
     state, _ = nuts.step(nuts_key, state)
 ```
 
 See [the documentation](https://blackjax-devs.github.io/blackjax/index.html) for more examples of how to use the library: how to write inference loops for one or several chains, how to use the Stan warmup, etc.
 
 ## Philosophy
```

### Comparing `blackjax-1.1.1/README.md` & `blackjax-1.2.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -77,16 +77,16 @@
 
 # Initialize the state
 initial_position = {"loc": 1., "scale": 2.}
 state = nuts.init(initial_position)
 
 # Iterate
 rng_key = jax.random.key(0)
-for _ in range(100):
-    rng_key, nuts_key = jax.random.split(rng_key)
+for step in range(100):
+    nuts_key = jax.random.fold_in(rng_key, step)
     state, _ = nuts.step(nuts_key, state)
 ```
 
 See [the documentation](https://blackjax-devs.github.io/blackjax/index.html) for more examples of how to use the library: how to write inference loops for one or several chains, how to use the Stan warmup, etc.
 
 ## Philosophy
```

### Comparing `blackjax-1.1.1/blackjax/adaptation/base.py` & `blackjax-1.2.0/blackjax/adaptation/base.py`

 * *Files identical despite different names*

### Comparing `blackjax-1.1.1/blackjax/adaptation/chees_adaptation.py` & `blackjax-1.2.0/blackjax/adaptation/chees_adaptation.py`

 * *Files 1% similar despite different names*

```diff
@@ -357,28 +357,26 @@
         assert all(
             jax.tree_util.tree_flatten(
                 jax.tree_util.tree_map(lambda p: p.shape[0] == num_chains, positions)
             )[0]
         ), "initial `positions` leading dimension must be equal to the `num_chains`"
         num_dim = pytree_size(positions) // num_chains
 
-        key_init, key_step = jax.random.split(rng_key)
+        next_random_arg_fn = lambda i: i + 1
+        init_random_arg = 0
 
         if jitter_generator is not None:
-            jitter_gn = lambda key: jitter_generator(key) * jitter_amount + (
-                1.0 - jitter_amount
-            )
-            next_random_arg_fn = lambda key: jax.random.split(key)[1]
-            init_random_arg = key_init
+            rng_key, carry_key = jax.random.split(rng_key)
+            jitter_gn = lambda i: jitter_generator(
+                jax.random.fold_in(carry_key, i)
+            ) * jitter_amount + (1.0 - jitter_amount)
         else:
             jitter_gn = lambda i: dynamic_hmc.halton_sequence(
                 i, np.ceil(np.log2(num_steps + max_sampling_steps))
             ) * jitter_amount + (1.0 - jitter_amount)
-            next_random_arg_fn = lambda i: i + 1
-            init_random_arg = 0
 
         def integration_steps_fn(random_generator_arg, trajectory_length_adjusted):
             return jnp.asarray(
                 jnp.ceil(jitter_gn(random_generator_arg) * trajectory_length_adjusted),
                 dtype=int,
             )
 
@@ -421,15 +419,15 @@
 
         batch_init = jax.vmap(
             lambda p: dynamic_hmc.init(p, logdensity_fn, init_random_arg)
         )
         init_states = batch_init(positions)
         init_adaptation_state = init(init_random_arg, step_size)
 
-        keys_step = jax.random.split(key_step, num_steps)
+        keys_step = jax.random.split(rng_key, num_steps)
         (last_states, last_adaptation_state), info = jax.lax.scan(
             one_step, (init_states, init_adaptation_state), keys_step
         )
 
         trajectory_length_adjusted = jnp.exp(
             last_adaptation_state.log_trajectory_length_moving_average
             - last_adaptation_state.log_step_size_moving_average
```

### Comparing `blackjax-1.1.1/blackjax/adaptation/mass_matrix.py` & `blackjax-1.2.0/blackjax/adaptation/mass_matrix.py`

 * *Files identical despite different names*

### Comparing `blackjax-1.1.1/blackjax/adaptation/mclmc_adaptation.py` & `blackjax-1.2.0/blackjax/adaptation/mclmc_adaptation.py`

 * *Files 0% similar despite different names*

```diff
@@ -227,20 +227,20 @@
         # we use the last num_steps2 to compute the diagonal preconditioner
         outer_weights = jnp.concatenate((jnp.zeros(num_steps1), jnp.ones(num_steps2)))
 
         # initial state of the kalman filter
         kalman_state = (0.0, jnp.zeros(dim), jnp.zeros(dim))
 
         # run the steps
-        kalman_state = jax.lax.scan(
+        kalman_state, *_ = jax.lax.scan(
             step,
             init=(state, params, adap0, kalman_state),
             xs=(outer_weights, L_step_size_adaptation_keys),
             length=num_steps1 + num_steps2,
-        )[0]
+        )
         state, params, _, kalman_state_output = kalman_state
 
         L = params.L
         # determine L
         if num_steps2 != 0.0:
             _, F1, F2 = kalman_state_output
             variances = F2 - jnp.square(F1)
```

### Comparing `blackjax-1.1.1/blackjax/adaptation/meads_adaptation.py` & `blackjax-1.2.0/blackjax/adaptation/meads_adaptation.py`

 * *Files 1% similar despite different names*

```diff
@@ -89,24 +89,24 @@
 
         Returns
         -------
         New values of the step size, and the alpha and delta parameters
         of the generalized HMC algorithm.
 
         """
-        mean_position = jax.tree_map(lambda p: p.mean(axis=0), positions)
-        sd_position = jax.tree_map(lambda p: p.std(axis=0), positions)
-        normalized_positions = jax.tree_map(
+        mean_position = jax.tree.map(lambda p: p.mean(axis=0), positions)
+        sd_position = jax.tree.map(lambda p: p.std(axis=0), positions)
+        normalized_positions = jax.tree.map(
             lambda p, mu, sd: (p - mu) / sd,
             positions,
             mean_position,
             sd_position,
         )
 
-        batch_grad_scaled = jax.tree_map(
+        batch_grad_scaled = jax.tree.map(
             lambda grad, sd: grad * sd, logdensity_grad, sd_position
         )
 
         epsilon = jnp.minimum(
             0.5 / jnp.sqrt(maximum_eigenvalue(batch_grad_scaled)), 1.0
         )
         gamma = jnp.maximum(
```

### Comparing `blackjax-1.1.1/blackjax/adaptation/pathfinder_adaptation.py` & `blackjax-1.2.0/blackjax/adaptation/pathfinder_adaptation.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,20 +8,19 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Implementation of the Pathinder warmup for the HMC family of sampling algorithms."""
-from typing import Callable, NamedTuple, Union
+from typing import Callable, NamedTuple
 
 import jax
 import jax.numpy as jnp
 
-import blackjax.mcmc as mcmc
 import blackjax.vi as vi
 from blackjax.adaptation.base import AdaptationInfo, AdaptationResults
 from blackjax.adaptation.step_size import (
     DualAveragingAdaptationState,
     dual_averaging_adaptation,
 )
 from blackjax.base import AdaptationAlgorithm
@@ -134,15 +133,15 @@
         inverse_mass_matrix = warmup_state.inverse_mass_matrix
         return step_size, inverse_mass_matrix
 
     return init, update, final
 
 
 def pathfinder_adaptation(
-    algorithm: Union[mcmc.hmc.hmc, mcmc.nuts.nuts],
+    algorithm,
     logdensity_fn: Callable,
     initial_step_size: float = 1.0,
     target_acceptance_rate: float = 0.80,
     **extra_parameters,
 ) -> AdaptationAlgorithm:
     """Adapt the value of the inverse mass matrix and step size parameters of
     algorithms in the HMC fmaily.
```

### Comparing `blackjax-1.1.1/blackjax/adaptation/step_size.py` & `blackjax-1.2.0/blackjax/adaptation/step_size.py`

 * *Files 2% similar despite different names*

```diff
@@ -154,28 +154,28 @@
 #                 REASONABLE FIRST STEP SIZE
 # -------------------------------------------------------------------
 
 
 class ReasonableStepSizeState(NamedTuple):
     """State carried through the search for a reasonable first step size.
 
-    rng_key
-        Key used by JAX's random number generator.
+    step
+        The current iteration step.
     direction: {-1, 1}
         Determines whether the step size should be increased or decreased during the
         previous step search. If direction = 1 it will be increased, otherwise decreased.
     previous_direction
         The previous direction. It is necessary to carry it because the choice of step
         size is made at the end of the search update.
     step_size
         The current step size in the search.
 
     """
 
-    rng_key: PRNGKey
+    step: int
     direction: int
     previous_direction: int
     step_size: float
 
 
 def find_reasonable_step_size(
     rng_key: PRNGKey,
@@ -239,21 +239,21 @@
         has_acceptance_rate_not_crossed_threshold = (previous_direction == 0) | (
             direction == previous_direction
         )
         return is_step_size_not_extreme & has_acceptance_rate_not_crossed_threshold
 
     def update(rss_state: ReasonableStepSizeState) -> ReasonableStepSizeState:
         """Perform one step of the step size search."""
-        rng_key, direction, _, step_size = rss_state
-        rng_key, subkey = jax.random.split(rng_key)
+        i, direction, _, step_size = rss_state
+        subkey = jax.random.fold_in(rng_key, i)
 
         step_size = (2.0**direction) * step_size
         kernel = kernel_generator(step_size)
         _, info = kernel(subkey, reference_state)
 
         new_direction = jnp.where(target_accept < info.acceptance_rate, 1, -1)
-        return ReasonableStepSizeState(rng_key, new_direction, direction, step_size)
+        return ReasonableStepSizeState(i + 1, new_direction, direction, step_size)
 
-    rss_state = ReasonableStepSizeState(rng_key, 0, 0, initial_step_size)
+    rss_state = ReasonableStepSizeState(0, 0, 0, initial_step_size)
     rss_state = jax.lax.while_loop(do_continue, update, rss_state)
 
     return rss_state.step_size
```

### Comparing `blackjax-1.1.1/blackjax/adaptation/window_adaptation.py` & `blackjax-1.2.0/blackjax/adaptation/window_adaptation.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,20 +8,19 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Implementation of the Stan warmup for the HMC family of sampling algorithms."""
-from typing import Callable, NamedTuple, Union
+from typing import Callable, NamedTuple
 
 import jax
 import jax.numpy as jnp
 
-import blackjax.mcmc as mcmc
 from blackjax.adaptation.base import AdaptationInfo, AdaptationResults
 from blackjax.adaptation.mass_matrix import (
     MassMatrixAdaptationState,
     mass_matrix_adaptation,
 )
 from blackjax.adaptation.step_size import (
     DualAveragingAdaptationState,
@@ -239,24 +238,24 @@
         inverse_mass_matrix = warmup_state.imm_state.inverse_mass_matrix
         return step_size, inverse_mass_matrix
 
     return init, update, final
 
 
 def window_adaptation(
-    algorithm: Union[mcmc.hmc.hmc, mcmc.nuts.nuts],
+    algorithm,
     logdensity_fn: Callable,
     is_mass_matrix_diagonal: bool = True,
     initial_step_size: float = 1.0,
     target_acceptance_rate: float = 0.80,
     progress_bar: bool = False,
     **extra_parameters,
 ) -> AdaptationAlgorithm:
     """Adapt the value of the inverse mass matrix and step size parameters of
-    algorithms in the HMC fmaily.
+    algorithms in the HMC family.  See Blackjax.hmc_family
 
     Algorithms in the HMC family on a euclidean manifold depend on the value of
     at least two parameters: the step size, related to the trajectory
     integrator, and the mass matrix, linked to the euclidean metric.
 
     Good tuning is very important, especially for algorithms like NUTS which can
     be extremely inefficient with the wrong parameter values. This function
```

### Comparing `blackjax-1.1.1/blackjax/base.py` & `blackjax-1.2.0/blackjax/base.py`

 * *Files identical despite different names*

### Comparing `blackjax-1.1.1/blackjax/diagnostics.py` & `blackjax-1.2.0/blackjax/diagnostics.py`

 * *Files identical despite different names*

### Comparing `blackjax-1.1.1/blackjax/mcmc/barker.py` & `blackjax-1.2.0/blackjax/mcmc/barker.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 from jax.scipy import stats
 from jax.tree_util import tree_leaves, tree_map
 
 from blackjax.base import SamplingAlgorithm
 from blackjax.mcmc.proposal import static_binomial_sampling
 from blackjax.types import ArrayLikeTree, ArrayTree, PRNGKey
 
-__all__ = ["BarkerState", "BarkerInfo", "init", "build_kernel", "barker_proposal"]
+__all__ = ["BarkerState", "BarkerInfo", "init", "build_kernel", "as_top_level_api"]
 
 
 class BarkerState(NamedTuple):
     """State of the Barker's proposal algorithm.
 
     The Barker algorithm takes one position of the chain and returns another
     position. In order to make computations more efficient, we also store
@@ -124,15 +124,18 @@
         )
         do_accept, p_accept, _ = info
         return accepted_state, BarkerInfo(p_accept, do_accept, proposed_state)
 
     return kernel
 
 
-class barker_proposal:
+def as_top_level_api(
+    logdensity_fn: Callable,
+    step_size: float,
+) -> SamplingAlgorithm:
     """Implements the (basic) user interface for the Barker's proposal :cite:p:`Livingstone2022Barker` kernel with a
     Gaussian base kernel.
 
     The general Barker kernel builder (:meth:`blackjax.mcmc.barker.build_kernel`, alias `blackjax.barker.build_kernel`) can be
     cumbersome to manipulate. Since most users only need to specify the kernel
     parameters at initialization time, we provide a helper function that
     specializes the general kernel.
@@ -175,32 +178,24 @@
 
     Returns
     -------
     A ``SamplingAlgorithm``.
 
     """
 
-    init = staticmethod(init)
-    build_kernel = staticmethod(build_kernel)
+    kernel = build_kernel()
 
-    def __new__(  # type: ignore[misc]
-        cls,
-        logdensity_fn: Callable,
-        step_size: float,
-    ) -> SamplingAlgorithm:
-        kernel = cls.build_kernel()
-
-        def init_fn(position: ArrayLikeTree, rng_key=None):
-            del rng_key
-            return cls.init(position, logdensity_fn)
+    def init_fn(position: ArrayLikeTree, rng_key=None):
+        del rng_key
+        return init(position, logdensity_fn)
 
-        def step_fn(rng_key: PRNGKey, state):
-            return kernel(rng_key, state, logdensity_fn, step_size)
+    def step_fn(rng_key: PRNGKey, state):
+        return kernel(rng_key, state, logdensity_fn, step_size)
 
-        return SamplingAlgorithm(init_fn, step_fn)
+    return SamplingAlgorithm(init_fn, step_fn)
 
 
 def _barker_sample_nd(key, mean, a, scale):
     """
     Sample from a multivariate Barker's proposal distribution. In 1D, this has the following probability density function:
 
     .. math::
```

### Comparing `blackjax-1.1.1/blackjax/mcmc/diffusions.py` & `blackjax-1.2.0/blackjax/mcmc/diffusions.py`

 * *Files identical despite different names*

### Comparing `blackjax-1.1.1/blackjax/mcmc/dynamic_hmc.py` & `blackjax-1.2.0/blackjax/mcmc/dynamic_hmc.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,16 +23,16 @@
 from blackjax.mcmc.hmc import build_kernel as build_static_hmc_kernel
 from blackjax.types import Array, ArrayLikeTree, ArrayTree, PRNGKey
 
 __all__ = [
     "DynamicHMCState",
     "init",
     "build_kernel",
-    "dynamic_hmc",
     "halton_sequence",
+    "as_top_level_api",
 ]
 
 
 class DynamicHMCState(NamedTuple):
     """State of the dynamic HMC algorithm.
 
     Adds a utility array for generating a pseudo or quasi-random sequence of
@@ -111,15 +111,24 @@
             ),
             info,
         )
 
     return kernel
 
 
-class dynamic_hmc:
+def as_top_level_api(
+    logdensity_fn: Callable,
+    step_size: float,
+    inverse_mass_matrix: Array,
+    *,
+    divergence_threshold: int = 1000,
+    integrator: Callable = integrators.velocity_verlet,
+    next_random_arg_fn: Callable = lambda key: jax.random.split(key)[1],
+    integration_steps_fn: Callable = lambda key: jax.random.randint(key, (), 1, 10),
+) -> SamplingAlgorithm:
     """Implements the (basic) user interface for the dynamic HMC kernel.
 
     Parameters
     ----------
     logdensity_fn
         The log-density function we wish to draw samples from.
     step_size
@@ -140,49 +149,34 @@
         sequence, given the current `random_generator_arg`.
 
 
     Returns
     -------
     A ``SamplingAlgorithm``.
     """
+    kernel = build_kernel(
+        integrator, divergence_threshold, next_random_arg_fn, integration_steps_fn
+    )
+
+    def init_fn(position: ArrayLikeTree, rng_key: Array):
+        # Note that rng_key here is not necessarily a PRNGKey, could be a Array that
+        # for generates a sequence of pseudo or quasi-random numbers (previously
+        # named as `random_generator_arg`)
+        return init(position, logdensity_fn, rng_key)
 
-    init = staticmethod(init)
-    build_kernel = staticmethod(build_kernel)
-
-    def __new__(  # type: ignore[misc]
-        cls,
-        logdensity_fn: Callable,
-        step_size: float,
-        inverse_mass_matrix: Array,
-        *,
-        divergence_threshold: int = 1000,
-        integrator: Callable = integrators.velocity_verlet,
-        next_random_arg_fn: Callable = lambda key: jax.random.split(key)[1],
-        integration_steps_fn: Callable = lambda key: jax.random.randint(key, (), 1, 10),
-    ) -> SamplingAlgorithm:
-        kernel = cls.build_kernel(
-            integrator, divergence_threshold, next_random_arg_fn, integration_steps_fn
+    def step_fn(rng_key: PRNGKey, state):
+        return kernel(
+            rng_key,
+            state,
+            logdensity_fn,
+            step_size,
+            inverse_mass_matrix,
         )
 
-        def init_fn(position: ArrayLikeTree, rng_key: Array):
-            # Note that rng_key here is not necessarily a PRNGKey, could be a Array that
-            # for generates a sequence of pseudo or quasi-random numbers (previously
-            # named as `random_generator_arg`)
-            return cls.init(position, logdensity_fn, rng_key)
-
-        def step_fn(rng_key: PRNGKey, state):
-            return kernel(
-                rng_key,
-                state,
-                logdensity_fn,
-                step_size,
-                inverse_mass_matrix,
-            )
-
-        return SamplingAlgorithm(init_fn, step_fn)
+    return SamplingAlgorithm(init_fn, step_fn)
 
 
 def halton_sequence(i: Array, max_bits: int = 10) -> float:
     bit_masks = 2 ** jnp.arange(max_bits, dtype=i.dtype)
     return jnp.einsum("i,i->", jnp.mod((i + 1) // bit_masks, 2), 0.5 / bit_masks)
```

### Comparing `blackjax-1.1.1/blackjax/mcmc/elliptical_slice.py` & `blackjax-1.2.0/blackjax/mcmc/elliptical_slice.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 from blackjax.util import generate_gaussian_noise
 
 __all__ = [
     "EllipSliceState",
     "EllipSliceInfo",
     "init",
     "build_kernel",
-    "elliptical_slice",
+    "as_top_level_api",
 ]
 
 
 class EllipSliceState(NamedTuple):
     """State of the Elliptical Slice sampling algorithm.
 
     position
@@ -115,15 +115,20 @@
             logdensity_fn, momentum_generator, mean
         )
         return proposal_generator(rng_key, state)
 
     return kernel
 
 
-class elliptical_slice:
+def as_top_level_api(
+    loglikelihood_fn: Callable,
+    *,
+    mean: Array,
+    cov: Array,
+) -> SamplingAlgorithm:
     """Implements the (basic) user interface for the Elliptical Slice sampling kernel.
 
     Examples
     --------
 
     A new Elliptical Slice sampling kernel can be initialized and used with the following code:
 
@@ -147,39 +152,28 @@
     cov_matrix
         The value of the covariance matrix of the gaussian prior distribution from the posterior we wish to sample.
 
     Returns
     -------
     A ``SamplingAlgorithm``.
     """
+    kernel = build_kernel(cov, mean)
 
-    init = staticmethod(init)
-    build_kernel = staticmethod(build_kernel)
-
-    def __new__(  # type: ignore[misc]
-        cls,
-        loglikelihood_fn: Callable,
-        *,
-        mean: Array,
-        cov: Array,
-    ) -> SamplingAlgorithm:
-        kernel = cls.build_kernel(cov, mean)
-
-        def init_fn(position: ArrayLikeTree, rng_key=None):
-            del rng_key
-            return cls.init(position, loglikelihood_fn)
-
-        def step_fn(rng_key: PRNGKey, state):
-            return kernel(
-                rng_key,
-                state,
-                loglikelihood_fn,
-            )
+    def init_fn(position: ArrayLikeTree, rng_key=None):
+        del rng_key
+        return init(position, loglikelihood_fn)
+
+    def step_fn(rng_key: PRNGKey, state):
+        return kernel(
+            rng_key,
+            state,
+            loglikelihood_fn,
+        )
 
-        return SamplingAlgorithm(init_fn, step_fn)
+    return SamplingAlgorithm(init_fn, step_fn)
 
 
 def elliptical_proposal(
     logdensity_fn: Callable,
     momentum_generator: Callable,
     mean: Array,
 ) -> Callable:
@@ -204,15 +198,15 @@
 
     """
 
     def generate(
         rng_key: PRNGKey, state: EllipSliceState
     ) -> tuple[EllipSliceState, EllipSliceInfo]:
         position, logdensity = state
-        key_momentum, key_uniform, key_theta = jax.random.split(rng_key, 3)
+        key_slice, key_momentum, key_uniform, key_theta = jax.random.split(rng_key, 4)
         # step 1: sample momentum
         momentum = momentum_generator(key_momentum, position)
         # step 2: get slice (y)
         logy = logdensity + jnp.log(jax.random.uniform(key_uniform))
         # step 3: get theta (ellipsis move), set inital interval
         theta = 2 * jnp.pi * jax.random.uniform(key_theta)
         theta_min = theta - 2 * jnp.pi
@@ -231,28 +225,28 @@
 
             As the bracket `[theta_min, theta_max]` shrinks, the proposal gets closer
             to the original position, which has likelihood larger than the slice variable.
             It is guaranteed to stop in a finite number of iterations as long as the
             likelihood is continuous with respect to the parameter being sampled.
 
             """
-            rng, _, subiter, theta, theta_min, theta_max, *_ = vals
-            rng, thetak = jax.random.split(rng)
+            _, subiter, theta, theta_min, theta_max, *_ = vals
+            thetak = jax.random.fold_in(key_slice, subiter)
             theta = jax.random.uniform(thetak, minval=theta_min, maxval=theta_max)
             p, m = ellipsis(position, momentum, theta, mean)
             logdensity = logdensity_fn(p)
             theta_min = jnp.where(theta < 0, theta, theta_min)
             theta_max = jnp.where(theta > 0, theta, theta_max)
             subiter += 1
-            return rng, logdensity, subiter, theta, theta_min, theta_max, p, m
+            return logdensity, subiter, theta, theta_min, theta_max, p, m
 
-        _, logdensity, subiter, theta, *_, position, momentum = jax.lax.while_loop(
-            lambda vals: vals[1] <= logy,
+        logdensity, subiter, theta, *_, position, momentum = jax.lax.while_loop(
+            lambda vals: vals[0] <= logy,
             slice_fn,
-            (rng_key, logdensity, 1, theta, theta_min, theta_max, p, m),
+            (logdensity, 1, theta, theta_min, theta_max, p, m),
         )
         return (
             EllipSliceState(position, logdensity),
             EllipSliceInfo(momentum, theta, subiter),
         )
 
     return generate
```

### Comparing `blackjax-1.1.1/blackjax/mcmc/ghmc.py` & `blackjax-1.2.0/blackjax/mcmc/ghmc.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 import blackjax.mcmc.integrators as integrators
 import blackjax.mcmc.metrics as metrics
 from blackjax.base import SamplingAlgorithm
 from blackjax.mcmc.proposal import nonreversible_slice_sampling
 from blackjax.types import ArrayLikeTree, ArrayTree, PRNGKey
 from blackjax.util import generate_gaussian_noise
 
-__all__ = ["GHMCState", "init", "build_kernel", "ghmc"]
+__all__ = ["GHMCState", "init", "build_kernel", "as_top_level_api"]
 
 
 class GHMCState(NamedTuple):
     """State of the Generalized HMC algorithm.
 
     The Generalized HMC algorithm is persistent on its momentum, hence
     taking as input a position and momentum pair, updating and returning
@@ -181,25 +181,34 @@
     an updated momentum that is a mixture of the previous momentum a new sample
     from a Gaussian density (dependent on alpha). The weights of the mixture of
     these two components are a function of alpha.
 
     """
     position, momentum, *_ = state
 
-    momentum = jax.tree_map(
+    momentum = jax.tree.map(
         lambda prev_momentum, shifted_momentum: prev_momentum * jnp.sqrt(1.0 - alpha)
         + jnp.sqrt(alpha) * shifted_momentum,
         momentum,
         momentum_generator(rng_key, position),
     )
 
     return momentum
 
 
-class ghmc:
+def as_top_level_api(
+    logdensity_fn: Callable,
+    step_size: float,
+    momentum_inverse_scale: ArrayLikeTree,
+    alpha: float,
+    delta: float,
+    *,
+    divergence_threshold: int = 1000,
+    noise_gn: Callable = lambda _: 0.0,
+) -> SamplingAlgorithm:
     """Implements the (basic) user interface for the Generalized HMC kernel.
 
     The Generalized HMC kernel performs a similar procedure to the standard HMC
     kernel with the difference of a persistent momentum variable and a non-reversible
     Metropolis-Hastings step instead of the standard Metropolis-Hastings acceptance
     step.
 
@@ -253,38 +262,24 @@
         The parameter defaults to a random variable with a single atom at 0.
 
     Returns
     -------
     A ``SamplingAlgorithm``.
     """
 
-    init = staticmethod(init)
-    build_kernel = staticmethod(build_kernel)
+    kernel = build_kernel(noise_gn, divergence_threshold)
 
-    def __new__(  # type: ignore[misc]
-        cls,
-        logdensity_fn: Callable,
-        step_size: float,
-        momentum_inverse_scale: ArrayLikeTree,
-        alpha: float,
-        delta: float,
-        *,
-        divergence_threshold: int = 1000,
-        noise_gn: Callable = lambda _: 0.0,
-    ) -> SamplingAlgorithm:
-        kernel = cls.build_kernel(noise_gn, divergence_threshold)
-
-        def init_fn(position: ArrayLikeTree, rng_key: PRNGKey):
-            return cls.init(position, rng_key, logdensity_fn)
-
-        def step_fn(rng_key: PRNGKey, state):
-            return kernel(
-                rng_key,
-                state,
-                logdensity_fn,
-                step_size,
-                momentum_inverse_scale,
-                alpha,
-                delta,
-            )
+    def init_fn(position: ArrayLikeTree, rng_key: PRNGKey):
+        return init(position, rng_key, logdensity_fn)
+
+    def step_fn(rng_key: PRNGKey, state):
+        return kernel(
+            rng_key,
+            state,
+            logdensity_fn,
+            step_size,
+            momentum_inverse_scale,
+            alpha,
+            delta,
+        )
 
-        return SamplingAlgorithm(init_fn, step_fn)
+    return SamplingAlgorithm(init_fn, step_fn)
```

### Comparing `blackjax-1.1.1/blackjax/mcmc/hmc.py` & `blackjax-1.2.0/blackjax/mcmc/hmc.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 from blackjax.types import ArrayLikeTree, ArrayTree, PRNGKey
 
 __all__ = [
     "HMCState",
     "HMCInfo",
     "init",
     "build_kernel",
-    "hmc",
+    "as_top_level_api",
 ]
 
 
 class HMCState(NamedTuple):
     """State of the HMC algorithm.
 
     The HMC algorithm takes one position of the chain and returns another
@@ -146,15 +146,23 @@
         )
 
         return proposal, info
 
     return kernel
 
 
-class hmc:
+def as_top_level_api(
+    logdensity_fn: Callable,
+    step_size: float,
+    inverse_mass_matrix: metrics.MetricTypes,
+    num_integration_steps: int,
+    *,
+    divergence_threshold: int = 1000,
+    integrator: Callable = integrators.velocity_verlet,
+) -> SamplingAlgorithm:
     """Implements the (basic) user interface for the HMC kernel.
 
     The general hmc kernel builder (:meth:`blackjax.mcmc.hmc.build_kernel`, alias
     `blackjax.hmc.build_kernel`) can be cumbersome to manipulate. Since most users only
     need to specify the kernel parameters at initialization time, we provide a helper
     function that specializes the general kernel.
 
@@ -221,44 +229,31 @@
         trajectory.
 
     Returns
     -------
     A ``SamplingAlgorithm``.
     """
 
-    init = staticmethod(init)
-    build_kernel = staticmethod(build_kernel)
+    kernel = build_kernel(integrator, divergence_threshold)
 
-    def __new__(  # type: ignore[misc]
-        cls,
-        logdensity_fn: Callable,
-        step_size: float,
-        inverse_mass_matrix: metrics.MetricTypes,
-        num_integration_steps: int,
-        *,
-        divergence_threshold: int = 1000,
-        integrator: Callable = integrators.velocity_verlet,
-    ) -> SamplingAlgorithm:
-        kernel = cls.build_kernel(integrator, divergence_threshold)
-
-        def init_fn(position: ArrayLikeTree, rng_key=None):
-            del rng_key
-            return cls.init(position, logdensity_fn)
-
-        def step_fn(rng_key: PRNGKey, state):
-            return kernel(
-                rng_key,
-                state,
-                logdensity_fn,
-                step_size,
-                inverse_mass_matrix,
-                num_integration_steps,
-            )
+    def init_fn(position: ArrayLikeTree, rng_key=None):
+        del rng_key
+        return init(position, logdensity_fn)
+
+    def step_fn(rng_key: PRNGKey, state):
+        return kernel(
+            rng_key,
+            state,
+            logdensity_fn,
+            step_size,
+            inverse_mass_matrix,
+            num_integration_steps,
+        )
 
-        return SamplingAlgorithm(init_fn, step_fn)
+    return SamplingAlgorithm(init_fn, step_fn)
 
 
 def hmc_proposal(
     integrator: Callable,
     kinetic_energy: metrics.KineticEnergy,
     step_size: Union[float, ArrayLikeTree],
     num_integration_steps: int = 1,
```

### Comparing `blackjax-1.1.1/blackjax/mcmc/integrators.py` & `blackjax-1.2.0/blackjax/mcmc/integrators.py`

 * *Files identical despite different names*

### Comparing `blackjax-1.1.1/blackjax/mcmc/mala.py` & `blackjax-1.2.0/blackjax/mcmc/mala.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 import jax.numpy as jnp
 
 import blackjax.mcmc.diffusions as diffusions
 import blackjax.mcmc.proposal as proposal
 from blackjax.base import SamplingAlgorithm
 from blackjax.types import ArrayLikeTree, ArrayTree, PRNGKey
 
-__all__ = ["MALAState", "MALAInfo", "init", "build_kernel", "mala"]
+__all__ = ["MALAState", "MALAInfo", "init", "build_kernel", "as_top_level_api"]
 
 
 class MALAState(NamedTuple):
     """State of the MALA algorithm.
 
     The MALA algorithm takes one position of the chain and returns another
     position. In order to make computations more efficient, we also store
@@ -75,23 +75,23 @@
     information about the transition.
 
     """
 
     def transition_energy(state, new_state, step_size):
         """Transition energy to go from `state` to `new_state`"""
         theta = jax.tree_util.tree_map(
-            lambda new_x, x, g: new_x - x - step_size * g,
-            new_state.position,
+            lambda x, new_x, g: x - new_x - step_size * g,
             state.position,
-            state.logdensity_grad,
+            new_state.position,
+            new_state.logdensity_grad,
         )
         theta_dot = jax.tree_util.tree_reduce(
             operator.add, jax.tree_util.tree_map(lambda x: jnp.sum(x * x), theta)
         )
-        return -state.logdensity + 0.25 * (1.0 / step_size) * theta_dot
+        return -new_state.logdensity + 0.25 * (1.0 / step_size) * theta_dot
 
     compute_acceptance_ratio = proposal.compute_asymmetric_acceptance_ratio(
         transition_energy
     )
     sample_proposal = proposal.static_binomial_sampling
 
     def kernel(
@@ -113,15 +113,18 @@
         info = MALAInfo(p_accept, do_accept)
 
         return accepted_state, info
 
     return kernel
 
 
-class mala:
+def as_top_level_api(
+    logdensity_fn: Callable,
+    step_size: float,
+) -> SamplingAlgorithm:
     """Implements the (basic) user interface for the MALA kernel.
 
     The general mala kernel builder (:meth:`blackjax.mcmc.mala.build_kernel`, alias `blackjax.mala.build_kernel`) can be
     cumbersome to manipulate. Since most users only need to specify the kernel
     parameters at initialization time, we provide a helper function that
     specializes the general kernel.
 
@@ -163,25 +166,17 @@
 
     Returns
     -------
     A ``SamplingAlgorithm``.
 
     """
 
-    init = staticmethod(init)
-    build_kernel = staticmethod(build_kernel)
+    kernel = build_kernel()
 
-    def __new__(  # type: ignore[misc]
-        cls,
-        logdensity_fn: Callable,
-        step_size: float,
-    ) -> SamplingAlgorithm:
-        kernel = cls.build_kernel()
-
-        def init_fn(position: ArrayLikeTree, rng_key=None):
-            del rng_key
-            return cls.init(position, logdensity_fn)
+    def init_fn(position: ArrayLikeTree, rng_key=None):
+        del rng_key
+        return init(position, logdensity_fn)
 
-        def step_fn(rng_key: PRNGKey, state):
-            return kernel(rng_key, state, logdensity_fn, step_size)
+    def step_fn(rng_key: PRNGKey, state):
+        return kernel(rng_key, state, logdensity_fn, step_size)
 
-        return SamplingAlgorithm(init_fn, step_fn)
+    return SamplingAlgorithm(init_fn, step_fn)
```

### Comparing `blackjax-1.1.1/blackjax/mcmc/marginal_latent_gaussian.py` & `blackjax-1.2.0/blackjax/mcmc/marginal_latent_gaussian.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,15 +18,21 @@
 import jax.numpy as jnp
 import jax.scipy.linalg as linalg
 
 from blackjax.base import SamplingAlgorithm
 from blackjax.mcmc.proposal import static_binomial_sampling
 from blackjax.types import Array, PRNGKey
 
-__all__ = ["MarginalState", "MarginalInfo", "init", "build_kernel", "mgrad_gaussian"]
+__all__ = [
+    "MarginalState",
+    "MarginalInfo",
+    "init",
+    "build_kernel",
+    "as_top_level_api",
+]
 
 
 # [TODO](https://github.com/blackjax-devs/blackjax/issues/237)
 class MarginalState(NamedTuple):
     """State of the RMH chain.
 
     x
@@ -202,15 +208,21 @@
         do_accept, p_accept, _ = info
         info = MarginalInfo(p_accept, do_accept, proposed_state)
         return accepted_state, info
 
     return kernel
 
 
-class mgrad_gaussian:
+def as_top_level_api(
+    logdensity_fn: Callable,
+    covariance: Optional[Array] = None,
+    mean: Optional[Array] = None,
+    cov_svd: Optional[CovarianceSVD] = None,
+    step_size: float = 1.0,
+) -> SamplingAlgorithm:
     """Implements the marginal sampler for latent Gaussian model of :cite:p:`titsias2018auxiliary`.
 
     It uses a first order approximation to the log_likelihood of a model with Gaussian prior.
     Interestingly, the only parameter that needs calibrating is the "step size" delta,
     which can be done very efficiently.
     Calibrating it to have an acceptance rate of roughly 50% is a good starting point.
 
@@ -243,45 +255,32 @@
 
     Returns
     -------
     A ``SamplingAlgorithm``.
 
     """
 
-    init = staticmethod(init)
-    build_kernel = staticmethod(build_kernel)
+    if cov_svd is None:
+        if covariance is None:
+            raise ValueError("Either covariance or cov_svd must be provided.")
+        cov_svd = svd_from_covariance(covariance)
 
-    def __new__(  # type: ignore[misc]
-        cls,
-        logdensity_fn: Callable,
-        covariance: Optional[Array] = None,
-        mean: Optional[Array] = None,
-        cov_svd: Optional[CovarianceSVD] = None,
-        step_size: float = 1.0,
-    ) -> SamplingAlgorithm:
-        if cov_svd is None:
-            if covariance is None:
-                raise ValueError("Either covariance or cov_svd must be provided.")
-            cov_svd = svd_from_covariance(covariance)
-
-        U, Gamma, U_t = cov_svd
-
-        if mean is not None:
-            logdensity_fn = generate_mean_shifted_logprob(
-                logdensity_fn, mean, covariance
-            )
-
-        kernel = cls.build_kernel(cov_svd)
-
-        def init_fn(position: Array, rng_key=None):
-            del rng_key
-            return init(position, logdensity_fn, U_t)
-
-        def step_fn(rng_key: PRNGKey, state):
-            return kernel(
-                rng_key,
-                state,
-                logdensity_fn,
-                step_size,
-            )
+    U, Gamma, U_t = cov_svd
+
+    if mean is not None:
+        logdensity_fn = generate_mean_shifted_logprob(logdensity_fn, mean, covariance)
+
+    kernel = build_kernel(cov_svd)
+
+    def init_fn(position: Array, rng_key=None):
+        del rng_key
+        return init(position, logdensity_fn, U_t)
+
+    def step_fn(rng_key: PRNGKey, state):
+        return kernel(
+            rng_key,
+            state,
+            logdensity_fn,
+            step_size,
+        )
 
-        return SamplingAlgorithm(init_fn, step_fn)
+    return SamplingAlgorithm(init_fn, step_fn)
```

### Comparing `blackjax-1.1.1/blackjax/mcmc/mclmc.py` & `blackjax-1.2.0/blackjax/mcmc/mclmc.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 from jax.random import normal
 
 from blackjax.base import SamplingAlgorithm
 from blackjax.mcmc.integrators import IntegratorState, isokinetic_mclachlan
 from blackjax.types import ArrayLike, PRNGKey
 from blackjax.util import generate_unit_vector, pytree_size
 
-__all__ = ["MCLMCInfo", "init", "build_kernel", "mclmc"]
+__all__ = ["MCLMCInfo", "init", "build_kernel", "as_top_level_api"]
 
 
 class MCLMCInfo(NamedTuple):
     """
     Additional information on the MCLMC transition.
 
     logdensity
@@ -99,15 +99,20 @@
             energy_change=kinetic_change - logdensity + state.logdensity,
             kinetic_change=kinetic_change,
         )
 
     return kernel
 
 
-class mclmc:
+def as_top_level_api(
+    logdensity_fn: Callable,
+    L,
+    step_size,
+    integrator=isokinetic_mclachlan,
+) -> SamplingAlgorithm:
     """The general mclmc kernel builder (:meth:`blackjax.mcmc.mclmc.build_kernel`, alias `blackjax.mclmc.build_kernel`) can be
     cumbersome to manipulate. Since most users only need to specify the kernel
     parameters at initialization time, we provide a helper function that
     specializes the general kernel.
 
     We also add the general kernel and state generator as an attribute to this class so
     users only need to pass `blackjax.mclmc` to SMC, adaptation, etc. algorithms.
@@ -146,33 +151,23 @@
         an integrator. We recommend using the default here.
 
     Returns
     -------
     A ``SamplingAlgorithm``.
     """
 
-    init = staticmethod(init)
-    build_kernel = staticmethod(build_kernel)
+    kernel = build_kernel(logdensity_fn, integrator)
 
-    def __new__(  # type: ignore[misc]
-        cls,
-        logdensity_fn: Callable,
-        L,
-        step_size,
-        integrator=isokinetic_mclachlan,
-    ) -> SamplingAlgorithm:
-        kernel = cls.build_kernel(logdensity_fn, integrator)
+    def init_fn(position: ArrayLike, rng_key: PRNGKey):
+        return init(position, logdensity_fn, rng_key)
 
-        def init_fn(position: ArrayLike, rng_key: PRNGKey):
-            return cls.init(position, logdensity_fn, rng_key)
+    def update_fn(rng_key, state):
+        return kernel(rng_key, state, L, step_size)
 
-        def update_fn(rng_key, state):
-            return kernel(rng_key, state, L, step_size)
-
-        return SamplingAlgorithm(init_fn, update_fn)
+    return SamplingAlgorithm(init_fn, update_fn)
 
 
 def partially_refresh_momentum(momentum, rng_key, step_size, L):
     """Adds a small noise to momentum and normalizes.
 
     Parameters
     ----------
```

### Comparing `blackjax-1.1.1/blackjax/mcmc/metrics.py` & `blackjax-1.2.0/blackjax/mcmc/metrics.py`

 * *Files identical despite different names*

### Comparing `blackjax-1.1.1/blackjax/mcmc/nuts.py` & `blackjax-1.2.0/blackjax/mcmc/nuts.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 import blackjax.mcmc.metrics as metrics
 import blackjax.mcmc.proposal as proposal
 import blackjax.mcmc.termination as termination
 import blackjax.mcmc.trajectory as trajectory
 from blackjax.base import SamplingAlgorithm
 from blackjax.types import ArrayLikeTree, ArrayTree, PRNGKey
 
-__all__ = ["NUTSInfo", "init", "build_kernel", "nuts"]
+__all__ = ["NUTSInfo", "init", "build_kernel", "as_top_level_api"]
 
 
 init = hmc.init
 
 
 class NUTSInfo(NamedTuple):
     """Additional information on the NUTS transition.
@@ -143,15 +143,23 @@
             proposal.position, proposal.logdensity, proposal.logdensity_grad
         )
         return proposal, info
 
     return kernel
 
 
-class nuts:
+def as_top_level_api(
+    logdensity_fn: Callable,
+    step_size: float,
+    inverse_mass_matrix: metrics.MetricTypes,
+    *,
+    max_num_doublings: int = 10,
+    divergence_threshold: int = 1000,
+    integrator: Callable = integrators.velocity_verlet,
+) -> SamplingAlgorithm:
     """Implements the (basic) user interface for the nuts kernel.
 
     Examples
     --------
 
     A new NUTS kernel can be initialized and used with the following code:
 
@@ -198,45 +206,31 @@
         (algorithm parameter) The symplectic integrator to use to integrate the trajectory.
 
     Returns
     -------
     A ``SamplingAlgorithm``.
 
     """
+    kernel = build_kernel(integrator, divergence_threshold)
 
-    init = staticmethod(hmc.init)
-    build_kernel = staticmethod(build_kernel)
-
-    def __new__(  # type: ignore[misc]
-        cls,
-        logdensity_fn: Callable,
-        step_size: float,
-        inverse_mass_matrix: metrics.MetricTypes,
-        *,
-        max_num_doublings: int = 10,
-        divergence_threshold: int = 1000,
-        integrator: Callable = integrators.velocity_verlet,
-    ) -> SamplingAlgorithm:
-        kernel = cls.build_kernel(integrator, divergence_threshold)
-
-        def init_fn(position: ArrayLikeTree, rng_key=None):
-            del rng_key
-            return cls.init(position, logdensity_fn)
-
-        def step_fn(rng_key: PRNGKey, state):
-            return kernel(
-                rng_key,
-                state,
-                logdensity_fn,
-                step_size,
-                inverse_mass_matrix,
-                max_num_doublings,
-            )
+    def init_fn(position: ArrayLikeTree, rng_key=None):
+        del rng_key
+        return init(position, logdensity_fn)
+
+    def step_fn(rng_key: PRNGKey, state):
+        return kernel(
+            rng_key,
+            state,
+            logdensity_fn,
+            step_size,
+            inverse_mass_matrix,
+            max_num_doublings,
+        )
 
-        return SamplingAlgorithm(init_fn, step_fn)
+    return SamplingAlgorithm(init_fn, step_fn)
 
 
 def iterative_nuts_proposal(
     integrator: Callable,
     kinetic_energy: metrics.KineticEnergy,
     uturn_check_fn: metrics.CheckTurning,
     max_num_expansions: int = 10,
```

### Comparing `blackjax-1.1.1/blackjax/mcmc/periodic_orbital.py` & `blackjax-1.2.0/blackjax/mcmc/periodic_orbital.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 import jax.numpy as jnp
 
 import blackjax.mcmc.integrators as integrators
 import blackjax.mcmc.metrics as metrics
 from blackjax.base import SamplingAlgorithm
 from blackjax.types import Array, ArrayLikeTree, ArrayTree, PRNGKey
 
-__all__ = ["PeriodicOrbitalState", "init", "build_kernel", "orbital_hmc"]
+__all__ = ["PeriodicOrbitalState", "init", "build_kernel", "as_top_level_api"]
 
 
 class PeriodicOrbitalState(NamedTuple):
     """State of the periodic orbital algorithm.
 
     The periodic orbital algorithm takes one orbit with weights,
     samples from the points on that orbit according to their weights
@@ -213,15 +213,22 @@
         proposal, info = proposal_generator(direction, augmented_state)
 
         return proposal, info
 
     return kernel
 
 
-class orbital_hmc:
+def as_top_level_api(
+    logdensity_fn: Callable,
+    step_size: float,
+    inverse_mass_matrix: Array,  # assume momentum is always Gaussian
+    period: int,
+    *,
+    bijection: Callable = integrators.velocity_verlet,
+) -> SamplingAlgorithm:
     """Implements the (basic) user interface for the Periodic orbital MCMC kernel.
 
     Each iteration of the periodic orbital MCMC outputs ``period`` weighted samples from
     a single Hamiltonian orbit connecting the previous sample and momentum (latent) variable
     with precision matrix ``inverse_mass_matrix``, evaluated using the ``bijection`` as an
     integrator with discretization parameter ``step_size``.
 
@@ -257,44 +264,31 @@
     bijection
         (algorithm parameter) The symplectic integrator to use to build the orbit.
 
     Returns
     -------
     A ``SamplingAlgorithm``.
     """
+    kernel = build_kernel(bijection)
 
-    init = staticmethod(init)
-    build_kernel = staticmethod(build_kernel)
-
-    def __new__(  # type: ignore[misc]
-        cls,
-        logdensity_fn: Callable,
-        step_size: float,
-        inverse_mass_matrix: Array,  # assume momentum is always Gaussian
-        period: int,
-        *,
-        bijection: Callable = integrators.velocity_verlet,
-    ) -> SamplingAlgorithm:
-        kernel = cls.build_kernel(bijection)
-
-        def init_fn(position: ArrayLikeTree, rng_key=None):
-            del rng_key
-            return cls.init(position, logdensity_fn, period)
-
-        def step_fn(rng_key: PRNGKey, state):
-            return kernel(
-                rng_key,
-                state,
-                logdensity_fn,
-                step_size,
-                inverse_mass_matrix,
-                period,
-            )
+    def init_fn(position: ArrayLikeTree, rng_key=None):
+        del rng_key
+        return init(position, logdensity_fn, period)
+
+    def step_fn(rng_key: PRNGKey, state):
+        return kernel(
+            rng_key,
+            state,
+            logdensity_fn,
+            step_size,
+            inverse_mass_matrix,
+            period,
+        )
 
-        return SamplingAlgorithm(init_fn, step_fn)
+    return SamplingAlgorithm(init_fn, step_fn)
 
 
 def periodic_orbital_proposal(
     bijection: Callable,
     kinetic_energy_fn: Callable,
     period: int,
     step_size: float,
```

### Comparing `blackjax-1.1.1/blackjax/mcmc/proposal.py` & `blackjax-1.2.0/blackjax/mcmc/proposal.py`

 * *Files identical despite different names*

### Comparing `blackjax-1.1.1/blackjax/mcmc/random_walk.py` & `blackjax-1.2.0/blackjax/mcmc/random_walk.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,16 +76,17 @@
     "build_irmh",
     "build_rmh",
     "RWInfo",
     "RWState",
     "rmh_proposal",
     "build_rmh_transition_energy",
     "additive_step_random_walk",
-    "irmh",
-    "rmh",
+    "irmh_as_top_level_api",
+    "rmh_as_top_level_api",
+    "normal_random_walk",
 ]
 
 
 def normal(sigma: Array) -> Callable:
     """Normal Random Walk proposal.
 
     Propose a new position such that its distance to the current position is
@@ -178,15 +179,33 @@
 
         inner_kernel = build_rmh()
         return inner_kernel(rng_key, state, logdensity_fn, proposal_generator)
 
     return kernel
 
 
-class additive_step_random_walk:
+def normal_random_walk(logdensity_fn: Callable, sigma):
+    """
+    Parameters
+    ----------
+    logdensity_fn
+        The log density probability density function from which we wish to sample.
+    sigma
+        The value of the covariance matrix of the gaussian proposal distribution.
+
+    Returns
+    -------
+         A ``SamplingAlgorithm``.
+    """
+    return additive_step_random_walk(logdensity_fn, normal(sigma))
+
+
+def additive_step_random_walk(
+    logdensity_fn: Callable, random_step: Callable
+) -> SamplingAlgorithm:
     """Implements the user interface for the Additive Step RMH
 
     Examples
     --------
 
     A new kernel can be initialized and used with the following code:
 
@@ -214,47 +233,24 @@
         which will be added to the current position to obtain a new position. Must be symmetric
         to maintain detailed balance. This means that P(step|position) = P(-step | position+step)
 
     Returns
     -------
     A ``SamplingAlgorithm``.
     """
+    kernel = build_additive_step()
 
-    init = staticmethod(init)
-    build_kernel = staticmethod(build_additive_step)
-
-    @classmethod
-    def normal_random_walk(cls, logdensity_fn: Callable, sigma):
-        """
-        Parameters
-        ----------
-        logdensity_fn
-            The log density probability density function from which we wish to sample.
-        sigma
-            The value of the covariance matrix of the gaussian proposal distribution.
-
-        Returns
-        -------
-             A ``SamplingAlgorithm``.
-        """
-        return cls(logdensity_fn, normal(sigma))
-
-    def __new__(  # type: ignore[misc]
-        cls, logdensity_fn: Callable, random_step: Callable
-    ) -> SamplingAlgorithm:
-        kernel = cls.build_kernel()
-
-        def init_fn(position: ArrayLikeTree, rng_key=None):
-            del rng_key
-            return cls.init(position, logdensity_fn)
+    def init_fn(position: ArrayLikeTree, rng_key=None):
+        del rng_key
+        return init(position, logdensity_fn)
 
-        def step_fn(rng_key: PRNGKey, state):
-            return kernel(rng_key, state, logdensity_fn, random_step)
+    def step_fn(rng_key: PRNGKey, state):
+        return kernel(rng_key, state, logdensity_fn, random_step)
 
-        return SamplingAlgorithm(init_fn, step_fn)
+    return SamplingAlgorithm(init_fn, step_fn)
 
 
 def build_irmh() -> Callable:
     """
     Build an Independent Random Walk Rosenbluth-Metropolis-Hastings kernel. This implies
     that the proposal distribution does not depend on the particle being mutated :cite:p:`wang2022exact`.
 
@@ -293,15 +289,19 @@
         return inner_kernel(
             rng_key, state, logdensity_fn, proposal_generator, proposal_logdensity_fn
         )
 
     return kernel
 
 
-class irmh:
+def irmh_as_top_level_api(
+    logdensity_fn: Callable,
+    proposal_distribution: Callable,
+    proposal_logdensity_fn: Optional[Callable] = None,
+) -> SamplingAlgorithm:
     """Implements the (basic) user interface for the independent RMH.
 
     Examples
     --------
 
     A new kernel can be initialized and used with the following code:
 
@@ -330,40 +330,30 @@
         to obtain a given proposal knowing the current state. If it is not
         provided we assume the proposal is symmetric.
     Returns
     -------
     A ``SamplingAlgorithm``.
 
     """
+    kernel = build_irmh()
 
-    init = staticmethod(init)
-    build_kernel = staticmethod(build_irmh)
-
-    def __new__(  # type: ignore[misc]
-        cls,
-        logdensity_fn: Callable,
-        proposal_distribution: Callable,
-        proposal_logdensity_fn: Optional[Callable] = None,
-    ) -> SamplingAlgorithm:
-        kernel = cls.build_kernel()
-
-        def init_fn(position: ArrayLikeTree, rng_key=None):
-            del rng_key
-            return cls.init(position, logdensity_fn)
-
-        def step_fn(rng_key: PRNGKey, state):
-            return kernel(
-                rng_key,
-                state,
-                logdensity_fn,
-                proposal_distribution,
-                proposal_logdensity_fn,
-            )
+    def init_fn(position: ArrayLikeTree, rng_key=None):
+        del rng_key
+        return init(position, logdensity_fn)
+
+    def step_fn(rng_key: PRNGKey, state):
+        return kernel(
+            rng_key,
+            state,
+            logdensity_fn,
+            proposal_distribution,
+            proposal_logdensity_fn,
+        )
 
-        return SamplingAlgorithm(init_fn, step_fn)
+    return SamplingAlgorithm(init_fn, step_fn)
 
 
 def build_rmh():
     """Build a Rosenbluth-Metropolis-Hastings kernel.
 
     Returns
     -------
@@ -416,15 +406,19 @@
         )
         new_state, do_accept, p_accept = proposal_generator(rng_key, state)
         return new_state, RWInfo(p_accept, do_accept, new_state)
 
     return kernel
 
 
-class rmh:
+def rmh_as_top_level_api(
+    logdensity_fn: Callable,
+    proposal_generator: Callable[[PRNGKey, ArrayLikeTree], ArrayTree],
+    proposal_logdensity_fn: Optional[Callable[[ArrayLikeTree], ArrayTree]] = None,
+) -> SamplingAlgorithm:
     """Implements the user interface for the RMH.
 
     Examples
     --------
 
     A new kernel can be initialized and used with the following code:
 
@@ -452,40 +446,30 @@
          P(x_t|x_t-1) is not equal to P(x_t-1|x_t), then this parameter must be not None in order to apply
          the Metropolis-Hastings correction for detailed balance.
 
     Returns
     -------
     A ``SamplingAlgorithm``.
     """
+    kernel = build_rmh()
 
-    init = staticmethod(init)
-    build_kernel = staticmethod(build_rmh)
-
-    def __new__(  # type: ignore[misc]
-        cls,
-        logdensity_fn: Callable,
-        proposal_generator: Callable[[PRNGKey, ArrayLikeTree], ArrayTree],
-        proposal_logdensity_fn: Optional[Callable[[ArrayLikeTree], ArrayTree]] = None,
-    ) -> SamplingAlgorithm:
-        kernel = cls.build_kernel()
-
-        def init_fn(position: ArrayLikeTree, rng_key=None):
-            del rng_key
-            return cls.init(position, logdensity_fn)
-
-        def step_fn(rng_key: PRNGKey, state):
-            return kernel(
-                rng_key,
-                state,
-                logdensity_fn,
-                proposal_generator,
-                proposal_logdensity_fn,
-            )
+    def init_fn(position: ArrayLikeTree, rng_key=None):
+        del rng_key
+        return init(position, logdensity_fn)
+
+    def step_fn(rng_key: PRNGKey, state):
+        return kernel(
+            rng_key,
+            state,
+            logdensity_fn,
+            proposal_generator,
+            proposal_logdensity_fn,
+        )
 
-        return SamplingAlgorithm(init_fn, step_fn)
+    return SamplingAlgorithm(init_fn, step_fn)
 
 
 def build_rmh_transition_energy(proposal_logdensity_fn: Optional[Callable]) -> Callable:
     if proposal_logdensity_fn is None:
 
         def transition_energy(prev_state, new_state):
             return -new_state.logdensity
```

### Comparing `blackjax-1.1.1/blackjax/mcmc/rmhmc.py` & `blackjax-1.2.0/blackjax/mcmc/rmhmc.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,22 +16,30 @@
 
 import blackjax.mcmc.integrators as integrators
 import blackjax.mcmc.metrics as metrics
 from blackjax.base import SamplingAlgorithm
 from blackjax.mcmc import hmc
 from blackjax.types import ArrayTree, PRNGKey
 
-__all__ = ["init", "build_kernel", "rmhmc"]
+__all__ = ["init", "build_kernel", "as_top_level_api"]
 
 
 init = hmc.init
 build_kernel = hmc.build_kernel
 
 
-class rmhmc:
+def as_top_level_api(
+    logdensity_fn: Callable,
+    step_size: float,
+    mass_matrix: Union[metrics.Metric, Callable],
+    num_integration_steps: int,
+    *,
+    divergence_threshold: int = 1000,
+    integrator: Callable = integrators.implicit_midpoint,
+) -> SamplingAlgorithm:
     """A Riemannian Manifold Hamiltonian Monte Carlo kernel
 
     Of note, this kernel is simply an alias of the ``hmc`` kernel with a
     different choice of default integrator (``implicit_midpoint`` instead of
     ``velocity_verlet``) since RMHMC is typically used for Hamiltonian systems
     that are not separable.
 
@@ -58,38 +66,24 @@
         (algorithm parameter) The symplectic integrator to use to integrate the
         trajectory.
 
     Returns
     -------
     A ``SamplingAlgorithm``.
     """
+    kernel = build_kernel(integrator, divergence_threshold)
 
-    init = staticmethod(init)
-    build_kernel = staticmethod(build_kernel)
+    def init_fn(position: ArrayTree, rng_key=None):
+        del rng_key
+        return init(position, logdensity_fn)
+
+    def step_fn(rng_key: PRNGKey, state):
+        return kernel(
+            rng_key,
+            state,
+            logdensity_fn,
+            step_size,
+            mass_matrix,
+            num_integration_steps,
+        )
 
-    def __new__(  # type: ignore[misc]
-        cls,
-        logdensity_fn: Callable,
-        step_size: float,
-        mass_matrix: Union[metrics.Metric, Callable],
-        num_integration_steps: int,
-        *,
-        divergence_threshold: int = 1000,
-        integrator: Callable = integrators.implicit_midpoint,
-    ) -> SamplingAlgorithm:
-        kernel = cls.build_kernel(integrator, divergence_threshold)
-
-        def init_fn(position: ArrayTree, rng_key=None):
-            del rng_key
-            return cls.init(position, logdensity_fn)
-
-        def step_fn(rng_key: PRNGKey, state):
-            return kernel(
-                rng_key,
-                state,
-                logdensity_fn,
-                step_size,
-                mass_matrix,
-                num_integration_steps,
-            )
-
-        return SamplingAlgorithm(init_fn, step_fn)
+    return SamplingAlgorithm(init_fn, step_fn)
```

### Comparing `blackjax-1.1.1/blackjax/mcmc/termination.py` & `blackjax-1.2.0/blackjax/mcmc/termination.py`

 * *Files identical despite different names*

### Comparing `blackjax-1.1.1/blackjax/mcmc/trajectory.py` & `blackjax-1.2.0/blackjax/mcmc/trajectory.py`

 * *Files 2% similar despite different names*

```diff
@@ -197,25 +197,25 @@
             Initial energy H0 of the HMC step (not to confused with the initial
             energy of the subtree)
 
         """
 
         def do_keep_integrating(loop_state):
             """Decide whether we should continue integrating the trajectory"""
-            _, integration_state, (is_diverging, has_terminated) = loop_state
+            integration_state, (is_diverging, has_terminated) = loop_state
             return (
                 (integration_state.step < max_num_steps)
                 & ~has_terminated
                 & ~is_diverging
             )
 
         def add_one_state(loop_state):
-            rng_key, integration_state, _ = loop_state
+            integration_state, _ = loop_state
             step, proposal, trajectory, termination_state = integration_state
-            rng_key, proposal_key = jax.random.split(rng_key)
+            proposal_key = jax.random.fold_in(rng_key, step)
 
             new_state = integrator(trajectory.rightmost_state, direction * step_size)
             new_proposal = generate_proposal(initial_energy, new_state)
             is_diverging = -new_proposal.weight > divergence_threshold
 
             # At step 0, we always accept the proposal, since we
             # take one step to get the leftmost state of the tree.
@@ -242,33 +242,33 @@
             new_integration_state = DynamicIntegrationState(
                 step + 1,
                 sampled_proposal,
                 new_trajectory,
                 new_termination_state,
             )
 
-            return (rng_key, new_integration_state, (is_diverging, has_terminated))
+            return (new_integration_state, (is_diverging, has_terminated))
 
         proposal_placeholder = generate_proposal(initial_energy, initial_state)
         trajectory_placeholder = Trajectory(
             initial_state, initial_state, initial_state.momentum, 0
         )
         integration_state_placeholder = DynamicIntegrationState(
             0,
             proposal_placeholder,
             trajectory_placeholder,
             termination_state,
         )
 
-        _, integration_state, (is_diverging, has_terminated) = jax.lax.while_loop(
+        new_integration_state, (is_diverging, has_terminated) = jax.lax.while_loop(
             do_keep_integrating,
             add_one_state,
-            (rng_key, integration_state_placeholder, (False, False)),
+            (integration_state_placeholder, (False, False)),
         )
-        step, proposal, trajectory, termination_state = integration_state
+        _, proposal, trajectory, termination_state = new_integration_state
 
         # In the while_loop we always extend on the right most direction.
         new_trajectory = jax.lax.cond(
             direction > 0,
             lambda _: trajectory,
             lambda _: Trajectory(
                 trajectory.rightmost_state,
@@ -381,15 +381,15 @@
                 initial_state,
                 direction,
                 tree_depth - 1,
                 step_size,
                 initial_energy,
             )
             # Note that is_diverging and is_turning is inplace updated
-            if ~is_diverging & ~is_turning:
+            if (not is_diverging) & (not is_turning):
                 start_state = jax.lax.cond(
                     direction > 0,
                     lambda _: trajectory.rightmost_state,
                     lambda _: trajectory.leftmost_state,
                     operand=None,
                 )
                 (
@@ -407,15 +407,15 @@
                     initial_energy,
                 )
                 left_trajectory, right_trajectory = reorder_trajectories(
                     direction, trajectory, new_trajectory
                 )
                 trajectory = merge_trajectories(left_trajectory, right_trajectory)
 
-                if ~is_turning:
+                if not is_turning:
                     is_turning = uturn_check_fn(
                         trajectory.leftmost_state.momentum,
                         trajectory.rightmost_state.momentum,
                         trajectory.momentum_sum,
                     )
                     if use_robust_uturn_check & (tree_depth - 1 > 0):
                         momentum_sum_left = jax.tree_util.tree_map(
@@ -492,16 +492,15 @@
         A function that runs the symplectic integrators and returns a new proposal
         and the integrated trajectory.
     uturn_check_fn
         Function used to check the U-Turn criterion.
     step_size
         The step size used by the symplectic integrator.
     max_num_expansions
-        The maximum number of trajectory expansions until the proposal is
-        returned.
+        The maximum number of trajectory expansions until the proposal is returned.
     rate
         The rate of the geometrical expansion. Typically 2 in NUTS, this is why
         the literature often refers to "tree doubling".
 
     """
     proposal_sampler = progressive_biased_sampling
 
@@ -509,15 +508,15 @@
         rng_key: PRNGKey,
         initial_expansion_state: DynamicExpansionState,
         initial_energy: float,
         step_size: float,
     ):
         def do_keep_expanding(loop_state) -> bool:
             """Determine whether we need to keep expanding the trajectory."""
-            _, expansion_state, (is_diverging, is_turning) = loop_state
+            expansion_state, (is_diverging, is_turning) = loop_state
             return (
                 (expansion_state.step < max_num_expansions)
                 & ~is_diverging
                 & ~is_turning
             )
 
         def expand_once(loop_state):
@@ -527,20 +526,19 @@
             starting from the leftmost or rightmost point of the current
             trajectory that is twice as long as the current trajectory.
 
             Once that is done, possibly update the current proposal with that of
             the subtrajectory.
 
             """
-            rng_key, expansion_state, _ = loop_state
+            expansion_state, _ = loop_state
             step, proposal, trajectory, termination_state = expansion_state
 
-            rng_key, direction_key, trajectory_key, proposal_key = jax.random.split(
-                rng_key, 4
-            )
+            subkey = jax.random.fold_in(rng_key, step)
+            direction_key, trajectory_key, proposal_key = jax.random.split(subkey, 3)
 
             # create new subtrajectory that is twice as long as the current
             # trajectory.
             direction = jnp.where(jax.random.bernoulli(direction_key), 1, -1)
             start_state = jax.lax.cond(
                 direction > 0,
                 lambda _: trajectory.rightmost_state,
@@ -604,20 +602,20 @@
             )
 
             new_state = DynamicExpansionState(
                 step + 1, updated_proposal, merged_trajectory, termination_state
             )
             info = (is_diverging, is_turning_subtree | is_turning)
 
-            return (rng_key, new_state, info)
+            return (new_state, info)
 
-        _, expansion_state, (is_diverging, is_turning) = jax.lax.while_loop(
+        expansion_state, (is_diverging, is_turning) = jax.lax.while_loop(
             do_keep_expanding,
             expand_once,
-            (rng_key, initial_expansion_state, (False, False)),
+            (initial_expansion_state, (False, False)),
         )
 
         return expansion_state, (is_diverging, is_turning)
 
     return expand
```

### Comparing `blackjax-1.1.1/blackjax/optimizers/dual_averaging.py` & `blackjax-1.2.0/blackjax/optimizers/dual_averaging.py`

 * *Files identical despite different names*

### Comparing `blackjax-1.1.1/blackjax/optimizers/lbfgs.py` & `blackjax-1.2.0/blackjax/optimizers/lbfgs.py`

 * *Files 1% similar despite different names*

```diff
@@ -135,15 +135,15 @@
 
     # Unravel optimization path history.
     history = LBFGSHistory(
         x=unravel_fn_mapped(history_raveled.x),
         f=history_raveled.f,
         g=unravel_fn_mapped(history_raveled.g),
         alpha=unravel_fn_mapped(history_raveled.alpha),
-        update_mask=jax.tree_map(
+        update_mask=jax.tree.map(
             lambda x: x.astype(history_raveled.update_mask.dtype),
             unravel_fn_mapped(history_raveled.update_mask.astype(x0_raveled.dtype)),
         ),
     )
 
     return last_step, history
 
@@ -226,15 +226,15 @@
         update_mask=jnp.zeros_like(x0, dtype=bool),
     )
 
     ((last_step, _), _), history = lax.scan(
         scan_body, ((init_step, initial_history), True), jnp.arange(maxiter)
     )
     # Append initial state to history.
-    history = jax.tree_map(
+    history = jax.tree.map(
         lambda x, y: jnp.concatenate([x[None, ...], y], axis=0),
         initial_history,
         history,
     )
     return last_step, history
```

### Comparing `blackjax-1.1.1/blackjax/progress_bar.py` & `blackjax-1.2.0/blackjax/progress_bar.py`

 * *Files 16% similar despite different names*

```diff
@@ -12,76 +12,60 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Progress bar decorators for use with step functions.
 Adapted from Jeremie Coullon's blog post :cite:p:`progress_bar`.
 """
 from fastprogress.fastprogress import progress_bar
 from jax import lax
-from jax.experimental import host_callback
+from jax.experimental import io_callback
 
 
 def progress_bar_scan(num_samples, print_rate=None):
     "Progress bar for a JAX scan"
     progress_bars = {}
 
     if print_rate is None:
         if num_samples > 20:
             print_rate = int(num_samples / 20)
         else:
             print_rate = 1  # if you run the sampler for less than 20 iterations
 
-    def _define_bar(arg, transform, device):
+    def _define_bar(arg):
+        del arg
         progress_bars[0] = progress_bar(range(num_samples))
         progress_bars[0].update(0)
 
-    def _update_bar(arg, transform, device):
-        progress_bars[0].update_bar(arg)
+    def _update_bar(arg):
+        progress_bars[0].update_bar(arg + 1)
+
+    def _close_bar(arg):
+        del arg
+        progress_bars[0].on_iter_end()
 
     def _update_progress_bar(iter_num):
         "Updates progress bar of a JAX scan or loop"
         _ = lax.cond(
             iter_num == 0,
-            lambda _: host_callback.id_tap(
-                _define_bar, iter_num, result=iter_num, tap_with_device=True
-            ),
-            lambda _: iter_num,
+            lambda _: io_callback(_define_bar, None, iter_num),
+            lambda _: None,
             operand=None,
         )
 
         _ = lax.cond(
             # update every multiple of `print_rate` except at the end
-            (iter_num % print_rate == 0),
-            lambda _: host_callback.id_tap(
-                _update_bar, iter_num, result=iter_num, tap_with_device=True
-            ),
-            lambda _: iter_num,
+            (iter_num % print_rate == 0) | (iter_num == (num_samples - 1)),
+            lambda _: io_callback(_update_bar, None, iter_num),
+            lambda _: None,
             operand=None,
         )
 
         _ = lax.cond(
-            # update by `remainder`
-            iter_num == num_samples - 1,
-            lambda _: host_callback.id_tap(
-                _update_bar, num_samples, result=iter_num, tap_with_device=True
-            ),
-            lambda _: iter_num,
-            operand=None,
-        )
-
-    def _close_bar(arg, transform, device):
-        progress_bars[0].on_iter_end()
-        print()
-
-    def close_bar(result, iter_num):
-        return lax.cond(
             iter_num == num_samples - 1,
-            lambda _: host_callback.id_tap(
-                _close_bar, None, result=result, tap_with_device=True
-            ),
-            lambda _: result,
+            lambda _: io_callback(_close_bar, None, None),
+            lambda _: None,
             operand=None,
         )
 
     def _progress_bar_scan(func):
         """Decorator that adds a progress bar to `body_fun` used in `lax.scan`.
         Note that `body_fun` must either be looping over `np.arange(num_samples)`,
         or be looping over a tuple who's first element is `np.arange(num_samples)`
@@ -90,13 +74,12 @@
 
         def wrapper_progress_bar(carry, x):
             if type(x) is tuple:
                 iter_num, *_ = x
             else:
                 iter_num = x
             _update_progress_bar(iter_num)
-            result = func(carry, x)
-            return close_bar(result, iter_num)
+            return func(carry, x)
 
         return wrapper_progress_bar
 
     return _progress_bar_scan
```

### Comparing `blackjax-1.1.1/blackjax/sgmcmc/csgld.py` & `blackjax-1.2.0/blackjax/sgmcmc/csgld.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 import jax
 import jax.numpy as jnp
 
 from blackjax.base import SamplingAlgorithm
 from blackjax.sgmcmc.diffusions import overdamped_langevin
 from blackjax.types import Array, ArrayLikeTree, ArrayTree, PRNGKey
 
-__all__ = ["ContourSGLDState", "init", "build_kernel", "csgld"]
+__all__ = ["ContourSGLDState", "init", "build_kernel", "as_top_level_api"]
 
 
 class ContourSGLDState(NamedTuple):
     r"""State of the Contour SgLD algorithm.
 
     Parameters
     ----------
@@ -170,15 +170,22 @@
         )
 
         return ContourSGLDState(position, energy_pdf, idx)
 
     return kernel
 
 
-class csgld:
+def as_top_level_api(
+    logdensity_estimator: Callable,
+    gradient_estimator: Callable,
+    zeta: float = 1,
+    num_partitions: int = 512,
+    energy_gap: float = 100,
+    min_energy: float = 0,
+) -> SamplingAlgorithm:
     r"""Implements the (basic) user interface for the Contour SGLD kernel.
 
     Parameters
     ----------
     logdensity_estimator
         A function that returns an estimation of the model's logdensity given
         a position and a batch of data.
@@ -205,46 +212,34 @@
         the closer the gap between min_energy and 3456 is, the better.
 
     Returns
     -------
     A ``SamplingAlgorithm``.
 
     """
-    init = staticmethod(init)
-    build_kernel = staticmethod(build_kernel)
+    kernel = build_kernel(num_partitions, energy_gap, min_energy)
 
-    def __new__(  # type: ignore[misc]
-        cls,
-        logdensity_estimator: Callable,
-        gradient_estimator: Callable,
-        zeta: float = 1,
-        num_partitions: int = 512,
-        energy_gap: float = 100,
-        min_energy: float = 0,
-    ) -> SamplingAlgorithm:
-        kernel = cls.build_kernel(num_partitions, energy_gap, min_energy)
-
-        def init_fn(position: ArrayLikeTree, rng_key=None):
-            del rng_key
-            return cls.init(position, num_partitions)
-
-        def step_fn(
-            rng_key: PRNGKey,
-            state: ContourSGLDState,
-            minibatch: ArrayLikeTree,
-            step_size_diff: float,
-            step_size_stoch: float,
-            temperature: float = 1.0,
-        ) -> ContourSGLDState:
-            return kernel(
-                rng_key,
-                state,
-                logdensity_estimator,
-                gradient_estimator,
-                minibatch,
-                step_size_diff,
-                step_size_stoch,
-                zeta,
-                temperature,
-            )
+    def init_fn(position: ArrayLikeTree, rng_key=None):
+        del rng_key
+        return init(position, num_partitions)
+
+    def step_fn(
+        rng_key: PRNGKey,
+        state: ContourSGLDState,
+        minibatch: ArrayLikeTree,
+        step_size_diff: float,
+        step_size_stoch: float,
+        temperature: float = 1.0,
+    ) -> ContourSGLDState:
+        return kernel(
+            rng_key,
+            state,
+            logdensity_estimator,
+            gradient_estimator,
+            minibatch,
+            step_size_diff,
+            step_size_stoch,
+            zeta,
+            temperature,
+        )
 
-        return SamplingAlgorithm(init_fn, step_fn)  # type: ignore[arg-type]
+    return SamplingAlgorithm(init_fn, step_fn)  # type: ignore[arg-type]
```

### Comparing `blackjax-1.1.1/blackjax/sgmcmc/diffusions.py` & `blackjax-1.2.0/blackjax/sgmcmc/diffusions.py`

 * *Files identical despite different names*

### Comparing `blackjax-1.1.1/blackjax/sgmcmc/gradients.py` & `blackjax-1.2.0/blackjax/sgmcmc/gradients.py`

 * *Files 1% similar despite different names*

```diff
@@ -121,15 +121,15 @@
         An approximation of the value of the log-posterior density function for
         the current value of the random variables.
 
         """
         grad_estimate = logdensity_grad_estimator(position, minibatch)
         center_grad_estimate = logdensity_grad_estimator(centering_position, minibatch)
 
-        return jax.tree_map(
+        return jax.tree.map(
             lambda grad_est, cv_grad_est, cv_grad: cv_grad + grad_est - cv_grad_est,
             grad_estimate,
             center_grad_estimate,
             cv_grad_value,
         )
 
     return cv_grad_estimator_fn
```

### Comparing `blackjax-1.1.1/blackjax/sgmcmc/sghmc.py` & `blackjax-1.2.0/blackjax/sgmcmc/sghmc.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 import jax
 
 import blackjax.sgmcmc.diffusions as diffusions
 from blackjax.base import SamplingAlgorithm
 from blackjax.types import ArrayLikeTree, ArrayTree, PRNGKey
 from blackjax.util import generate_gaussian_noise
 
-__all__ = ["init", "build_kernel", "sghmc"]
+__all__ = ["init", "build_kernel", "as_top_level_api"]
 
 
 def init(position: ArrayLikeTree) -> ArrayLikeTree:
     return position
 
 
 def build_kernel(alpha: float = 0.01, beta: float = 0) -> Callable:
@@ -54,15 +54,20 @@
         (position, momentum), _ = jax.lax.scan(body_fn, (position, momentum), keys)
 
         return position
 
     return kernel
 
 
-class sghmc:
+def as_top_level_api(
+    grad_estimator: Callable,
+    num_integration_steps: int = 10,
+    alpha: float = 0.01,
+    beta: float = 0,
+) -> SamplingAlgorithm:
     """Implements the (basic) user interface for the SGHMC kernel.
 
     The general sghmc kernel builder (:meth:`blackjax.sgmcmc.sghmc.build_kernel`, alias
     `blackjax.sghmc.build_kernel`) can be cumbersome to manipulate. Since most users
     only need to specify the kernel parameters at initialization time, we
     provide a helper function that specializes the general kernel.
 
@@ -107,41 +112,31 @@
 
     Returns
     -------
     A ``SamplingAlgorithm``.
 
     """
 
-    init = staticmethod(init)
-    build_kernel = staticmethod(build_kernel)
+    kernel = build_kernel(alpha, beta)
 
-    def __new__(  # type: ignore[misc]
-        cls,
-        grad_estimator: Callable,
-        num_integration_steps: int = 10,
-        alpha: float = 0.01,
-        beta: float = 0,
-    ) -> SamplingAlgorithm:
-        kernel = cls.build_kernel(alpha, beta)
-
-        def init_fn(position: ArrayLikeTree, rng_key=None):
-            del rng_key
-            return cls.init(position)
-
-        def step_fn(
-            rng_key: PRNGKey,
-            state: ArrayLikeTree,
-            minibatch: ArrayLikeTree,
-            step_size: float,
-            temperature: float = 1,
-        ) -> ArrayTree:
-            return kernel(
-                rng_key,
-                state,
-                grad_estimator,
-                minibatch,
-                step_size,
-                num_integration_steps,
-                temperature,
-            )
+    def init_fn(position: ArrayLikeTree, rng_key=None):
+        del rng_key
+        return init(position)
+
+    def step_fn(
+        rng_key: PRNGKey,
+        state: ArrayLikeTree,
+        minibatch: ArrayLikeTree,
+        step_size: float,
+        temperature: float = 1,
+    ) -> ArrayTree:
+        return kernel(
+            rng_key,
+            state,
+            grad_estimator,
+            minibatch,
+            step_size,
+            num_integration_steps,
+            temperature,
+        )
 
-        return SamplingAlgorithm(init_fn, step_fn)  # type: ignore[arg-type]
+    return SamplingAlgorithm(init_fn, step_fn)  # type: ignore[arg-type]
```

### Comparing `blackjax-1.1.1/blackjax/sgmcmc/sgld.py` & `blackjax-1.2.0/blackjax/sgmcmc/sgld.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 """Public API for the Stochastic gradient Langevin Dynamics kernel."""
 from typing import Callable
 
 import blackjax.sgmcmc.diffusions as diffusions
 from blackjax.base import SamplingAlgorithm
 from blackjax.types import ArrayLikeTree, ArrayTree, PRNGKey
 
-__all__ = ["init", "build_kernel", "sgld"]
+__all__ = ["init", "build_kernel", "as_top_level_api"]
 
 
 def init(position: ArrayLikeTree) -> ArrayLikeTree:
     return position
 
 
 def build_kernel() -> Callable:
@@ -43,15 +43,17 @@
         )
 
         return new_position
 
     return kernel
 
 
-class sgld:
+def as_top_level_api(
+    grad_estimator: Callable,
+) -> SamplingAlgorithm:
     """Implements the (basic) user interface for the SGLD kernel.
 
     The general sgld kernel builder (:meth:`blackjax.sgmcmc.sgld.build_kernel`, alias
     `blackjax.sgld.build_kernel`) can be cumbersome to manipulate. Since most users
     only need to specify the kernel parameters at initialization time, we
     provide a helper function that specializes the general kernel.
 
@@ -96,32 +98,23 @@
 
     Returns
     -------
     A ``SamplingAlgorithm``.
 
     """
 
-    init = staticmethod(init)
-    build_kernel = staticmethod(build_kernel)
+    kernel = build_kernel()
 
-    def __new__(  # type: ignore[misc]
-        cls,
-        grad_estimator: Callable,
-    ) -> SamplingAlgorithm:
-        kernel = cls.build_kernel()
+    def init_fn(position: ArrayLikeTree, rng_key=None):
+        del rng_key
+        return init(position)
 
-        def init_fn(position: ArrayLikeTree, rng_key=None):
-            del rng_key
-            return cls.init(position)
-
-        def step_fn(
-            rng_key: PRNGKey,
-            state: ArrayLikeTree,
-            minibatch: ArrayLikeTree,
-            step_size: float,
-            temperature: float = 1,
-        ) -> ArrayTree:
-            return kernel(
-                rng_key, state, grad_estimator, minibatch, step_size, temperature
-            )
+    def step_fn(
+        rng_key: PRNGKey,
+        state: ArrayLikeTree,
+        minibatch: ArrayLikeTree,
+        step_size: float,
+        temperature: float = 1,
+    ) -> ArrayTree:
+        return kernel(rng_key, state, grad_estimator, minibatch, step_size, temperature)
 
-        return SamplingAlgorithm(init_fn, step_fn)  # type: ignore[arg-type]
+    return SamplingAlgorithm(init_fn, step_fn)  # type: ignore[arg-type]
```

### Comparing `blackjax-1.1.1/blackjax/sgmcmc/sgnht.py` & `blackjax-1.2.0/blackjax/sgmcmc/sgnht.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from typing import Callable, NamedTuple, Union
 
 import blackjax.sgmcmc.diffusions as diffusions
 from blackjax.base import SamplingAlgorithm
 from blackjax.types import ArrayLikeTree, ArrayTree, PRNGKey
 from blackjax.util import generate_gaussian_noise
 
-__all__ = ["SGNHTState", "init", "build_kernel", "sgnht"]
+__all__ = ["SGNHTState", "init", "build_kernel", "as_top_level_api"]
 
 
 class SGNHTState(NamedTuple):
     r"""State of the SGNHT algorithm.
 
     Parameters
     ----------
@@ -63,15 +63,19 @@
             rng_key, position, momentum, xi, logdensity_grad, step_size, temperature
         )
         return SGNHTState(position, momentum, xi)
 
     return kernel
 
 
-class sgnht:
+def as_top_level_api(
+    grad_estimator: Callable,
+    alpha: float = 0.01,
+    beta: float = 0.0,
+) -> SamplingAlgorithm:
     """Implements the (basic) user interface for the SGNHT kernel.
 
     The general sgnht kernel (:meth:`blackjax.sgmcmc.sgnht.build_kernel`, alias
     `blackjax.sgnht.build_kernel`) can be cumbersome to manipulate. Since most users
     only need to specify the kernel parameters at initialization time, we
     provide a helper function that specializes the general kernel.
 
@@ -117,37 +121,26 @@
 
     Returns
     -------
     A ``SamplingAlgorithm``.
 
     """
 
-    init = staticmethod(init)
-    build_kernel = staticmethod(build_kernel)
+    kernel = build_kernel(alpha, beta)
 
-    def __new__(  # type: ignore[misc]
-        cls,
-        grad_estimator: Callable,
-        alpha: float = 0.01,
-        beta: float = 0.0,
-    ) -> SamplingAlgorithm:
-        kernel = cls.build_kernel(alpha, beta)
-
-        def init_fn(
-            position: ArrayLikeTree,
-            rng_key: PRNGKey,
-            init_xi: Union[None, float] = None,
-        ):
-            return cls.init(position, rng_key, init_xi or alpha)
-
-        def step_fn(
-            rng_key: PRNGKey,
-            state: SGNHTState,
-            minibatch: ArrayLikeTree,
-            step_size: float,
-            temperature: float = 1,
-        ) -> SGNHTState:
-            return kernel(
-                rng_key, state, grad_estimator, minibatch, step_size, temperature
-            )
+    def init_fn(
+        position: ArrayLikeTree,
+        rng_key: PRNGKey,
+        init_xi: Union[None, float] = None,
+    ):
+        return init(position, rng_key, init_xi or alpha)
+
+    def step_fn(
+        rng_key: PRNGKey,
+        state: SGNHTState,
+        minibatch: ArrayLikeTree,
+        step_size: float,
+        temperature: float = 1,
+    ) -> SGNHTState:
+        return kernel(rng_key, state, grad_estimator, minibatch, step_size, temperature)
 
-        return SamplingAlgorithm(init_fn, step_fn)  # type: ignore[arg-type]
+    return SamplingAlgorithm(init_fn, step_fn)  # type: ignore[arg-type]
```

### Comparing `blackjax-1.1.1/blackjax/smc/adaptive_tempered.py` & `blackjax-1.2.0/blackjax/smc/adaptive_tempered.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 import blackjax.smc.base as base
 import blackjax.smc.ess as ess
 import blackjax.smc.solver as solver
 import blackjax.smc.tempered as tempered
 from blackjax.base import SamplingAlgorithm
 from blackjax.types import ArrayLikeTree, PRNGKey
 
-__all__ = ["build_kernel", "adaptive_tempered_smc"]
+__all__ = ["build_kernel", "init", "as_top_level_api"]
 
 
 def build_kernel(
     logprior_fn: Callable,
     loglikelihood_fn: Callable,
     mcmc_step_fn: Callable,
     mcmc_init_fn: Callable,
@@ -99,15 +99,28 @@
         delta = compute_delta(state)
         lmbda = delta + state.lmbda
         return tempered_kernel(rng_key, state, num_mcmc_steps, lmbda, mcmc_parameters)
 
     return kernel
 
 
-class adaptive_tempered_smc:
+init = tempered.init
+
+
+def as_top_level_api(
+    logprior_fn: Callable,
+    loglikelihood_fn: Callable,
+    mcmc_step_fn: Callable,
+    mcmc_init_fn: Callable,
+    mcmc_parameters: dict,
+    resampling_fn: Callable,
+    target_ess: float,
+    root_solver: Callable = solver.dichotomy,
+    num_mcmc_steps: int = 10,
+) -> SamplingAlgorithm:
     """Implements the (basic) user interface for the Adaptive Tempered SMC kernel.
 
     Parameters
     ----------
     logprior_fn
         The log-prior function of the model we wish to draw samples from.
     loglikelihood_fn
@@ -129,46 +142,30 @@
         The number of times the MCMC kernel is applied to the particles per step.
 
     Returns
     -------
     A ``SamplingAlgorithm``.
 
     """
+    kernel = build_kernel(
+        logprior_fn,
+        loglikelihood_fn,
+        mcmc_step_fn,
+        mcmc_init_fn,
+        resampling_fn,
+        target_ess,
+        root_solver,
+    )
 
-    init = staticmethod(tempered.init)
-    build_kernel = staticmethod(build_kernel)
-
-    def __new__(  # type: ignore[misc]
-        cls,
-        logprior_fn: Callable,
-        loglikelihood_fn: Callable,
-        mcmc_step_fn: Callable,
-        mcmc_init_fn: Callable,
-        mcmc_parameters: dict,
-        resampling_fn: Callable,
-        target_ess: float,
-        root_solver: Callable = solver.dichotomy,
-        num_mcmc_steps: int = 10,
-    ) -> SamplingAlgorithm:
-        kernel = cls.build_kernel(
-            logprior_fn,
-            loglikelihood_fn,
-            mcmc_step_fn,
-            mcmc_init_fn,
-            resampling_fn,
-            target_ess,
-            root_solver,
+    def init_fn(position: ArrayLikeTree, rng_key=None):
+        del rng_key
+        return init(position)
+
+    def step_fn(rng_key: PRNGKey, state):
+        return kernel(
+            rng_key,
+            state,
+            num_mcmc_steps,
+            mcmc_parameters,
         )
 
-        def init_fn(position: ArrayLikeTree, rng_key=None):
-            del rng_key
-            return cls.init(position)
-
-        def step_fn(rng_key: PRNGKey, state):
-            return kernel(
-                rng_key,
-                state,
-                num_mcmc_steps,
-                mcmc_parameters,
-            )
-
-        return SamplingAlgorithm(init_fn, step_fn)
+    return SamplingAlgorithm(init_fn, step_fn)
```

### Comparing `blackjax-1.1.1/blackjax/smc/base.py` & `blackjax-1.2.0/blackjax/smc/base.py`

 * *Files 9% similar despite different names*

```diff
@@ -36,14 +36,15 @@
         - Two variables, first one bivariate, second one 4-variate:
             [ Array([[1., 2.], [1.2, 0.5], [3.4, 50]]),
             Array([[50., 51., 52., 51], [51., 52., 52. ,54.], [55., 60, 60, 70]]) ]
     """
 
     particles: ArrayTree
     weights: Array
+    update_parameters: ArrayTree
 
 
 class SMCInfo(NamedTuple):
     """Additional information on the tempered SMC step.
 
     ancestors: Array
         The index of the particles proposed by the MCMC pass that were selected
@@ -55,20 +56,20 @@
     """
 
     ancestors: Array
     log_likelihood_increment: float
     update_info: NamedTuple
 
 
-def init(particles: ArrayLikeTree):
+def init(particles: ArrayLikeTree, init_update_params):
     # Infer the number of particles from the size of the leading dimension of
     # the first leaf of the inputted PyTree.
     num_particles = jax.tree_util.tree_flatten(particles)[0][0].shape[0]
     weights = jnp.ones(num_particles) / num_particles
-    return SMCState(particles, weights)
+    return SMCState(particles, weights, init_update_params)
 
 
 def step(
     rng_key: PRNGKey,
     state: SMCState,
     update_fn: Callable,
     weight_fn: Callable,
@@ -130,20 +131,31 @@
 
     num_particles = state.weights.shape[0]
 
     if num_resampled is None:
         num_resampled = num_particles
 
     resampling_idx = resample_fn(resampling_key, state.weights, num_resampled)
-    particles = jax.tree_map(lambda x: x[resampling_idx], state.particles)
+    particles = jax.tree.map(lambda x: x[resampling_idx], state.particles)
 
     keys = jax.random.split(updating_key, num_resampled)
-    particles, update_info = update_fn(keys, particles)
+    particles, update_info = update_fn(keys, particles, state.update_parameters)
 
     log_weights = weight_fn(particles)
     logsum_weights = jax.scipy.special.logsumexp(log_weights)
     normalizing_constant = logsum_weights - jnp.log(num_particles)
     weights = jnp.exp(log_weights - logsum_weights)
 
-    return SMCState(particles, weights), SMCInfo(
+    return SMCState(particles, weights, state.update_parameters), SMCInfo(
         resampling_idx, normalizing_constant, update_info
     )
+
+
+def extend_params(n_particles, params):
+    """Given a dictionary of params, repeats them for every single particle. The expected
+    usage is in cases where the aim is to repeat the same parameters for all chains within SMC.
+    """
+
+    def extend(param):
+        return jnp.repeat(jnp.asarray(param)[None, ...], n_particles, axis=0)
+
+    return jax.tree.map(extend, params)
```

### Comparing `blackjax-1.1.1/blackjax/smc/ess.py` & `blackjax-1.2.0/blackjax/smc/ess.py`

 * *Files identical despite different names*

### Comparing `blackjax-1.1.1/blackjax/smc/inner_kernel_tuning.py` & `blackjax-1.2.0/blackjax/smc/tempered.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,151 +1,213 @@
-from typing import Callable, Dict, NamedTuple, Tuple, Union
+# Copyright 2020- The Blackjax Authors.
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
+from typing import Callable, NamedTuple
 
+import jax
+import jax.numpy as jnp
+
+import blackjax.smc as smc
 from blackjax.base import SamplingAlgorithm
-from blackjax.smc.adaptive_tempered import adaptive_tempered_smc
-from blackjax.smc.base import SMCInfo, SMCState
-from blackjax.smc.tempered import tempered_smc
-from blackjax.types import ArrayTree, PRNGKey
+from blackjax.smc.base import SMCState
+from blackjax.types import Array, ArrayLikeTree, ArrayTree, PRNGKey
+
+__all__ = ["TemperedSMCState", "init", "build_kernel", "as_top_level_api"]
+
+
+class TemperedSMCState(NamedTuple):
+    """Current state for the tempered SMC algorithm.
 
+    particles: PyTree
+        The particles' positions.
+    lmbda: float
+        Current value of the tempering parameter.
 
-class StateWithParameterOverride(NamedTuple):
-    sampler_state: ArrayTree
-    parameter_override: ArrayTree
+    """
+
+    particles: ArrayTree
+    weights: Array
+    lmbda: float
 
 
-def init(alg_init_fn, position, initial_parameter_value):
-    return StateWithParameterOverride(alg_init_fn(position), initial_parameter_value)
+def init(particles: ArrayLikeTree):
+    # Infer the number of particles from the size of the leading dimension of
+    # the first leaf of the inputted PyTree.
+    num_particles = jax.tree_util.tree_flatten(particles)[0][0].shape[0]
+    weights = jnp.ones(num_particles) / num_particles
+    return TemperedSMCState(particles, weights, 0.0)
 
 
 def build_kernel(
-    smc_algorithm,
     logprior_fn: Callable,
     loglikelihood_fn: Callable,
-    mcmc_factory: Callable,
+    mcmc_step_fn: Callable,
     mcmc_init_fn: Callable,
-    mcmc_parameters: Dict,
     resampling_fn: Callable,
-    mcmc_parameter_update_fn: Callable[[SMCState, SMCInfo], ArrayTree],
-    num_mcmc_steps: int = 10,
-    **extra_parameters,
 ) -> Callable:
-    """In the context of an SMC sampler (whose step_fn returning state has a .particles attribute), there's an inner
-    MCMC that is used to perturbate/update each of the particles. This adaptation tunes some parameter of that MCMC,
-    based on particles. The parameter type must be a valid JAX type.
+    """Build the base Tempered SMC kernel.
+
+    Tempered SMC uses tempering to sample from a distribution given by
+
+    .. math::
+        p(x) \\propto p_0(x) \\exp(-V(x)) \\mathrm{d}x
+
+    where :math:`p_0` is the prior distribution, typically easy to sample from
+    and for which the density is easy to compute, and :math:`\\exp(-V(x))` is an
+    unnormalized likelihood term for which :math:`V(x)` is easy to compute
+    pointwise.
 
     Parameters
     ----------
-    smc_algorithm
-        Either blackjax.adaptive_tempered_smc or blackjax.tempered_smc (or any other implementation of
-        a sampling algorithm that returns an SMCState and SMCInfo pair).
     logprior_fn
         A function that computes the log density of the prior distribution
     loglikelihood_fn
-        A function that returns the probability at a given position.
-    mcmc_factory
-        A callable that can construct an inner kernel out of the newly-computed parameter
-    mcmc_init_fn
-        A callable that initializes the inner kernel
-    mcmc_parameters
-        Other (fixed across SMC iterations) parameters for the inner kernel
-    mcmc_parameter_update_fn
-        A callable that takes the SMCState and SMCInfo at step i and constructs a parameter to be used by the inner kernel in i+1 iteration.
-    extra_parameters:
-        parameters to be used for the creation of the smc_algorithm.
+        A function that returns the probability at a given
+        position.
+    mcmc_step_fn
+        A function that creates a mcmc kernel from a log-probability density function.
+    mcmc_init_fn: Callable
+        A function that creates a new mcmc state from a position and a
+        log-probability density function.
+    resampling_fn
+        A random function that resamples generated particles based of weights
+    num_mcmc_iterations
+        Number of iterations in the MCMC chain.
+
+    Returns
+    -------
+    A callable that takes a rng_key and a TemperedSMCState that contains the current state
+    of the chain and that returns a new state of the chain along with
+    information about the transition.
+
     """
 
     def kernel(
-        rng_key: PRNGKey, state: StateWithParameterOverride, **extra_step_parameters
-    ) -> Tuple[StateWithParameterOverride, SMCInfo]:
-        step_fn = smc_algorithm(
-            logprior_fn=logprior_fn,
-            loglikelihood_fn=loglikelihood_fn,
-            mcmc_step_fn=mcmc_factory(state.parameter_override),
-            mcmc_init_fn=mcmc_init_fn,
-            mcmc_parameters=mcmc_parameters,
-            resampling_fn=resampling_fn,
-            num_mcmc_steps=num_mcmc_steps,
-            **extra_parameters,
-        ).step
-        new_state, info = step_fn(rng_key, state.sampler_state, **extra_step_parameters)
-        new_parameter_override = mcmc_parameter_update_fn(new_state, info)
-        return StateWithParameterOverride(new_state, new_parameter_override), info
+        rng_key: PRNGKey,
+        state: TemperedSMCState,
+        num_mcmc_steps: int,
+        lmbda: float,
+        mcmc_parameters: dict,
+    ) -> tuple[TemperedSMCState, smc.base.SMCInfo]:
+        """Move the particles one step using the Tempered SMC algorithm.
+
+        Parameters
+        ----------
+        rng_key
+            JAX PRNGKey for randomness
+        state
+            Current state of the tempered SMC algorithm
+        lmbda
+            Current value of the tempering parameter
+
+        Returns
+        -------
+        state
+            The new state of the tempered SMC algorithm
+        info
+            Additional information on the SMC step
+
+        """
+        delta = lmbda - state.lmbda
+
+        def log_weights_fn(position: ArrayLikeTree) -> float:
+            return delta * loglikelihood_fn(position)
+
+        def tempered_logposterior_fn(position: ArrayLikeTree) -> float:
+            logprior = logprior_fn(position)
+            tempered_loglikelihood = state.lmbda * loglikelihood_fn(position)
+            return logprior + tempered_loglikelihood
+
+        def mcmc_kernel(rng_key, position, step_parameters):
+            state = mcmc_init_fn(position, tempered_logposterior_fn)
+
+            def body_fn(state, rng_key):
+                new_state, info = mcmc_step_fn(
+                    rng_key, state, tempered_logposterior_fn, **step_parameters
+                )
+                return new_state, info
+
+            keys = jax.random.split(rng_key, num_mcmc_steps)
+            last_state, info = jax.lax.scan(body_fn, state, keys)
+            return last_state.position, info
+
+        smc_state, info = smc.base.step(
+            rng_key,
+            SMCState(state.particles, state.weights, mcmc_parameters),
+            jax.vmap(mcmc_kernel),
+            jax.vmap(log_weights_fn),
+            resampling_fn,
+        )
+        tempered_state = TemperedSMCState(
+            smc_state.particles, smc_state.weights, state.lmbda + delta
+        )
+
+        return tempered_state, info
 
     return kernel
 
 
-class inner_kernel_tuning:
-    """In the context of an SMC sampler (whose step_fn returning state
-    has a .particles attribute), there's an inner MCMC that is used
-    to perturbate/update each of the particles. This adaptation tunes some
-    parameter of that MCMC, based on particles.
-    The parameter type must be a valid JAX type.
+def as_top_level_api(
+    logprior_fn: Callable,
+    loglikelihood_fn: Callable,
+    mcmc_step_fn: Callable,
+    mcmc_init_fn: Callable,
+    mcmc_parameters: dict,
+    resampling_fn: Callable,
+    num_mcmc_steps: int = 10,
+) -> SamplingAlgorithm:
+    """Implements the (basic) user interface for the Adaptive Tempered SMC kernel.
 
     Parameters
     ----------
-    smc_algorithm
-        Either blackjax.adaptive_tempered_smc or blackjax.tempered_smc (or any other implementation of
-        a sampling algorithm that returns an SMCState and SMCInfo pair).
     logprior_fn
-        A function that computes the log density of the prior distribution
+        The log-prior function of the model we wish to draw samples from.
     loglikelihood_fn
-        A function that returns the probability at a given position.
-    mcmc_factory
-        A callable that can construct an inner kernel out of the newly-computed parameter
+        The log-likelihood function of the model we wish to draw samples from.
+    mcmc_step_fn
+        The MCMC step function used to update the particles.
     mcmc_init_fn
-        A callable that initializes the inner kernel
+        The MCMC init function used to build a MCMC state from a particle position.
     mcmc_parameters
-        Other (fixed across SMC iterations) parameters for the inner kernel step
-    mcmc_parameter_update_fn
-        A callable that takes the SMCState and SMCInfo at step i and constructs a parameter to be used by the
-        inner kernel in i+1 iteration.
-    initial_parameter_value
-        Paramter to be used by the mcmc_factory before the first iteration.
-    extra_parameters:
-        parameters to be used for the creation of the smc_algorithm.
+        The parameters of the MCMC step function.
+    resampling_fn
+        The function used to resample the particles.
+    num_mcmc_steps
+        The number of times the MCMC kernel is applied to the particles per step.
 
     Returns
     -------
     A ``SamplingAlgorithm``.
 
     """
-
-    init = staticmethod(init)
-    build_kernel = staticmethod(build_kernel)
-
-    def __new__(  # type: ignore[misc]
-        cls,
-        smc_algorithm: Union[adaptive_tempered_smc, tempered_smc],
-        logprior_fn: Callable,
-        loglikelihood_fn: Callable,
-        mcmc_factory: Callable,
-        mcmc_init_fn: Callable,
-        mcmc_parameters: Dict,
-        resampling_fn: Callable,
-        mcmc_parameter_update_fn: Callable[[SMCState, SMCInfo], ArrayTree],
-        initial_parameter_value,
-        num_mcmc_steps: int = 10,
-        **extra_parameters,
-    ) -> SamplingAlgorithm:
-        kernel = cls.build_kernel(
-            smc_algorithm,
-            logprior_fn,
-            loglikelihood_fn,
-            mcmc_factory,
-            mcmc_init_fn,
-            mcmc_parameters,
-            resampling_fn,
-            mcmc_parameter_update_fn,
+    kernel = build_kernel(
+        logprior_fn,
+        loglikelihood_fn,
+        mcmc_step_fn,
+        mcmc_init_fn,
+        resampling_fn,
+    )
+
+    def init_fn(position: ArrayLikeTree, rng_key=None):
+        del rng_key
+        return init(position)
+
+    def step_fn(rng_key: PRNGKey, state, lmbda):
+        return kernel(
+            rng_key,
+            state,
             num_mcmc_steps,
-            **extra_parameters,
+            lmbda,
+            mcmc_parameters,
         )
 
-        def init_fn(position, rng_key=None):
-            del rng_key
-            return cls.init(smc_algorithm.init, position, initial_parameter_value)
-
-        def step_fn(
-            rng_key: PRNGKey, state, **extra_step_parameters
-        ) -> Tuple[StateWithParameterOverride, SMCInfo]:
-            return kernel(rng_key, state, **extra_step_parameters)
-
-        return SamplingAlgorithm(init_fn, step_fn)
+    return SamplingAlgorithm(init_fn, step_fn)  # type: ignore[arg-type]
```

### Comparing `blackjax-1.1.1/blackjax/smc/resampling.py` & `blackjax-1.2.0/blackjax/smc/resampling.py`

 * *Files identical despite different names*

### Comparing `blackjax-1.1.1/blackjax/smc/solver.py` & `blackjax-1.2.0/blackjax/smc/solver.py`

 * *Files identical despite different names*

### Comparing `blackjax-1.1.1/blackjax/smc/tuning/from_kernel_info.py` & `blackjax-1.2.0/blackjax/smc/tuning/from_kernel_info.py`

 * *Files identical despite different names*

### Comparing `blackjax-1.1.1/blackjax/smc/tuning/from_particles.py` & `blackjax-1.2.0/blackjax/smc/tuning/from_particles.py`

 * *Files identical despite different names*

### Comparing `blackjax-1.1.1/blackjax/types.py` & `blackjax-1.2.0/blackjax/types.py`

 * *Files identical despite different names*

### Comparing `blackjax-1.1.1/blackjax/util.py` & `blackjax-1.2.0/blackjax/util.py`

 * *Files identical despite different names*

### Comparing `blackjax-1.1.1/blackjax/vi/meanfield_vi.py` & `blackjax-1.2.0/blackjax/vi/meanfield_vi.py`

 * *Files 7% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
 __all__ = [
     "MFVIState",
     "MFVIInfo",
     "sample",
     "generate_meanfield_logdensity",
     "step",
-    "meanfield_vi",
+    "as_top_level_api",
 ]
 
 
 class MFVIState(NamedTuple):
     mu: ArrayTree
     rho: ArrayTree
     opt_state: OptState
@@ -44,16 +44,16 @@
 def init(
     position: ArrayLikeTree,
     optimizer: GradientTransformation,
     *optimizer_args,
     **optimizer_kwargs,
 ) -> MFVIState:
     """Initialize the mean-field VI state."""
-    mu = jax.tree_map(jnp.zeros_like, position)
-    rho = jax.tree_map(lambda x: -2.0 * jnp.ones_like(x), position)
+    mu = jax.tree.map(jnp.zeros_like, position)
+    rho = jax.tree.map(lambda x: -2.0 * jnp.ones_like(x), position)
     opt_state = optimizer.init((mu, rho))
     return MFVIState(mu, rho, opt_state)
 
 
 def step(
     rng_key: PRNGKey,
     state: MFVIState,
@@ -95,25 +95,29 @@
             rho = jax.lax.stop_gradient(rho)
         logq = jax.vmap(generate_meanfield_logdensity(mu, rho))(z)
         logp = jax.vmap(logdensity_fn)(z)
         return (logq - logp).mean()
 
     elbo, elbo_grad = jax.value_and_grad(kl_divergence_fn)(parameters)
     updates, new_opt_state = optimizer.update(elbo_grad, state.opt_state, parameters)
-    new_parameters = jax.tree_map(lambda p, u: p + u, parameters, updates)
+    new_parameters = jax.tree.map(lambda p, u: p + u, parameters, updates)
     new_state = MFVIState(new_parameters[0], new_parameters[1], new_opt_state)
     return new_state, MFVIInfo(elbo)
 
 
 def sample(rng_key: PRNGKey, state: MFVIState, num_samples: int = 1):
     """Sample from the mean-field approximation."""
     return _sample(rng_key, state.mu, state.rho, num_samples)
 
 
-class meanfield_vi:
+def as_top_level_api(
+    logdensity_fn: Callable,
+    optimizer: GradientTransformation,
+    num_samples: int = 100,
+):
     """High-level implementation of Mean-Field Variational Inference.
 
     Parameters
     ----------
     logdensity_fn
         A function that represents the log-density function associated with
         the distribution we want to sample from.
@@ -124,49 +128,39 @@
 
     Returns
     -------
     A ``VIAlgorithm``.
 
     """
 
-    init = staticmethod(init)
-    step = staticmethod(step)
-    sample = staticmethod(sample)
-
-    def __new__(
-        cls,
-        logdensity_fn: Callable,
-        optimizer: GradientTransformation,
-        num_samples: int = 100,
-    ):  # type: ignore[misc]
-        def init_fn(position: ArrayLikeTree):
-            return cls.init(position, optimizer)
+    def init_fn(position: ArrayLikeTree):
+        return init(position, optimizer)
 
-        def step_fn(rng_key: PRNGKey, state: MFVIState) -> tuple[MFVIState, MFVIInfo]:
-            return cls.step(rng_key, state, logdensity_fn, optimizer, num_samples)
+    def step_fn(rng_key: PRNGKey, state: MFVIState) -> tuple[MFVIState, MFVIInfo]:
+        return step(rng_key, state, logdensity_fn, optimizer, num_samples)
 
-        def sample_fn(rng_key: PRNGKey, state: MFVIState, num_samples: int):
-            return cls.sample(rng_key, state, num_samples)
+    def sample_fn(rng_key: PRNGKey, state: MFVIState, num_samples: int):
+        return sample(rng_key, state, num_samples)
 
-        return VIAlgorithm(init_fn, step_fn, sample_fn)
+    return VIAlgorithm(init_fn, step_fn, sample_fn)
 
 
 def _sample(rng_key, mu, rho, num_samples):
-    sigma = jax.tree_map(jnp.exp, rho)
+    sigma = jax.tree.map(jnp.exp, rho)
     mu_flatten, unravel_fn = jax.flatten_util.ravel_pytree(mu)
     sigma_flat, _ = jax.flatten_util.ravel_pytree(sigma)
     flatten_sample = (
         jax.random.normal(rng_key, (num_samples,) + mu_flatten.shape) * sigma_flat
         + mu_flatten
     )
     return jax.vmap(unravel_fn)(flatten_sample)
 
 
 def generate_meanfield_logdensity(mu, rho):
-    sigma_param = jax.tree_map(jnp.exp, rho)
+    sigma_param = jax.tree.map(jnp.exp, rho)
 
     def meanfield_logdensity(position):
-        logq_pytree = jax.tree_map(jsp.stats.norm.logpdf, position, mu, sigma_param)
-        logq = jax.tree_map(jnp.sum, logq_pytree)
+        logq_pytree = jax.tree.map(jsp.stats.norm.logpdf, position, mu, sigma_param)
+        logq = jax.tree.map(jnp.sum, logq_pytree)
         return jax.tree_util.tree_reduce(jnp.add, logq)
 
     return meanfield_logdensity
```

### Comparing `blackjax-1.1.1/blackjax/vi/pathfinder.py` & `blackjax-1.2.0/blackjax/vi/pathfinder.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 from blackjax.optimizers.lbfgs import (
     _minimize_lbfgs,
     bfgs_sample,
     lbfgs_inverse_hessian_factors,
 )
 from blackjax.types import Array, ArrayLikeTree, ArrayTree, PRNGKey
 
-__all__ = ["PathfinderState", "approximate", "sample", "pathfinder"]
+__all__ = ["PathfinderState", "approximate", "sample", "as_top_level_api"]
 
 
 class PathfinderState(NamedTuple):
     """State of the Pathfinder algorithm.
 
     Pathfinder locates normal approximations to the target density along a
     quasi-Newton optimization path, with local covariance estimated using
@@ -193,15 +193,15 @@
         unravel_fn_mapped(grad_position),
         alpha,
         beta,
         gamma,
     )
 
     max_elbo_idx = jnp.argmax(elbo)
-    return jax.tree_map(lambda x: x[max_elbo_idx], pathfinder_result), PathfinderInfo(
+    return jax.tree.map(lambda x: x[max_elbo_idx], pathfinder_result), PathfinderInfo(
         pathfinder_result
     )
 
 
 def sample(
     rng_key: PRNGKey,
     state: PathfinderState,
@@ -238,15 +238,15 @@
 
     if num_samples == ():
         return unravel_fn(phi), logq
     else:
         return jax.vmap(unravel_fn)(phi), logq
 
 
-class pathfinder:
+def as_top_level_api(logdensity_fn: Callable) -> PathFinderAlgorithm:
     """Implements the (basic) user interface for the pathfinder kernel.
 
     Pathfinder locates normal approximations to the target density along a
     quasi-Newton optimization path, with local covariance estimated using
     the inverse Hessian estimates produced by the L-BFGS optimizer.
     Pathfinder returns draws from the approximation with the lowest estimated
     Kullback-Leibler (KL) divergence to the true posterior.
@@ -262,25 +262,21 @@
 
     Returns
     -------
     A ``VISamplingAlgorithm``.
 
     """
 
-    approximate = staticmethod(approximate)
-    sample = staticmethod(sample)
-
-    def __new__(cls, logdensity_fn: Callable) -> PathFinderAlgorithm:  # type: ignore[misc]
-        def approximate_fn(
-            rng_key: PRNGKey,
-            position: ArrayLikeTree,
-            num_samples: int = 200,
-            **lbfgs_parameters,
-        ):
-            return cls.approximate(
-                rng_key, logdensity_fn, position, num_samples, **lbfgs_parameters
-            )
+    def approximate_fn(
+        rng_key: PRNGKey,
+        position: ArrayLikeTree,
+        num_samples: int = 200,
+        **lbfgs_parameters,
+    ):
+        return approximate(
+            rng_key, logdensity_fn, position, num_samples, **lbfgs_parameters
+        )
 
-        def sample_fn(rng_key: PRNGKey, state: PathfinderState, num_samples: int):
-            return cls.sample(rng_key, state, num_samples)
+    def sample_fn(rng_key: PRNGKey, state: PathfinderState, num_samples: int):
+        return sample(rng_key, state, num_samples)
 
-        return PathFinderAlgorithm(approximate_fn, sample_fn)
+    return PathFinderAlgorithm(approximate_fn, sample_fn)
```

### Comparing `blackjax-1.1.1/blackjax/vi/schrodinger_follmer.py` & `blackjax-1.2.0/blackjax/vi/schrodinger_follmer.py`

 * *Files 3% similar despite different names*

```diff
@@ -51,15 +51,15 @@
         Approximation of the drift term of the SDE
     """
 
     drift: ArrayLikeTree
 
 
 def init(example_position: ArrayLikeTree) -> SchrodingerFollmerState:
-    zero = jax.tree_map(jnp.zeros_like, example_position)
+    zero = jax.tree.map(jnp.zeros_like, example_position)
     return SchrodingerFollmerState(zero, 0.0)
 
 
 def step(
     rng_key: PRNGKey,
     state: SchrodingerFollmerState,
     logdensity_fn: Callable,
@@ -91,32 +91,32 @@
 
     ravelled_position, unravel_fn = ravel_pytree(state.position)
     scale = jnp.sqrt(1 - state.time)
 
     eps_drift = jax.random.normal(drift_key, (n_samples,) + ravelled_position.shape)
     eps_drift = jax.vmap(unravel_fn)(eps_drift)
 
-    perturbed_position = jax.tree_map(
+    perturbed_position = jax.tree.map(
         lambda a, b: a[None, ...] + scale * b, state.position, eps_drift
     )
 
     log_pdf = jax.vmap(_log_fn_corrected, in_axes=[0, None])(
         perturbed_position, logdensity_fn
     )
     log_pdf -= jnp.max(log_pdf, axis=0, keepdims=True)
     pdf = jnp.exp(log_pdf)
 
-    num = jax.tree_map(lambda a: pdf @ a, eps_drift)
+    num = jax.tree.map(lambda a: pdf @ a, eps_drift)
     den = scale * jnp.sum(pdf, axis=0)
 
-    drift = jax.tree_map(lambda a: a / den, num)
+    drift = jax.tree.map(lambda a: a / den, num)
 
     eps_sde = jax.random.normal(sde_key, ravelled_position.shape)
     eps_sde = unravel_fn(eps_sde)
-    next_position = jax.tree_map(
+    next_position = jax.tree.map(
         lambda a, b, c: a + step_size * b + step_size**0.5 * c,
         state.position,
         drift,
         eps_sde,
     )
     next_state = SchrodingerFollmerState(next_position, state.time + step_size)
     return next_state, SchrodingerFollmerInfo(drift)
@@ -147,45 +147,45 @@
         Number of samples to use to approximate the drift term
     n_samples
         Number of samples to draw
     """
     dt = 1.0 / n_steps
 
     initial_position = initial_state.position
-    initial_positions = jax.tree_map(
+    initial_positions = jax.tree.map(
         lambda a: jnp.zeros([n_samples, *a.shape], dtype=a.dtype), initial_position
     )
     initial_states = SchrodingerFollmerState(initial_positions, jnp.zeros((n_samples,)))
 
-    def body(_, carry):
-        key, states = carry
-        keys = jax.random.split(key, 1 + n_samples)
-        states, _ = jax.vmap(step, [0, 0, None, None, None])(
-            keys[1:], states, log_density_fn, dt, n_inner_samples
+    def body(i, states):
+        subkey = jax.random.fold_in(rng_key, i)
+        keys = jax.random.split(subkey, n_samples)
+        next_states, _ = jax.vmap(step, [0, 0, None, None, None])(
+            keys, states, log_density_fn, dt, n_inner_samples
         )
-        return keys[0], states
+        return next_states
 
-    _, final_states = jax.lax.fori_loop(0, n_steps, body, (rng_key, initial_states))
+    final_states = jax.lax.fori_loop(0, n_steps, body, initial_states)
 
     return final_states
 
 
 def _log_fn_corrected(position, logdensity_fn):
     """
     The Schrödinger-Föllmer algorithm requires the log-density to be given with respect to a standard Gaussian base measure
     but the log-density function passed to the algorithm in BlackJAX is typically given with respect to the Borel measure.
     This corrects the gradient of the log-density function to account for this.
     """
     log_pdf_val = logdensity_fn(position)
-    norm = jax.tree_map(lambda a: 0.5 * jnp.sum(a**2), position)
+    norm = jax.tree.map(lambda a: 0.5 * jnp.sum(a**2), position)
     norm = sum(tree_leaves(norm))
     return log_pdf_val + norm
 
 
-class schrodinger_follmer:
+def as_top_level_api(logdensity_fn: Callable, n_steps: int, n_inner_samples: int) -> VIAlgorithm:  # type: ignore[misc]
     """Implements the (basic) user interface for the Schrödinger-Föllmer algortithm :cite:p:`huang2021schrodingerfollmer`.
 
     The Schrödinger-Föllmer algorithm obtains (approximate) samples from the target distribution by means of a diffusion with
     approximated drifts.
 
     Parameters
     ----------
@@ -198,26 +198,21 @@
         Number of samples used to approximate the drift term
     Returns
     -------
     A ``VIAlgorithm``.
 
     """
 
-    init = staticmethod(init)
-    step = staticmethod(step)
-    sample = staticmethod(sample)
-
-    def __new__(cls, logdensity_fn: Callable, n_steps: int, n_inner_samples: int) -> VIAlgorithm:  # type: ignore[misc]
-        def init_fn(position: ArrayLikeTree):
-            return cls.init(position)
-
-        def step_fn(
-            rng_key: PRNGKey, state: SchrodingerFollmerState
-        ) -> tuple[SchrodingerFollmerState, SchrodingerFollmerInfo]:
-            return cls.step(rng_key, state, logdensity_fn, 1 / n_steps, n_inner_samples)
-
-        def sample_fn(rng_key: PRNGKey, state: SchrodingerFollmerState, n_samples: int):
-            return cls.sample(
-                rng_key, state, logdensity_fn, n_steps, n_inner_samples, n_samples
-            )
+    def init_fn(position: ArrayLikeTree):
+        return init(position)
 
-        return VIAlgorithm(init_fn, step_fn, sample_fn)
+    def step_fn(
+        rng_key: PRNGKey, state: SchrodingerFollmerState
+    ) -> tuple[SchrodingerFollmerState, SchrodingerFollmerInfo]:
+        return step(rng_key, state, logdensity_fn, 1 / n_steps, n_inner_samples)
+
+    def sample_fn(rng_key: PRNGKey, state: SchrodingerFollmerState, n_samples: int):
+        return sample(
+            rng_key, state, logdensity_fn, n_steps, n_inner_samples, n_samples
+        )
+
+    return VIAlgorithm(init_fn, step_fn, sample_fn)
```

### Comparing `blackjax-1.1.1/blackjax/vi/svgd.py` & `blackjax-1.2.0/blackjax/vi/svgd.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,21 @@
 import jax.numpy as jnp
 import optax
 from jax.flatten_util import ravel_pytree
 
 from blackjax.base import SamplingAlgorithm
 from blackjax.types import ArrayLikeTree, ArrayTree
 
-__all__ = ["svgd", "rbf_kernel", "update_median_heuristic"]
+__all__ = [
+    "as_top_level_api",
+    "init",
+    "build_kernel",
+    "rbf_kernel",
+    "update_median_heuristic",
+]
 
 
 class SVGDState(NamedTuple):
     particles: ArrayTree
     kernel_parameters: dict[str, ArrayTree]
     opt_state: Any
 
@@ -119,15 +125,20 @@
     This strategy is called the median heuristic.
     """
 
     position, kernel_parameters, opt_state = state
     return SVGDState(position, median_heuristic(kernel_parameters, position), opt_state)
 
 
-class svgd:
+def as_top_level_api(
+    grad_logdensity_fn: Callable,
+    optimizer,
+    kernel: Callable = rbf_kernel,
+    update_kernel_parameters: Callable = update_median_heuristic,
+):
     """Implements the (basic) user interface for the svgd algorithm.
 
     Parameters
     ----------
     grad_logdensity_fn
         gradient, or an estimate, of the target log density function to samples approximately from
     optimizer
@@ -138,30 +149,20 @@
         function that updates the kernel parameters given the current state of the particles
 
     Returns
     -------
     A ``SamplingAlgorithm``.
     """
 
-    init = staticmethod(init)
-    build_kernel = staticmethod(build_kernel)
+    kernel_ = build_kernel(optimizer)
 
-    def __new__(
-        cls,
-        grad_logdensity_fn: Callable,
-        optimizer,
-        kernel: Callable = rbf_kernel,
-        update_kernel_parameters: Callable = update_median_heuristic,
+    def init_fn(
+        initial_position: ArrayLikeTree,
+        kernel_parameters: dict[str, Any] = {"length_scale": 1.0},
     ):
-        kernel_ = cls.build_kernel(optimizer)
+        return init(initial_position, kernel_parameters, optimizer)
 
-        def init_fn(
-            initial_position: ArrayLikeTree,
-            kernel_parameters: dict[str, Any] = {"length_scale": 1.0},
-        ):
-            return cls.init(initial_position, kernel_parameters, optimizer)
-
-        def step_fn(state, **grad_params):
-            state = kernel_(state, grad_logdensity_fn, kernel, **grad_params)
-            return update_kernel_parameters(state)
+    def step_fn(state, **grad_params):
+        state = kernel_(state, grad_logdensity_fn, kernel, **grad_params)
+        return update_kernel_parameters(state)
 
-        return SamplingAlgorithm(init_fn, step_fn)  # type: ignore[arg-type]
+    return SamplingAlgorithm(init_fn, step_fn)  # type: ignore[arg-type]
```

### Comparing `blackjax-1.1.1/blackjax.egg-info/PKG-INFO` & `blackjax-1.2.0/blackjax.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blackjax
-Version: 1.1.1
+Version: 1.2.0
 Summary: Flexible and fast sampling in Python
 Author-email: The Blackjax team <remi@thetypicalset.com>
 License: Apache License 2.0
 Project-URL: homepage, https://github.com/blackjax-devs/blackjax
 Project-URL: documentation, https://blackjax-devs.github.io/blackjax/
 Project-URL: repository, https://github.com/blackjax-devs/blackjax
 Keywords: probability,machine learning,statistics,mcmc,sampling
@@ -114,16 +114,16 @@
 
 # Initialize the state
 initial_position = {"loc": 1., "scale": 2.}
 state = nuts.init(initial_position)
 
 # Iterate
 rng_key = jax.random.key(0)
-for _ in range(100):
-    rng_key, nuts_key = jax.random.split(rng_key)
+for step in range(100):
+    nuts_key = jax.random.fold_in(rng_key, step)
     state, _ = nuts.step(nuts_key, state)
 ```
 
 See [the documentation](https://blackjax-devs.github.io/blackjax/index.html) for more examples of how to use the library: how to write inference loops for one or several chains, how to use the Stan warmup, etc.
 
 ## Philosophy
```

### Comparing `blackjax-1.1.1/blackjax.egg-info/SOURCES.txt` & `blackjax-1.2.0/blackjax.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `blackjax-1.1.1/docs/_static/blackjax.png` & `blackjax-1.2.0/docs/_static/blackjax.png`

 * *Files identical despite different names*

### Comparing `blackjax-1.1.1/docs/conf.py` & `blackjax-1.2.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `blackjax-1.1.1/docs/examples/data/blackjax.png` & `blackjax-1.2.0/docs/examples/data/blackjax.png`

 * *Files identical despite different names*

### Comparing `blackjax-1.1.1/docs/examples/data/google.csv` & `blackjax-1.2.0/docs/examples/data/google.csv`

 * *Files identical despite different names*

### Comparing `blackjax-1.1.1/docs/examples/howto_custom_gradients.md` & `blackjax-1.2.0/docs/examples/howto_custom_gradients.md`

 * *Files identical despite different names*

### Comparing `blackjax-1.1.1/docs/examples/howto_metropolis_within_gibbs.md` & `blackjax-1.2.0/docs/examples/howto_metropolis_within_gibbs.md`

 * *Files 0% similar despite different names*

```diff
@@ -321,15 +321,15 @@
     num_samples=10_000
 )
 ```
 
 ### Check Result
 
 ```{code-cell} ipython3
-jax.tree_map(lambda x, y: jnp.max(jnp.abs(x-y)), positions, positions_general)
+jax.tree.map(lambda x, y: jnp.max(jnp.abs(x-y)), positions, positions_general)
 ```
 
 ## Developer Notes
 
 - The update method above (using `blackjax.algorithm.init()`) should work out-of-the-box for most (if not all) MCMC algorithms in BlackJAX.  However, it is not optimally efficient.  For example for the RMH update, after obtaining $\yy_{t-1}$ but before drawing $\xx_t$, the method above would calculate `RWState.log_density` to be $\log p(\xx_{t-1}, \yy_{t-1})$.  But we've already calculated this value from the previous HMC update of $\yy_{t-1} \sim p(\yy \mid \xx_{t-1})$.  So, we could save ourselves the cost of calculating the log-density twice, at the expense of a deeper understanding of the low-level components of the algorithms at hand and less generalizable code.
 
 - The general MWG kernel prototyped above should be adequate for problems with a small number of components.  However, the for-loop over the components of `state` gets unrolled by the JAX JIT compiler (as discussed [here](https://jax.readthedocs.io/en/latest/notebooks/Common_Gotchas_in_JAX.html#structured-control-flow-primitives)), which can cause long compilation times when the number of components is large.  To mitigate this problem, the for-loop could be replaced by a `lax.scan()` primitive.  For the sake of simplicity this approach is not fully developed here.
```

### Comparing `blackjax-1.1.1/docs/examples/howto_other_frameworks.md` & `blackjax-1.2.0/docs/examples/howto_other_frameworks.md`

 * *Files identical despite different names*

### Comparing `blackjax-1.1.1/docs/examples/howto_reproduce_the_blackjax_image.md` & `blackjax-1.2.0/docs/examples/howto_reproduce_the_blackjax_image.md`

 * *Files 2% similar despite different names*

```diff
@@ -135,20 +135,20 @@
 ```python
 # Define the loop
 def smc_inference_loop(loop_key, smc_kernel, init_state, schedule):
     """Run the tempered SMC algorithm.
     """
 
     def body_fn(carry, lmbda):
-        carry_key, state = carry
-        carry_key, subkey = jax.random.split(carry_key)
+        i, state = carry
+        subkey = jax.random.fold_in(loop_key, i)
         new_state, info = smc_kernel(subkey, state, lmbda)
-        return (rng_key, new_state), (new_state, info)
+        return (i + 1, new_state), (new_state, info)
 
-    _, (all_samples, _) = jax.lax.scan(body_fn, (loop_key, init_state), schedule)
+    _, (all_samples, _) = jax.lax.scan(body_fn, (0, init_state), schedule)
 
     return all_samples
 
 
 # Run the SMC sampler
 blackjax_samples = smc_inference_loop(rng_key, tempered.step, initial_smc_state, lambda_schedule)
 ```
```

### Comparing `blackjax-1.1.1/docs/examples/howto_sample_multiple_chains.md` & `blackjax-1.2.0/docs/examples/howto_sample_multiple_chains.md`

 * *Files identical despite different names*

### Comparing `blackjax-1.1.1/docs/examples/howto_use_aesara.md` & `blackjax-1.2.0/docs/examples/howto_use_aesara.md`

 * *Files identical despite different names*

### Comparing `blackjax-1.1.1/docs/examples/howto_use_numpyro.md` & `blackjax-1.2.0/docs/examples/howto_use_numpyro.md`

 * *Files identical despite different names*

### Comparing `blackjax-1.1.1/docs/examples/howto_use_oryx.md` & `blackjax-1.2.0/docs/examples/howto_use_oryx.md`

 * *Files identical despite different names*

### Comparing `blackjax-1.1.1/docs/examples/howto_use_pymc.md` & `blackjax-1.2.0/docs/examples/howto_use_pymc.md`

 * *Files identical despite different names*

### Comparing `blackjax-1.1.1/docs/examples/howto_use_tfp.md` & `blackjax-1.2.0/docs/examples/howto_use_tfp.md`

 * *Files identical despite different names*

### Comparing `blackjax-1.1.1/docs/examples/quickstart.md` & `blackjax-1.2.0/docs/examples/quickstart.md`

 * *Files identical despite different names*

### Comparing `blackjax-1.1.1/docs/examples/scatter.gif` & `blackjax-1.2.0/docs/examples/scatter.gif`

 * *Files identical despite different names*

### Comparing `blackjax-1.1.1/docs/index.md` & `blackjax-1.2.0/docs/index.md`

 * *Files 4% similar despite different names*

```diff
@@ -35,16 +35,16 @@
 # Initialize the state
 initial_position = {"loc": 1., "scale": 2.}
 state = nuts.init(initial_position)
 
 # Iterate
 rng_key = jax.random.key(0)
 step = jax.jit(nuts.step)
-for _ in range(1_000):
-    rng_key, nuts_key = jax.random.split(rng_key)
+for i in range(1_000):
+    nuts_key = jax.random.fold_in(rng_key, i)
     state, _ = nuts.step(nuts_key, state)
 ```
 
 :::{note}
 If you want to use Blackjax with a model implemented with a PPL, go to the related tutorials in the left menu.
 :::
 
@@ -110,14 +110,15 @@
 caption: HOW TO
 hidden:
 ---
 Sample with multiple chains?<examples/howto_sample_multiple_chains.md>
 Use custom gradients?<examples/howto_custom_gradients.md>
 Use non-JAX log-prob functions?<examples/howto_other_frameworks.md>
 Build a Metropolis-Within-Gibbs sampler?<examples/howto_metropolis_within_gibbs.md>
+Sample from the word BlackJAX using BlackJAX?<examples/howto_reproduce_the_blackjax_image.md>
 ```
 
 ```{toctree}
 ---
 maxdepth: 1
 caption: LEARN BY EXAMPLE
 hidden:
```

### Comparing `blackjax-1.1.1/docs/refs.bib` & `blackjax-1.2.0/docs/refs.bib`

 * *Files identical despite different names*

### Comparing `blackjax-1.1.1/pyproject.toml` & `blackjax-1.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `blackjax-1.1.1/tests/adaptation/test_adaptation.py` & `blackjax-1.2.0/tests/adaptation/test_adaptation.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     ).sum()
 
     num_burnin_steps = 1000
     num_results = 500
     num_chains = 16
     step_size = 0.1
 
-    init_key, warmup_key, inference_key = jax.random.split(jax.random.key(0), 3)
+    init_key, warmup_key, inference_key = jax.random.split(jax.random.key(346), 3)
 
     warmup = blackjax.chees_adaptation(
         logprob_fn, num_chains=num_chains, target_acceptance_rate=0.75
     )
 
     initial_positions = jax.random.normal(init_key, (num_chains, 2))
     (last_states, parameters), warmup_info = warmup.run(
@@ -64,8 +64,8 @@
     _, _, infos = jax.vmap(
         lambda key, state: run_inference_algorithm(key, state, algorithm, num_results)
     )(chain_keys, last_states)
 
     harmonic_mean = 1.0 / jnp.mean(1.0 / infos.acceptance_rate)
     np.testing.assert_allclose(harmonic_mean, 0.75, rtol=1e-1)
     np.testing.assert_allclose(parameters["step_size"], 1.5, rtol=2e-1)
-    np.testing.assert_allclose(infos.num_integration_steps.mean(), 15.0, rtol=3e-1)
+    np.testing.assert_array_less(infos.num_integration_steps.mean(), 15.0)
```

### Comparing `blackjax-1.1.1/tests/adaptation/test_mass_matrix.py` & `blackjax-1.2.0/tests/adaptation/test_mass_matrix.py`

 * *Files identical despite different names*

### Comparing `blackjax-1.1.1/tests/adaptation/test_step_size.py` & `blackjax-1.2.0/tests/adaptation/test_step_size.py`

 * *Files identical despite different names*

### Comparing `blackjax-1.1.1/tests/mcmc/test_barker.py` & `blackjax-1.2.0/tests/mcmc/test_barker.py`

 * *Files identical despite different names*

### Comparing `blackjax-1.1.1/tests/mcmc/test_integrators.py` & `blackjax-1.2.0/tests/mcmc/test_integrators.py`

 * *Files identical despite different names*

### Comparing `blackjax-1.1.1/tests/mcmc/test_latent_gaussian.py` & `blackjax-1.2.0/tests/mcmc/test_latent_gaussian.py`

 * *Files identical despite different names*

### Comparing `blackjax-1.1.1/tests/mcmc/test_metrics.py` & `blackjax-1.2.0/tests/mcmc/test_metrics.py`

 * *Files identical despite different names*

### Comparing `blackjax-1.1.1/tests/mcmc/test_proposal.py` & `blackjax-1.2.0/tests/mcmc/test_proposal.py`

 * *Files identical despite different names*

### Comparing `blackjax-1.1.1/tests/mcmc/test_random_walk_without_chex.py` & `blackjax-1.2.0/tests/mcmc/test_random_walk_without_chex.py`

 * *Files identical despite different names*

### Comparing `blackjax-1.1.1/tests/mcmc/test_sampling.py` & `blackjax-1.2.0/tests/mcmc/test_sampling.py`

 * *Files 10% similar despite different names*

```diff
@@ -23,20 +23,20 @@
 
     keys = jax.random.split(rng_key, orbits.shape[0])
     samples = jax.vmap(sample_orbit)(orbits, weights, keys)
 
     return samples
 
 
-def irmh_proposal_distribution(rng_key):
+def irmh_proposal_distribution(rng_key, mean):
     """
     The proposal distribution is chosen to be wider than the target, so that the RMH rejection
     doesn't make the sample overemphasize the center of the target distribution.
     """
-    return 1.0 + jax.random.normal(rng_key) * 25.0
+    return mean + jax.random.normal(rng_key) * 25.0
 
 
 def rmh_proposal_distribution(rng_key, position):
     return position + jax.random.normal(rng_key) * 25.0
 
 
 regression_test_cases = [
@@ -453,52 +453,50 @@
 
         init_position = 1.0
         init_position = sghmc.init(init_position)
         data_batch = X_data[:100, :]
         _ = sghmc.step(rng_key, init_position, data_batch, 1e-3)
 
     def test_linear_regression_sgnht(self):
-        rng_key, data_key = jax.random.split(self.key, 2)
+        step_key, data_key = jax.random.split(self.key, 2)
 
         data_size = 1000
         X_data = jax.random.normal(data_key, shape=(data_size, 5))
 
         grad_fn = blackjax.sgmcmc.grad_estimator(
             self.logprior_fn, self.loglikelihood_fn, data_size
         )
         sgnht = blackjax.sgnht(grad_fn)
 
-        _, rng_key = jax.random.split(rng_key)
         data_batch = X_data[100:200, :]
         init_position = 1.0
         data_batch = X_data[:100, :]
         init_state = sgnht.init(init_position, self.key)
-        _ = sgnht.step(rng_key, init_state, data_batch, 1e-3)
+        _ = sgnht.step(step_key, init_state, data_batch, 1e-3)
 
     def test_linear_regression_sgnhtc_cv(self):
-        rng_key, data_key = jax.random.split(self.key, 2)
+        step_key, data_key = jax.random.split(self.key, 2)
 
         data_size = 1000
         X_data = jax.random.normal(data_key, shape=(data_size, 5))
 
         centering_position = 1.0
         grad_fn = blackjax.sgmcmc.grad_estimator(
             self.logprior_fn, self.loglikelihood_fn, data_size
         )
         cv_grad_fn = blackjax.sgmcmc.gradients.control_variates(
             grad_fn, centering_position, X_data
         )
 
         sgnht = blackjax.sgnht(cv_grad_fn)
 
-        _, rng_key = jax.random.split(rng_key)
         init_position = 1.0
         data_batch = X_data[:100, :]
         init_state = sgnht.init(init_position, self.key)
-        _ = sgnht.step(rng_key, init_state, data_batch, 1e-3)
+        _ = sgnht.step(step_key, init_state, data_batch, 1e-3)
 
 
 class LatentGaussianTest(chex.TestCase):
     """Test sampling of a linear regression model."""
 
     def setUp(self):
         super().setUp()
@@ -537,168 +535,200 @@
 
 
 def rmhmc_static_mass_matrix_fn(position):
     del position
     return jnp.array([1.0])
 
 
-normal_test_cases = [
-    {
-        "algorithm": blackjax.hmc,
-        "initial_position": jnp.array(3.0),
-        "parameters": {
-            "step_size": 3.9,
-            "inverse_mass_matrix": jnp.array([1.0]),
-            "num_integration_steps": 30,
-        },
-        "num_sampling_steps": 6000,
-        "burnin": 1_000,
-    },
-    {
-        "algorithm": blackjax.nuts,
-        "initial_position": jnp.array(3.0),
-        "parameters": {"step_size": 4.0, "inverse_mass_matrix": jnp.array([1.0])},
-        "num_sampling_steps": 6000,
-        "burnin": 1_000,
-    },
-    {
-        "algorithm": blackjax.orbital_hmc,
-        "initial_position": jnp.array(100.0),
-        "parameters": {
-            "step_size": 0.1,
-            "inverse_mass_matrix": jnp.array([0.1]),
-            "period": 100,
-        },
-        "num_sampling_steps": 20_000,
-        "burnin": 15_000,
-    },
-    {
-        "algorithm": blackjax.additive_step_random_walk.normal_random_walk,
-        "initial_position": 1.0,
-        "parameters": {"sigma": jnp.array([1.0])},
-        "num_sampling_steps": 20_000,
-        "burnin": 5_000,
-    },
-    {
-        "algorithm": blackjax.rmh,
-        "parameters": {},
-        "initial_position": 1.0,
-        "num_sampling_steps": 20_000,
-        "burnin": 5_000,
-    },
-    {
-        "algorithm": blackjax.mala,
-        "initial_position": 1.0,
-        "parameters": {"step_size": 1e-1},
-        "num_sampling_steps": 45_000,
-        "burnin": 5_000,
-    },
-    {
-        "algorithm": blackjax.elliptical_slice,
-        "initial_position": 1.0,
-        "parameters": {"cov": jnp.array([2.0**2]), "mean": 1.0},
-        "num_sampling_steps": 20_000,
-        "burnin": 5_000,
-    },
-    {
-        "algorithm": blackjax.irmh,
-        "initial_position": jnp.array(1.0),
-        "parameters": {},
-        "num_sampling_steps": 50_000,
-        "burnin": 5_000,
-    },
-    {
-        "algorithm": blackjax.ghmc,
-        "initial_position": jnp.array(1.0),
-        "parameters": {
-            "step_size": 1.0,
-            "momentum_inverse_scale": jnp.array(1.0),
-            "alpha": 0.8,
-            "delta": 2.0,
-        },
-        "num_sampling_steps": 6000,
-        "burnin": 1_000,
-    },
-    {
-        "algorithm": blackjax.barker_proposal,
-        "initial_position": 1.0,
-        "parameters": {"step_size": 1.5},
-        "num_sampling_steps": 20_000,
-        "burnin": 2_000,
-    },
-    {
-        "algorithm": blackjax.rmhmc,
-        "initial_position": jnp.array(3.0),
-        "parameters": {
-            "step_size": 1.0,
-            "num_integration_steps": 30,
-        },
-        "num_sampling_steps": 6000,
-        "burnin": 1_000,
-    },
-]
-
-
 class UnivariateNormalTest(chex.TestCase):
     """Test sampling of a univariate Normal distribution.
 
     (TODO) This only passes due to clever seed hacking.
     """
 
     def setUp(self):
         super().setUp()
         self.key = jax.random.key(12)
 
     def normal_logprob(self, x):
         return stats.norm.logpdf(x, loc=1.0, scale=2.0)
 
-    @chex.all_variants(with_pmap=False)
-    @parameterized.parameters(normal_test_cases)
-    def test_univariate_normal(
-        self, algorithm, initial_position, parameters, num_sampling_steps, burnin
+    def univariate_normal_test_case(
+        self,
+        inference_algorithm,
+        rng_key,
+        initial_state,
+        num_sampling_steps,
+        burnin,
+        postprocess_samples=None,
     ):
-        if algorithm == blackjax.irmh:
-            parameters["proposal_distribution"] = irmh_proposal_distribution
-
-        if algorithm == blackjax.rmh:
-            parameters["proposal_generator"] = rmh_proposal_distribution
-
-        if algorithm == blackjax.rmhmc:
-            parameters["mass_matrix"] = rmhmc_static_mass_matrix_fn
-
-        inference_algorithm = algorithm(self.normal_logprob, **parameters)
-        rng_key = self.key
-        if algorithm == blackjax.elliptical_slice:
-            inference_algorithm = algorithm(lambda x: jnp.ones_like(x), **parameters)
-        if algorithm == blackjax.ghmc:
-            rng_key, initial_state_key = jax.random.split(rng_key)
-            initial_state = inference_algorithm.init(
-                initial_position, initial_state_key
-            )
-        else:
-            initial_state = inference_algorithm.init(initial_position)
-
         inference_key, orbit_key = jax.random.split(rng_key)
         _, states, _ = self.variant(
             functools.partial(
                 run_inference_algorithm,
                 inference_algorithm=inference_algorithm,
                 num_steps=num_sampling_steps,
             )
         )(inference_key, initial_state)
 
-        if algorithm == blackjax.orbital_hmc:
-            samples = orbit_samples(
-                states.positions[burnin:], states.weights[burnin:], orbit_key
-            )
+        # else:
+        if postprocess_samples:
+            samples = postprocess_samples(states, orbit_key)
         else:
             samples = states.position[burnin:]
         np.testing.assert_allclose(np.mean(samples), 1.0, rtol=1e-1)
         np.testing.assert_allclose(np.var(samples), 4.0, rtol=1e-1)
 
+    @chex.all_variants(with_pmap=False)
+    def test_irmh(self):
+        inference_algorithm = blackjax.irmh(
+            self.normal_logprob,
+            proposal_distribution=functools.partial(
+                irmh_proposal_distribution, mean=1.0
+            ),
+        )
+        initial_state = inference_algorithm.init(jnp.array(1.0))
+
+        self.univariate_normal_test_case(
+            inference_algorithm, self.key, initial_state, 50000, 5000
+        )
+
+    @chex.all_variants(with_pmap=False)
+    def test_nuts(self):
+        inference_algorithm = blackjax.nuts(
+            self.normal_logprob, step_size=4.0, inverse_mass_matrix=jnp.array([1.0])
+        )
+
+        initial_state = inference_algorithm.init(jnp.array(3.0))
+
+        self.univariate_normal_test_case(
+            inference_algorithm, self.key, initial_state, 5000, 1000
+        )
+
+    @chex.all_variants(with_pmap=False)
+    def test_rmh(self):
+        inference_algorithm = blackjax.rmh(
+            self.normal_logprob, proposal_generator=rmh_proposal_distribution
+        )
+        initial_state = inference_algorithm.init(1.0)
+
+        self.univariate_normal_test_case(
+            inference_algorithm, self.key, initial_state, 20_000, 5_000
+        )
+
+    @chex.all_variants(with_pmap=False)
+    def test_rmhmc(self):
+        inference_algorithm = blackjax.rmhmc(
+            self.normal_logprob,
+            mass_matrix=rmhmc_static_mass_matrix_fn,
+            step_size=1.0,
+            num_integration_steps=30,
+        )
+
+        initial_state = inference_algorithm.init(jnp.array(3.0))
+
+        self.univariate_normal_test_case(
+            inference_algorithm, self.key, initial_state, 6_000, 1_000
+        )
+
+    @chex.all_variants(with_pmap=False)
+    def test_elliptical_slice(self):
+        inference_algorithm = blackjax.elliptical_slice(
+            lambda x: jnp.ones_like(x), cov=jnp.array([2.0**2]), mean=1.0
+        )
+
+        initial_state = inference_algorithm.init(1.0)
+
+        self.univariate_normal_test_case(
+            inference_algorithm, self.key, initial_state, 20_000, 5_000
+        )
+
+    @chex.all_variants(with_pmap=False)
+    def test_ghmc(self):
+        rng_key, initial_state_key = jax.random.split(self.key)
+        inference_algorithm = blackjax.ghmc(
+            self.normal_logprob,
+            step_size=1.0,
+            momentum_inverse_scale=jnp.array(1.0),
+            alpha=0.8,
+            delta=2.0,
+        )
+        initial_state = inference_algorithm.init(jnp.array(1.0), initial_state_key)
+        self.univariate_normal_test_case(
+            inference_algorithm, rng_key, initial_state, 6000, 1000
+        )
+
+    @chex.all_variants(with_pmap=False)
+    def test_hmc(self):
+        rng_key, initial_state_key = jax.random.split(self.key)
+        inference_algorithm = blackjax.hmc(
+            self.normal_logprob,
+            step_size=3.9,
+            inverse_mass_matrix=jnp.array([1.0]),
+            num_integration_steps=30,
+        )
+        initial_state = inference_algorithm.init(jnp.array(3.0))
+        self.univariate_normal_test_case(
+            inference_algorithm, rng_key, initial_state, 6000, 1000
+        )
+
+    @chex.all_variants(with_pmap=False)
+    def test_orbital_hmc(self):
+        inference_algorithm = blackjax.orbital_hmc(
+            self.normal_logprob,
+            step_size=0.1,
+            inverse_mass_matrix=jnp.array([0.1]),
+            period=100,
+        )
+        initial_state = inference_algorithm.init(jnp.array(100.0))
+        burnin = 15_000
+
+        def postprocess_samples(states, key):
+            return orbit_samples(
+                states.positions[burnin:], states.weights[burnin:], key
+            )
+
+        self.univariate_normal_test_case(
+            inference_algorithm,
+            self.key,
+            initial_state,
+            20_000,
+            burnin,
+            postprocess_samples,
+        )
+
+    @chex.all_variants(with_pmap=False)
+    def test_random_walk(self):
+        inference_algorithm = blackjax.additive_step_random_walk.normal_random_walk(
+            self.normal_logprob, sigma=jnp.array([1.0])
+        )
+        initial_state = inference_algorithm.init(jnp.array(1.0))
+
+        self.univariate_normal_test_case(
+            inference_algorithm, self.key, initial_state, 20_000, 5_000
+        )
+
+    @chex.all_variants(with_pmap=False)
+    def test_mala(self):
+        inference_algorithm = blackjax.mala(self.normal_logprob, step_size=1e-1)
+        initial_state = inference_algorithm.init(jnp.array(1.0))
+        self.univariate_normal_test_case(
+            inference_algorithm, self.key, initial_state, 45000, 5_000
+        )
+
+    @chex.all_variants(with_pmap=False)
+    def test_barker(self):
+        inference_algorithm = blackjax.barker_proposal(
+            self.normal_logprob, step_size=1.5
+        )
+        initial_state = inference_algorithm.init(jnp.array(1.0))
+        self.univariate_normal_test_case(
+            inference_algorithm, self.key, initial_state, 20000, 2_000
+        )
+
 
 mcse_test_cases = [
     {
         "algorithm": blackjax.hmc,
         "parameters": {
             "step_size": 0.5,
             "num_integration_steps": 20,
@@ -732,15 +762,15 @@
 
 
 class MonteCarloStandardErrorTest(chex.TestCase):
     """Test sampler correctness using Monte Carlo Central Limit Theorem."""
 
     def setUp(self):
         super().setUp()
-        self.key = jax.random.key(20220203)
+        self.key = jax.random.key(8456)
 
     def generate_multivariate_target(self, rng=None):
         """Genrate a Multivariate Normal distribution as target."""
         if rng is None:
             loc = jnp.array([0.0, 3])
             scale = jnp.array([1.0, 2.0])
             rho = jnp.array(0.75)
@@ -815,15 +845,15 @@
         posterior_samples = states.position[:, -1000:]
         posterior_delta = posterior_samples - true_loc
         posterior_variance = posterior_delta**2.0
         posterior_correlation = jnp.prod(posterior_delta, axis=-1, keepdims=True) / (
             true_scale[0] * true_scale[1]
         )
 
-        _ = jax.tree_map(
+        _ = jax.tree.map(
             self.mcse_test,
             [posterior_samples, posterior_variance, posterior_correlation],
             [true_loc, true_scale**2, true_rho],
         )
 
 
 if __name__ == "__main__":
```

### Comparing `blackjax-1.1.1/tests/mcmc/test_trajectory.py` & `blackjax-1.2.0/tests/mcmc/test_trajectory.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,8 @@
 """Test the trajectory integration"""
-import functools
-
 import chex
 import jax
 import jax.numpy as jnp
 import numpy as np
 from absl.testing import absltest, parameterized
 
 import blackjax.mcmc.dynamic_hmc as dynamic_hmc
@@ -71,15 +69,15 @@
             step_size,
             initial_energy,
         )
 
         assert is_diverging.item() is should_diverge
 
     def test_dynamic_progressive_equal_recursive(self):
-        rng_key = jax.random.key(23132)
+        rng_key = jax.random.key(23133)
 
         def logdensity_fn(x):
             return -((1.0 - x[0]) ** 2) - 1.5 * (x[1] - x[0] ** 2) ** 2
 
         inverse_mass_matrix = jnp.asarray([[1.0, 0.5], [0.5, 1.25]])
         (
             momentum_generator,
@@ -120,23 +118,24 @@
         buildtree_integrator = trajectory.dynamic_recursive_integration(
             integrator,
             kinetic_energy_fn,
             uturn_check_fn,
             divergence_threshold,
         )
 
-        for _ in range(50):
+        for i in range(50):
+            subkey = jax.random.fold_in(rng_key, i)
             (
-                rng_key,
+                rng_buildtree,
                 rng_direction,
                 rng_tree_depth,
                 rng_step_size,
                 rng_position,
                 rng_momentum,
-            ) = jax.random.split(rng_key, 6)
+            ) = jax.random.split(subkey, 6)
             direction = jax.random.choice(rng_direction, jnp.array([-1, 1]))
             tree_depth = jax.random.choice(rng_tree_depth, np.arange(2, 5))
             initial_state = integrators.new_integrator_state(
                 logdensity_fn,
                 jax.random.normal(rng_position, [2]),
                 jax.random.normal(rng_momentum, [2]),
             )
@@ -149,15 +148,15 @@
             (
                 proposal0,
                 trajectory0,
                 _,
                 is_diverging0,
                 has_terminated0,
             ) = trajectory_integrator(
-                rng_key,
+                rng_buildtree,
                 initial_state,
                 direction,
                 termination_state,
                 2**tree_depth,
                 step_size,
                 initial_energy,
             )
@@ -165,27 +164,24 @@
             (
                 _,
                 proposal1,
                 trajectory1,
                 is_diverging1,
                 has_terminated1,
             ) = buildtree_integrator(
-                rng_key,
+                rng_buildtree,
                 initial_state,
                 direction,
                 tree_depth,
                 step_size,
                 initial_energy,
             )
             # Assert that the trajectory being built is the same
-            jax.tree_map(
-                functools.partial(np.testing.assert_allclose, rtol=1e-5),
-                trajectory0,
-                trajectory1,
-            )
+            chex.assert_trees_all_close(trajectory0, trajectory1, rtol=1e-5)
+
             assert is_diverging0 == is_diverging1
             assert has_terminated0 == has_terminated1
             # We dont expect the proposal to be the same (even with the same PRNGKey
             # as the order of selection is different). but the property associate
             # with the full trajectory should be the same.
             np.testing.assert_allclose(proposal0.weight, proposal1.weight, rtol=1e-5)
             np.testing.assert_allclose(
@@ -283,19 +279,15 @@
         # performed using a scan
         scan_state = static_integration(initial_state, 0.1, 10)
 
         # When jitted, the number of steps is no longer static - make sure that
         # we still get the same result
         fori_state = jax.jit(static_integration)(initial_state, 0.1, 10)
 
-        jax.tree_util.tree_map(
-            functools.partial(np.testing.assert_allclose, rtol=1e-5),
-            fori_state,
-            scan_state,
-        )
+        chex.assert_trees_all_close(fori_state, scan_state, rtol=1e-5)
 
     def test_dynamic_hmc_integration_steps(self):
         rng_key = jax.random.key(0)
         num_step_key, sample_key = jax.random.split(rng_key)
         initial_position = jnp.array(3.0)
         parameters = {"step_size": 3.9, "inverse_mass_matrix": jnp.array([1.0])}
```

### Comparing `blackjax-1.1.1/tests/mcmc/test_uturn.py` & `blackjax-1.2.0/tests/mcmc/test_uturn.py`

 * *Files identical despite different names*

### Comparing `blackjax-1.1.1/tests/optimizers/test_optimizers.py` & `blackjax-1.2.0/tests/optimizers/test_optimizers.py`

 * *Files 0% similar despite different names*

```diff
@@ -84,15 +84,15 @@
         b0_flatten, unravel_fn = ravel_pytree(b0)
         objective_fn = lambda x: -fn(unravel_fn(x))
         (_, status), history = self.variant(
             functools.partial(
                 minimize_lbfgs, objective_fn, maxiter=maxiter, maxcor=maxcor
             )
         )(b0_flatten)
-        history = jax.tree_map(lambda x: x[: status.iter_num + 1], history)
+        history = jax.tree.map(lambda x: x[: status.iter_num + 1], history)
 
         # Test recover alpha
         S = jnp.diff(history.x, axis=0)
         Z = jnp.diff(history.g, axis=0)
         alpha0 = history.alpha[0]
 
         def scan_fn(alpha, val):
@@ -134,15 +134,15 @@
 
         def loss_fn(x):
             return -stats.multivariate_normal.logpdf(x, mean, cov)
 
         (result, status), history = self.variant(
             functools.partial(minimize_lbfgs, loss_fn, maxiter=50)
         )(np.zeros(nd))
-        history = jax.tree_map(lambda x: x[: status.iter_num + 1], history)
+        history = jax.tree.map(lambda x: x[: status.iter_num + 1], history)
 
         np.testing.assert_allclose(result, mean, rtol=0.01)
 
         S_partial = jnp.diff(history.x, axis=0)[-10:].T
         Z_partial = jnp.diff(history.g, axis=0)[-10:].T
         alpha = history.alpha[-1]
```

### Comparing `blackjax-1.1.1/tests/optimizers/test_pathfinder.py` & `blackjax-1.2.0/tests/optimizers/test_pathfinder.py`

 * *Files identical despite different names*

### Comparing `blackjax-1.1.1/tests/smc/__init__.py` & `blackjax-1.2.0/tests/smc/__init__.py`

 * *Files identical despite different names*

### Comparing `blackjax-1.1.1/tests/smc/test_inner_kernel_tuning.py` & `blackjax-1.2.0/tests/smc/test_inner_kernel_tuning.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,17 @@
 import jax.scipy.stats as stats
 import numpy as np
 from absl.testing import absltest
 
 import blackjax
 import blackjax.smc.resampling as resampling
 from blackjax import adaptive_tempered_smc, tempered_smc
-from blackjax.smc.inner_kernel_tuning import inner_kernel_tuning
+from blackjax.mcmc.random_walk import build_irmh
+from blackjax.smc import extend_params
+from blackjax.smc.inner_kernel_tuning import as_top_level_api as inner_kernel_tuning
 from blackjax.smc.tuning.from_kernel_info import update_scale_from_acceptance_rate
 from blackjax.smc.tuning.from_particles import (
     mass_matrix_from_particles,
     particles_as_rows,
     particles_covariance_matrix,
     particles_means,
     particles_stds,
@@ -88,46 +90,45 @@
         # Don't use exactly the invariant distribution for the MCMC kernel
         init_particles = 0.25 + np.random.randn(1000) * 50
 
         proposal_factory = MagicMock()
         proposal_factory.return_value = 100
 
         def mcmc_parameter_update_fn(state, info):
-            return 100
+            return extend_params(1000, {"mean": 100})
 
-        mcmc_factory = MagicMock()
-        sampling_algorithm = MagicMock()
-        mcmc_factory.return_value = sampling_algorithm
         prior = lambda x: stats.norm.logpdf(x)
 
-        def kernel_factory(proposal_distribution):
-            kernel = blackjax.irmh.build_kernel()
-
-            def wrapped_kernel(rng_key, state, logdensity):
-                return kernel(rng_key, state, logdensity, proposal_distribution)
-
-            return wrapped_kernel
+        def wrapped_kernel(rng_key, state, logdensity, mean):
+            return build_irmh()(
+                rng_key,
+                state,
+                logdensity,
+                functools.partial(irmh_proposal_distribution, mean=mean),
+            )
 
         kernel = inner_kernel_tuning(
             logprior_fn=prior,
             loglikelihood_fn=specialized_log_weights_fn,
-            mcmc_factory=kernel_factory,
+            mcmc_step_fn=wrapped_kernel,
             mcmc_init_fn=blackjax.irmh.init,
             resampling_fn=resampling.systematic,
             smc_algorithm=smc_algorithm,
-            mcmc_parameters={},
             mcmc_parameter_update_fn=mcmc_parameter_update_fn,
-            initial_parameter_value=irmh_proposal_distribution,
+            initial_parameter_value=extend_params(1000, {"mean": 1.0}),
             **smc_parameters,
         )
 
         new_state, new_info = kernel.step(
             self.key, state=kernel.init(init_particles), **step_parameters
         )
-        assert new_state.parameter_override == 100
+        assert set(new_state.parameter_override.keys()) == {
+            "mean",
+        }
+        np.testing.assert_allclose(new_state.parameter_override["mean"], 100)
 
 
 class MeanAndStdFromParticlesTest(chex.TestCase):
     def setUp(self):
         super().setUp()
         self.key = jax.random.key(42)
 
@@ -266,102 +267,122 @@
 
 
 class InnerKernelTuningJitTest(SMCLinearRegressionTestCase):
     def setUp(self):
         super().setUp()
         self.key = jax.random.key(42)
 
-    def mcmc_factory(self, mass_matrix):
-        return functools.partial(
-            blackjax.hmc.build_kernel(),
-            inverse_mass_matrix=mass_matrix,
-            step_size=10e-2,
-            num_integration_steps=50,
-        )
-
     @chex.all_variants(with_pmap=False)
     def test_with_adaptive_tempered(self):
         (
             init_particles,
             logprior_fn,
             loglikelihood_fn,
         ) = self.particles_prior_loglikelihood()
 
+        def parameter_update(state, info):
+            return extend_params(
+                100,
+                {
+                    "inverse_mass_matrix": mass_matrix_from_particles(state.particles),
+                    "step_size": 10e-2,
+                    "num_integration_steps": 50,
+                },
+            )
+
         init, step = blackjax.inner_kernel_tuning(
             adaptive_tempered_smc,
             logprior_fn,
             loglikelihood_fn,
-            self.mcmc_factory,
+            blackjax.hmc.build_kernel(),
             blackjax.hmc.init,
-            {},
             resampling.systematic,
-            mcmc_parameter_update_fn=lambda state, info: mass_matrix_from_particles(
-                state.particles
+            mcmc_parameter_update_fn=parameter_update,
+            initial_parameter_value=extend_params(
+                100,
+                dict(
+                    inverse_mass_matrix=jnp.eye(2),
+                    step_size=10e-2,
+                    num_integration_steps=50,
+                ),
             ),
-            initial_parameter_value=jnp.eye(2),
             num_mcmc_steps=10,
             target_ess=0.5,
         )
         init_state = init(init_particles)
         smc_kernel = self.variant(step)
 
         def inference_loop(kernel, rng_key, initial_state):
             def cond(carry):
-                state, key = carry
+                _, state = carry
                 return state.sampler_state.lmbda < 1
 
             def body(carry):
-                state, op_key = carry
-                op_key, subkey = jax.random.split(op_key, 2)
+                i, state = carry
+                subkey = jax.random.fold_in(rng_key, i)
                 state, _ = kernel(subkey, state)
-                return state, op_key
+                return i + 1, state
 
-            return jax.lax.while_loop(cond, body, (initial_state, rng_key))
+            return jax.lax.while_loop(cond, body, (0, initial_state))
 
-        state, _ = inference_loop(smc_kernel, self.key, init_state)
+        _, state = inference_loop(smc_kernel, self.key, init_state)
 
-        assert state.parameter_override.shape == (2, 2)
+        assert state.parameter_override["inverse_mass_matrix"].shape == (100, 2, 2)
         self.assert_linear_regression_test_case(state.sampler_state)
 
     @chex.all_variants(with_pmap=False)
     def test_with_tempered_smc(self):
         num_tempering_steps = 10
         (
             init_particles,
             logprior_fn,
             loglikelihood_fn,
         ) = self.particles_prior_loglikelihood()
 
+        def parameter_update(state, info):
+            return extend_params(
+                100,
+                {
+                    "inverse_mass_matrix": mass_matrix_from_particles(state.particles),
+                    "step_size": 10e-2,
+                    "num_integration_steps": 50,
+                },
+            )
+
         init, step = blackjax.inner_kernel_tuning(
             tempered_smc,
             logprior_fn,
             loglikelihood_fn,
-            self.mcmc_factory,
+            blackjax.hmc.build_kernel(),
             blackjax.hmc.init,
-            {},
             resampling.systematic,
-            mcmc_parameter_update_fn=lambda state, info: mass_matrix_from_particles(
-                state.particles
+            mcmc_parameter_update_fn=parameter_update,
+            initial_parameter_value=extend_params(
+                100,
+                dict(
+                    inverse_mass_matrix=jnp.eye(2),
+                    step_size=10e-2,
+                    num_integration_steps=50,
+                ),
             ),
-            initial_parameter_value=jnp.eye(2),
             num_mcmc_steps=10,
         )
 
         init_state = init(init_particles)
         smc_kernel = self.variant(step)
 
         lambda_schedule = np.logspace(-5, 0, num_tempering_steps)
 
         def body_fn(carry, lmbda):
-            rng_key, state = carry
-            rng_key, subkey = jax.random.split(rng_key)
+            i, state = carry
+            subkey = jax.random.fold_in(self.key, i)
             new_state, info = smc_kernel(subkey, state, lmbda=lmbda)
-            return (rng_key, new_state), (new_state, info)
+            return (i + 1, new_state), (new_state, info)
 
-        (_, result), _ = jax.lax.scan(body_fn, (self.key, init_state), lambda_schedule)
+        (_, result), _ = jax.lax.scan(body_fn, (0, init_state), lambda_schedule)
         self.assert_linear_regression_test_case(result.sampler_state)
 
 
 class ParticlesAsRowsTest(unittest.TestCase):
     def test_particles_as_rows(self):
         n_particles = 1000
         test_particles = {
```

### Comparing `blackjax-1.1.1/tests/smc/test_resampling.py` & `blackjax-1.2.0/tests/smc/test_resampling.py`

 * *Files identical despite different names*

### Comparing `blackjax-1.1.1/tests/smc/test_smc.py` & `blackjax-1.2.0/tests/smc/test_smc.py`

 * *Files 27% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import jax.numpy as jnp
 import jax.scipy.stats as stats
 import numpy as np
 from absl.testing import absltest
 
 import blackjax
 import blackjax.smc.resampling as resampling
-from blackjax.smc.base import init, step
+from blackjax.smc.base import extend_params, init, step
 
 
 def logdensity_fn(position):
     return jnp.sum(stats.norm.logpdf(position))
 
 
 def _weighted_avg_and_std(values, weights):
@@ -27,37 +27,37 @@
         self.key = jax.random.key(42)
 
     @chex.variants(with_jit=True)
     def test_smc(self):
         num_mcmc_steps = 20
         num_particles = 1000
 
-        hmc = blackjax.hmc(
-            logdensity_fn,
-            step_size=1e-2,
-            inverse_mass_matrix=jnp.eye(1),
-            num_integration_steps=50,
-        )
-
-        def update_fn(rng_key, position):
+        def update_fn(rng_key, position, update_params):
+            hmc = blackjax.hmc(logdensity_fn, **update_params)
             state = hmc.init(position)
 
             def body_fn(state, rng_key):
                 new_state, info = hmc.step(rng_key, state)
                 return new_state, info
 
             keys = jax.random.split(rng_key, num_mcmc_steps)
             last_state, info = jax.lax.scan(body_fn, state, keys)
             return last_state.position, info
 
         init_key, sample_key = jax.random.split(self.key)
 
         # Initialize the state of the SMC sampler
         init_particles = 0.25 + jax.random.normal(init_key, shape=(num_particles,))
-        state = init(init_particles)
+        same_for_all_params = dict(
+            step_size=1e-2, inverse_mass_matrix=jnp.eye(1), num_integration_steps=50
+        )
+        state = init(
+            init_particles,
+            extend_params(num_particles, same_for_all_params),
+        )
 
         # Run the SMC sampler once
         new_state, info = self.variant(step, static_argnums=(2, 3, 4))(
             sample_key,
             state,
             jax.vmap(update_fn),
             jax.vmap(logdensity_fn),
@@ -70,42 +70,46 @@
 
     @chex.variants(with_jit=True)
     def test_smc_waste_free(self):
         num_mcmc_steps = 10
         num_particles = 1000
         num_resampled = num_particles // num_mcmc_steps
 
-        hmc = blackjax.hmc(
-            logdensity_fn,
-            step_size=1e-2,
-            inverse_mass_matrix=jnp.eye(1),
-            num_integration_steps=100,
-        )
-
-        def waste_free_update_fn(keys, particles):
-            def one_particle_fn(rng_key, position):
+        def waste_free_update_fn(keys, particles, update_params):
+            def one_particle_fn(rng_key, position, particle_update_params):
+                hmc = blackjax.hmc(logdensity_fn, **particle_update_params)
                 state = hmc.init(position)
 
                 def body_fn(state, rng_key):
                     new_state, info = hmc.step(rng_key, state)
                     return new_state, (state, info)
 
                 keys = jax.random.split(rng_key, num_mcmc_steps)
                 _, (states, info) = jax.lax.scan(body_fn, state, keys)
                 return states.position, info
 
-            particles, info = jax.vmap(one_particle_fn)(keys, particles)
+            particles, info = jax.vmap(one_particle_fn)(keys, particles, update_params)
             particles = particles.reshape((num_particles,))
             return particles, info
 
         init_key, sample_key = jax.random.split(self.key)
 
         # Initialize the state of the SMC sampler
         init_particles = 0.25 + jax.random.normal(init_key, shape=(num_particles,))
-        state = init(init_particles)
+        state = init(
+            init_particles,
+            extend_params(
+                num_resampled,
+                dict(
+                    step_size=1e-2,
+                    inverse_mass_matrix=jnp.eye(1),
+                    num_integration_steps=100,
+                ),
+            ),
+        )
 
         # Run the SMC sampler once
         new_state, info = self.variant(step, static_argnums=(2, 3, 4, 5))(
             sample_key,
             state,
             waste_free_update_fn,
             jax.vmap(logdensity_fn),
@@ -114,9 +118,31 @@
         )
 
         mean, std = _weighted_avg_and_std(new_state.particles, state.weights)
         np.testing.assert_allclose(0.0, mean, atol=1e-1)
         np.testing.assert_allclose(1.0, std, atol=1e-1)
 
 
+class ExtendParamsTest(chex.TestCase):
+    def test_extend_params(self):
+        extended = extend_params(
+            3,
+            {
+                "a": 50,
+                "b": np.array([50]),
+                "c": np.array([50, 60]),
+                "d": np.array([[1, 2], [3, 4]]),
+            },
+        )
+        np.testing.assert_allclose(extended["a"], np.ones((3,)) * 50)
+        np.testing.assert_allclose(extended["b"], np.array([[50], [50], [50]]))
+        np.testing.assert_allclose(
+            extended["c"], np.array([[50, 60], [50, 60], [50, 60]])
+        )
+        np.testing.assert_allclose(
+            extended["d"],
+            np.array([[[1, 2], [3, 4]], [[1, 2], [3, 4]], [[1, 2], [3, 4]]]),
+        )
+
+
 if __name__ == "__main__":
     absltest.main()
```

### Comparing `blackjax-1.1.1/tests/smc/test_smc_ess.py` & `blackjax-1.2.0/tests/smc/test_smc_ess.py`

 * *Files identical despite different names*

### Comparing `blackjax-1.1.1/tests/smc/test_solver.py` & `blackjax-1.2.0/tests/smc/test_solver.py`

 * *Files identical despite different names*

### Comparing `blackjax-1.1.1/tests/smc/test_tempered_smc.py` & `blackjax-1.2.0/tests/smc/test_tempered_smc.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,30 +8,31 @@
 import numpy as np
 from absl.testing import absltest
 
 import blackjax
 import blackjax.smc.resampling as resampling
 import blackjax.smc.solver as solver
 from blackjax import adaptive_tempered_smc, tempered_smc
+from blackjax.smc import extend_params
 from tests.smc import SMCLinearRegressionTestCase
 
 
 def inference_loop(kernel, rng_key, initial_state):
     def cond(carry):
         _, state, *_ = carry
         return state.lmbda < 1
 
     def body(carry):
-        i, state, op_key, curr_loglikelihood = carry
-        op_key, subkey = jax.random.split(op_key, 2)
+        i, state, curr_loglikelihood = carry
+        subkey = jax.random.fold_in(rng_key, i)
         state, info = kernel(subkey, state)
-        return i + 1, state, op_key, curr_loglikelihood + info.log_likelihood_increment
+        return i + 1, state, curr_loglikelihood + info.log_likelihood_increment
 
-    total_iter, final_state, _, log_likelihood = jax.lax.while_loop(
-        cond, body, (0, initial_state, rng_key, 0.0)
+    total_iter, final_state, log_likelihood = jax.lax.while_loop(
+        cond, body, (0, initial_state, 0.0)
     )
 
     return total_iter, final_state, log_likelihood
 
 
 class TemperedSMCTest(SMCLinearRegressionTestCase):
     """Test posterior mean estimate."""
@@ -60,19 +61,22 @@
         smc_state_init = [log_scale_init, coeffs_init]
 
         iterates = []
         results = []
 
         hmc_kernel = blackjax.hmc.build_kernel()
         hmc_init = blackjax.hmc.init
-        hmc_parameters = {
-            "step_size": 10e-2,
-            "inverse_mass_matrix": jnp.eye(2),
-            "num_integration_steps": 50,
-        }
+        hmc_parameters = extend_params(
+            num_particles,
+            {
+                "step_size": 10e-2,
+                "inverse_mass_matrix": jnp.eye(2),
+                "num_integration_steps": 50,
+            },
+        )
 
         for target_ess in [0.5, 0.75]:
             tempering = adaptive_tempered_smc(
                 logprior_fn,
                 loglikelihood_fn,
                 hmc_kernel,
                 hmc_init,
@@ -106,39 +110,42 @@
         ) = self.particles_prior_loglikelihood()
 
         num_tempering_steps = 10
 
         lambda_schedule = np.logspace(-5, 0, num_tempering_steps)
         hmc_init = blackjax.hmc.init
         hmc_kernel = blackjax.hmc.build_kernel()
-        hmc_parameters = {
-            "step_size": 10e-2,
-            "inverse_mass_matrix": jnp.eye(2),
-            "num_integration_steps": 50,
-        }
+        hmc_parameters = extend_params(
+            100,
+            {
+                "step_size": 10e-2,
+                "inverse_mass_matrix": jnp.eye(2),
+                "num_integration_steps": 50,
+            },
+        )
 
         tempering = tempered_smc(
             logprior_fn,
             loglikelihood_fn,
             hmc_kernel,
             hmc_init,
             hmc_parameters,
             resampling.systematic,
             10,
         )
         init_state = tempering.init(init_particles)
         smc_kernel = self.variant(tempering.step)
 
         def body_fn(carry, lmbda):
-            rng_key, state = carry
-            rng_key, subkey = jax.random.split(rng_key)
+            i, state = carry
+            subkey = jax.random.fold_in(self.key, i)
             new_state, info = smc_kernel(subkey, state, lmbda)
-            return (rng_key, new_state), (new_state, info)
+            return (i + 1, new_state), (new_state, info)
 
-        (_, result), _ = jax.lax.scan(body_fn, (self.key, init_state), lambda_schedule)
+        (_, result), _ = jax.lax.scan(body_fn, (0, init_state), lambda_schedule)
         self.assert_linear_regression_test_case(result)
 
 
 def normal_logdensity_fn(x, chol_cov):
     """minus log-density of a centered multivariate normal distribution"""
     dim = chol_cov.shape[0]
     y = jax.scipy.linalg.solve_triangular(chol_cov, x, lower=True)
@@ -170,19 +177,22 @@
         loglikelihood_fn = lambda x: normal_logdensity_fn(x, chol_cov)
 
         rng_key, init_key = jax.random.split(rng_key, 2)
         x_init = jax.random.normal(init_key, shape=(num_particles, num_dim))
 
         hmc_init = blackjax.hmc.init
         hmc_kernel = blackjax.hmc.build_kernel()
-        hmc_parameters = {
-            "step_size": 10e-2,
-            "inverse_mass_matrix": jnp.eye(num_dim),
-            "num_integration_steps": 50,
-        }
+        hmc_parameters = extend_params(
+            num_particles,
+            {
+                "step_size": 10e-2,
+                "inverse_mass_matrix": jnp.eye(num_dim),
+                "num_integration_steps": 50,
+            },
+        )
 
         tempering = adaptive_tempered_smc(
             logprior_fn,
             loglikelihood_fn,
             hmc_kernel,
             hmc_init,
             hmc_parameters,
```

### Comparing `blackjax-1.1.1/tests/test_benchmarks.py` & `blackjax-1.2.0/tests/test_benchmarks.py`

 * *Files identical despite different names*

### Comparing `blackjax-1.1.1/tests/test_compilation.py` & `blackjax-1.2.0/tests/test_compilation.py`

 * *Files 8% similar despite different names*

```diff
@@ -36,16 +36,16 @@
             logdensity_fn,
             step_size=1e-2,
             inverse_mass_matrix=jnp.array([1.0]),
             num_integration_steps=10,
         )
         step = jax.jit(kernel.step)
 
-        for _ in range(10):
-            rng_key, sample_key = jax.random.split(rng_key)
+        for i in range(10):
+            sample_key = jax.random.fold_in(rng_key, i)
             state, _ = step(sample_key, state)
 
     def test_nuts(self):
         """Count the number of times the logdensity is compiled when using NUTS.
 
         The logdensity is compiled twice: when initializing the state and when
         compiling the kernel.
@@ -62,16 +62,16 @@
         state = blackjax.nuts.init(1.0, logdensity_fn)
 
         kernel = blackjax.nuts(
             logdensity_fn, step_size=1e-2, inverse_mass_matrix=jnp.array([1.0])
         )
         step = jax.jit(kernel.step)
 
-        for _ in range(10):
-            rng_key, sample_key = jax.random.split(rng_key)
+        for i in range(10):
+            sample_key = jax.random.fold_in(rng_key, i)
             state, _ = step(sample_key, state)
 
     def test_hmc_warmup(self):
         """Count the number of times the logdensity is compiled when using window
         adaptation to adapt the value of the step size and the inverse mass
         matrix for the HMC algorithm.
 
@@ -90,16 +90,16 @@
             logdensity_fn=logdensity_fn,
             target_acceptance_rate=0.8,
             num_integration_steps=10,
         )
         (state, parameters), _ = warmup.run(rng_key, 1.0, num_steps=100)
         kernel = jax.jit(blackjax.hmc(logdensity_fn, **parameters).step)
 
-        for _ in range(10):
-            rng_key, sample_key = jax.random.split(rng_key)
+        for i in range(10):
+            sample_key = jax.random.fold_in(rng_key, i)
             state, _ = kernel(sample_key, state)
 
     def test_nuts_warmup(self):
         """Count the number of times the logdensity is compiled when using window
         adaptation to adapt the value of the step size and the inverse mass
         matrix for the NUTS algorithm.
 
@@ -117,14 +117,14 @@
             algorithm=blackjax.nuts,
             logdensity_fn=logdensity_fn,
             target_acceptance_rate=0.8,
         )
         (state, parameters), _ = warmup.run(rng_key, 1.0, num_steps=100)
         step = jax.jit(blackjax.nuts(logdensity_fn, **parameters).step)
 
-        for _ in range(10):
-            rng_key, sample_key = jax.random.split(rng_key)
+        for i in range(10):
+            sample_key = jax.random.fold_in(rng_key, i)
             state, _ = step(sample_key, state)
 
 
 if __name__ == "__main__":
     absltest.main()
```

### Comparing `blackjax-1.1.1/tests/test_diagnostics.py` & `blackjax-1.2.0/tests/test_diagnostics.py`

 * *Files identical despite different names*

### Comparing `blackjax-1.1.1/tests/test_util.py` & `blackjax-1.2.0/tests/test_util.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import chex
 import jax
 import jax.numpy as jnp
 from absl.testing import absltest, parameterized
 
-from blackjax.mcmc.hmc import hmc
+import blackjax
 from blackjax.util import run_inference_algorithm
 
 
 class RunInferenceAlgorithmTest(chex.TestCase):
     def setUp(self):
         super().setUp()
         self.key = jax.random.key(42)
-        self.algorithm = hmc(
+        self.algorithm = blackjax.hmc(
             logdensity_fn=self.logdensity_fn,
             inverse_mass_matrix=jnp.eye(2),
             step_size=1.0,
             num_integration_steps=1000,
         )
         self.num_steps = 10
```

### Comparing `blackjax-1.1.1/tests/vi/test_meanfield_vi.py` & `blackjax-1.2.0/tests/vi/test_meanfield_vi.py`

 * *Files 9% similar despite different names*

```diff
@@ -32,20 +32,20 @@
         num_samples = 500
 
         optimizer = optax.sgd(1e-2)
         mfvi = blackjax.meanfield_vi(logdensity_fn, optimizer, num_samples)
         state = mfvi.init(initial_position)
 
         rng_key = self.key
-        for _ in range(num_steps):
-            rng_key, subkey = jax.random.split(rng_key)
+        for i in range(num_steps):
+            subkey = jax.random.fold_in(rng_key, i)
             state, _ = jax.jit(mfvi.step)(subkey, state)
 
         loc_1, loc_2 = state.mu["x_1"], state.mu["x_2"]
-        scale = jax.tree_map(jnp.exp, state.rho)
+        scale = jax.tree.map(jnp.exp, state.rho)
         scale_1, scale_2 = scale["x_1"], scale["x_2"]
         self.assertAlmostEqual(loc_1, ground_truth[0][0], delta=0.01)
         self.assertAlmostEqual(scale_1, ground_truth[0][1], delta=0.01)
         self.assertAlmostEqual(loc_2, ground_truth[1][0], delta=0.01)
         self.assertAlmostEqual(scale_2, ground_truth[1][1], delta=0.01)
```

### Comparing `blackjax-1.1.1/tests/vi/test_schrodinger_follmer.py` & `blackjax-1.2.0/tests/vi/test_schrodinger_follmer.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import chex
 import jax
 import jax.numpy as jnp
 import jax.scipy.stats as stats
 from absl.testing import absltest
 
-from blackjax.vi.schrodinger_follmer import schrodinger_follmer
+from blackjax.vi.schrodinger_follmer import as_top_level_api as schrodinger_follmer
 
 
 class SchrodingerFollmerTest(chex.TestCase):
     def setUp(self):
         super().setUp()
         self.key = jax.random.key(1)
```

### Comparing `blackjax-1.1.1/tests/vi/test_svgd.py` & `blackjax-1.2.0/tests/vi/test_svgd.py`

 * *Files identical despite different names*

