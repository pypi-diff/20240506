# Comparing `tmp/stock-indicators-1.2.1.tar.gz` & `tmp/stock_indicators-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stock-indicators-1.2.1.tar", last modified: Thu Mar  7 13:33:23 2024, max compression
+gzip compressed data, was "stock_indicators-1.3.0.tar", last modified: Mon May  6 11:40:11 2024, max compression
```

## Comparing `stock-indicators-1.2.1.tar` & `stock_indicators-1.3.0.tar`

### file list

```diff
@@ -1,390 +1,397 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 13:33:23.993917 stock-indicators-1.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)      502 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 13:33:23.925917 stock-indicators-1.2.1/.github/
--rw-r--r--   0 runner    (1001) docker     (127)     5311 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/.github/CODE_OF_CONDUCT.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 13:33:23.925917 stock-indicators-1.2.1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      448 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/.github/SECURITY.md
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 13:33:23.925917 stock-indicators-1.2.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2194 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/.github/workflows/deploy.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1877 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/.github/workflows/docs-deploy.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/.github/workflows/docs-test-a11y.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1874 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/.github/workflows/docs-test-links.yml
--rw-r--r--   0 runner    (1001) docker     (127)      377 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/.github/workflows/lock.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2987 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/.github/workflows/semantic-pr-linter.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/.github/workflows/test-all-env.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/.github/workflows/test-coverage.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1854 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4295 2024-03-07 13:33:23.993917 stock-indicators-1.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1718 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 13:33:23.925917 stock-indicators-1.2.1/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/benchmarks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2024 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/benchmarks/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     7732 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/benchmarks/test_benchmark_indicators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 13:33:23.929917 stock-indicators-1.2.1/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 13:33:23.929917 stock-indicators-1.2.1/docs/.offline/
--rw-r--r--   0 runner    (1001) docker     (127)   106009 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/docs/.offline/banner.png
--rw-r--r--   0 runner    (1001) docker     (127)   490879 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/docs/.offline/banner.xcf
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/docs/.pa11yci
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/docs/404.html
--rw-r--r--   0 runner    (1001) docker     (127)      544 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/docs/GemFile
--rw-r--r--   0 runner    (1001) docker     (127)     8424 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/docs/GemFile.lock
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/docs/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/docs/_config.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 13:33:23.929917 stock-indicators-1.2.1/docs/_data/
--rw-r--r--   0 runner    (1001) docker     (127)     1924 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/docs/_data/aliases.yml
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/docs/_data/categories.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 13:33:23.929917 stock-indicators-1.2.1/docs/_includes/
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/docs/_includes/candle-result.md
--rw-r--r--   0 runner    (1001) docker     (127)      514 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/docs/_includes/candlepart-options.md
--rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/docs/_includes/cyclotron.html
--rw-r--r--   0 runner    (1001) docker     (127)      533 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/docs/_includes/footer.html
--rw-r--r--   0 runner    (1001) docker     (127)     5297 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/docs/_includes/head-style.html
--rw-r--r--   0 runner    (1001) docker     (127)     1741 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/docs/_includes/head.html
--rw-r--r--   0 runner    (1001) docker     (127)      849 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/docs/_includes/header.html
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/docs/_includes/scripts.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 13:33:23.945917 stock-indicators-1.2.1/docs/_indicators/
--rw-r--r--   0 runner    (1001) docker     (127)     2995 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/docs/_indicators/Adl.md
--rw-r--r--   0 runner    (1001) docker     (127)     3309 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/docs/_indicators/Adx.md
--rw-r--r--   0 runner    (1001) docker     (127)     3982 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/docs/_indicators/Alligator.md
--rw-r--r--   0 runner    (1001) docker     (127)     3069 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/docs/_indicators/Alma.md
--rw-r--r--   0 runner    (1001) docker     (127)     2790 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/docs/_indicators/Aroon.md
--rw-r--r--   0 runner    (1001) docker     (127)     3297 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/docs/_indicators/Atr.md
--rw-r--r--   0 runner    (1001) docker     (127)     2925 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/docs/_indicators/Awesome.md
--rw-r--r--   0 runner    (1001) docker     (127)     4503 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/docs/_indicators/Beta.md
--rw-r--r--   0 runner    (1001) docker     (127)     3645 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/docs/_indicators/BollingerBands.md
--rw-r--r--   0 runner    (1001) docker     (127)     2748 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/docs/_indicators/Bop.md
--rw-r--r--   0 runner    (1001) docker     (127)     2676 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/docs/_indicators/Cci.md
--rw-r--r--   0 runner    (1001) docker     (127)     3664 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/docs/_indicators/ChaikinOsc.md
--rw-r--r--   0 runner    (1001) docker     (127)     3403 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/docs/_indicators/Chandelier.md
--rw-r--r--   0 runner    (1001) docker     (127)     2628 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/docs/_indicators/Chop.md
--rw-r--r--   0 runner    (1001) docker     (127)     2864 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/docs/_indicators/Cmf.md
--rw-r--r--   0 runner    (1001) docker     (127)     3718 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/docs/_indicators/ConnorsRsi.md
--rw-r--r--   0 runner    (1001) docker     (127)     3711 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/docs/_indicators/Correlation.md
--rw-r--r--   0 runner    (1001) docker     (127)     3099 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/docs/_indicators/Dema.md
--rw-r--r--   0 runner    (1001) docker     (127)     2827 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/docs/_indicators/Doji.md
--rw-r--r--   0 runner    (1001) docker     (127)     3139 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/docs/_indicators/Donchian.md
--rw-r--r--   0 runner    (1001) docker     (127)     2773 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/docs/_indicators/Dpo.md
--rw-r--r--   0 runner    (1001) docker     (127)     3262 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/docs/_indicators/ElderRay.md
--rw-r--r--   0 runner    (1001) docker     (127)     3379 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/docs/_indicators/Ema.md
--rw-r--r--   0 runner    (1001) docker     (127)     2699 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/docs/_indicators/Epma.md
--rw-r--r--   0 runner    (1001) docker     (127)     2966 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/docs/_indicators/Fcb.md
--rw-r--r--   0 runner    (1001) docker     (127)     3066 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/docs/_indicators/FisherTransform.md
--rw-r--r--   0 runner    (1001) docker     (127)     3081 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/docs/_indicators/ForceIndex.md
--rw-r--r--   0 runner    (1001) docker     (127)     3646 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/docs/_indicators/Fractal.md
--rw-r--r--   0 runner    (1001) docker     (127)     3303 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/docs/_indicators/Gator.md
--rw-r--r--   0 runner    (1001) docker     (127)     2761 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/docs/_indicators/HeikinAshi.md
--rw-r--r--   0 runner    (1001) docker     (127)     2664 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/docs/_indicators/Hma.md
--rw-r--r--   0 runner    (1001) docker     (127)     3122 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/docs/_indicators/HtTrendline.md
--rw-r--r--   0 runner    (1001) docker     (127)     3117 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/docs/_indicators/Hurst.md
--rw-r--r--   0 runner    (1001) docker     (127)     4327 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/docs/_indicators/Ichimoku.md
--rw-r--r--   0 runner    (1001) docker     (127)     3722 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/docs/_indicators/Kama.md
--rw-r--r--   0 runner    (1001) docker     (127)     3686 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/docs/_indicators/Keltner.md
--rw-r--r--   0 runner    (1001) docker     (127)     3384 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/docs/_indicators/Kvo.md
--rw-r--r--   0 runner    (1001) docker     (127)     4533 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/docs/_indicators/MaEnvelopes.md
--rw-r--r--   0 runner    (1001) docker     (127)     3889 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/docs/_indicators/Macd.md
--rw-r--r--   0 runner    (1001) docker     (127)     3027 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/docs/_indicators/Mama.md
--rw-r--r--   0 runner    (1001) docker     (127)     2839 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/docs/_indicators/Marubozu.md
--rw-r--r--   0 runner    (1001) docker     (127)     2595 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/docs/_indicators/Mfi.md
--rw-r--r--   0 runner    (1001) docker     (127)     2893 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/docs/_indicators/Obv.md
--rw-r--r--   0 runner    (1001) docker     (127)     3538 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/docs/_indicators/ParabolicSar.md
--rw-r--r--   0 runner    (1001) docker     (127)     4670 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/docs/_indicators/PivotPoints.md
--rw-r--r--   0 runner    (1001) docker     (127)     4660 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/docs/_indicators/Pivots.md
--rw-r--r--   0 runner    (1001) docker     (127)     3151 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/docs/_indicators/Pmo.md
--rw-r--r--   0 runner    (1001) docker     (127)     3941 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/docs/_indicators/Prs.md
--rw-r--r--   0 runner    (1001) docker     (127)     3579 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/docs/_indicators/Pvo.md
--rw-r--r--   0 runner    (1001) docker     (127)     6188 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/docs/_indicators/Renko.md
--rw-r--r--   0 runner    (1001) docker     (127)     4665 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/docs/_indicators/Roc.md
--rw-r--r--   0 runner    (1001) docker     (127)     4394 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/docs/_indicators/RollingPivots.md
--rw-r--r--   0 runner    (1001) docker     (127)     3213 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/docs/_indicators/Rsi.md
--rw-r--r--   0 runner    (1001) docker     (127)     3510 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/docs/_indicators/Slope.md
--rw-r--r--   0 runner    (1001) docker     (127)     3684 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/docs/_indicators/Sma.md
--rw-r--r--   0 runner    (1001) docker     (127)     3317 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/docs/_indicators/Smi.md
--rw-r--r--   0 runner    (1001) docker     (127)     3196 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/docs/_indicators/Smma.md
--rw-r--r--   0 runner    (1001) docker     (127)     3695 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/docs/_indicators/StarcBands.md
--rw-r--r--   0 runner    (1001) docker     (127)     3372 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/docs/_indicators/Stc.md
--rw-r--r--   0 runner    (1001) docker     (127)     3285 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/docs/_indicators/StdDev.md
--rw-r--r--   0 runner    (1001) docker     (127)     3754 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/docs/_indicators/StdDevChannels.md
--rw-r--r--   0 runner    (1001) docker     (127)     4393 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/docs/_indicators/Stoch.md
--rw-r--r--   0 runner    (1001) docker     (127)     4273 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/docs/_indicators/StochRsi.md
--rw-r--r--   0 runner    (1001) docker     (127)     3739 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/docs/_indicators/SuperTrend.md
--rw-r--r--   0 runner    (1001) docker     (127)     3192 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/docs/_indicators/T3.md
--rw-r--r--   0 runner    (1001) docker     (127)     3444 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/docs/_indicators/Tema.md
--rw-r--r--   0 runner    (1001) docker     (127)     3403 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/docs/_indicators/Trix.md
--rw-r--r--   0 runner    (1001) docker     (127)     3409 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/docs/_indicators/Tsi.md
--rw-r--r--   0 runner    (1001) docker     (127)     2670 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/docs/_indicators/UlcerIndex.md
--rw-r--r--   0 runner    (1001) docker     (127)     3020 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/docs/_indicators/Ultimate.md
--rw-r--r--   0 runner    (1001) docker     (127)     4022 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/docs/_indicators/VolatilityStop.md
--rw-r--r--   0 runner    (1001) docker     (127)     2829 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/docs/_indicators/Vortex.md
--rw-r--r--   0 runner    (1001) docker     (127)     3375 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/docs/_indicators/Vwap.md
--rw-r--r--   0 runner    (1001) docker     (127)     2578 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/docs/_indicators/Vwma.md
--rw-r--r--   0 runner    (1001) docker     (127)     2846 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/docs/_indicators/WilliamsR.md
--rw-r--r--   0 runner    (1001) docker     (127)     2980 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/docs/_indicators/Wma.md
--rw-r--r--   0 runner    (1001) docker     (127)     4173 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/docs/_indicators/ZigZag.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 13:33:23.945917 stock-indicators-1.2.1/docs/_layouts/
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/docs/_layouts/base.html
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/docs/_layouts/indicator.html
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/docs/_layouts/page.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 13:33:23.945917 stock-indicators-1.2.1/docs/assets/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 13:33:23.945917 stock-indicators-1.2.1/docs/assets/css/
--rw-r--r--   0 runner    (1001) docker     (127)     7485 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/docs/assets/css/normalize.css
--rw-r--r--   0 runner    (1001) docker     (127)     2903 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/docs/assets/css/rouge-github.css
--rw-r--r--   0 runner    (1001) docker     (127)     9652 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/docs/assets/css/style.scss
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 13:33:23.949917 stock-indicators-1.2.1/docs/assets/icons/
--rw-r--r--   0 runner    (1001) docker     (127)     6223 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/docs/assets/icons/android-chrome-192x192.png
--rw-r--r--   0 runner    (1001) docker     (127)    15305 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/docs/assets/icons/android-chrome-512x512.png
--rw-r--r--   0 runner    (1001) docker     (127)     3862 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/docs/assets/icons/apple-touch-icon.png
--rw-r--r--   0 runner    (1001) docker     (127)      222 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/docs/assets/icons/browserconfig.xml
--rw-r--r--   0 runner    (1001) docker     (127)      973 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/docs/assets/icons/favicon-16x16.png
--rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/docs/assets/icons/favicon-32x32.png
--rw-r--r--   0 runner    (1001) docker     (127)     7352 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/docs/assets/icons/maskable_icon_x192.png
--rw-r--r--   0 runner    (1001) docker     (127)    21568 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/docs/assets/icons/maskable_icon_x512.png
--rw-r--r--   0 runner    (1001) docker     (127)     3711 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/docs/assets/icons/mstile-144x144.png
--rw-r--r--   0 runner    (1001) docker     (127)     3785 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/docs/assets/icons/mstile-150x150.png
--rw-r--r--   0 runner    (1001) docker     (127)     3924 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/docs/assets/icons/mstile-310x150.png
--rw-r--r--   0 runner    (1001) docker     (127)     6454 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/docs/assets/icons/mstile-310x310.png
--rw-r--r--   0 runner    (1001) docker     (127)     2972 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/docs/assets/icons/mstile-70x70.png
--rw-r--r--   0 runner    (1001) docker     (127)     6147 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/docs/assets/icons/safari-pinned-tab.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 13:33:23.949917 stock-indicators-1.2.1/docs/assets/js/
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/docs/assets/js/ga.js
--rw-r--r--   0 runner    (1001) docker     (127)     7889 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/docs/assets/js/lazysizes.min.js
--rw-r--r--   0 runner    (1001) docker     (127)      794 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/docs/assets/manifest.json
--rw-r--r--   0 runner    (1001) docker     (127)   106009 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/docs/assets/social-banner.png
--rw-r--r--   0 runner    (1001) docker     (127)     8803 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/docs/contributing.md
--rw-r--r--   0 runner    (1001) docker     (127)    15086 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/docs/favicon.ico
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 13:33:23.949917 stock-indicators-1.2.1/docs/pages/
--rw-r--r--   0 runner    (1001) docker     (127)    13824 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/docs/pages/guide.md
--rw-r--r--   0 runner    (1001) docker     (127)     4674 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/docs/pages/home.md
--rw-r--r--   0 runner    (1001) docker     (127)     1700 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/docs/pages/indicators.html
--rw-r--r--   0 runner    (1001) docker     (127)    34393 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/docs/pages/performance.md
--rw-r--r--   0 runner    (1001) docker     (127)     3576 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/docs/pages/utilities.md
--rw-r--r--   0 runner    (1001) docker     (127)     3149 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 13:33:23.921917 stock-indicators-1.2.1/samples/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 13:33:23.957917 stock-indicators-1.2.1/samples/quotes/
--rw-r--r--   0 runner    (1001) docker     (127)    32824 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/samples/quotes/Bad.csv
--rw-r--r--   0 runner    (1001) docker     (127)    75494 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/samples/quotes/Bitcoin.csv
--rw-r--r--   0 runner    (1001) docker     (127)    28127 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/samples/quotes/Compare.csv
--rw-r--r--   0 runner    (1001) docker     (127)    26480 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/samples/quotes/Default.csv
--rw-r--r--   0 runner    (1001) docker     (127)  2350932 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/samples/quotes/History.xlsx
--rw-r--r--   0 runner    (1001) docker     (127)    94960 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/samples/quotes/Intraday.csv
--rw-r--r--   0 runner    (1001) docker     (127)   909185 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/samples/quotes/Longest.csv
--rw-r--r--   0 runner    (1001) docker     (127)   332796 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/samples/quotes/Longish.csv
--rw-r--r--   0 runner    (1001) docker     (127)   357981 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/samples/quotes/MSFT.csv
--rw-r--r--   0 runner    (1001) docker     (127)    53463 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/samples/quotes/Max.csv
--rw-r--r--   0 runner    (1001) docker     (127)    24574 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/samples/quotes/Mismatch.csv
--rw-r--r--   0 runner    (1001) docker     (127)    22595 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/samples/quotes/Penny.csv
--rw-r--r--   0 runner    (1001) docker     (127)   411660 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/samples/quotes/SPX.csv
--rw-r--r--   0 runner    (1001) docker     (127)   132770 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/samples/quotes/TooBig.csv
--rw-r--r--   0 runner    (1001) docker     (127)    33255 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/samples/quotes/ZigZag.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 13:33:23.957917 stock-indicators-1.2.1/samples/zig_zag/
--rw-r--r--   0 runner    (1001) docker     (127)    83092 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/samples/zig_zag/data.ethusdt.json
--rw-r--r--   0 runner    (1001) docker     (127)     3045 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/samples/zig_zag/data.issue632.json
--rw-r--r--   0 runner    (1001) docker     (127)    55992 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/samples/zig_zag/data.schrodinger.json
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-07 13:33:23.993917 stock-indicators-1.2.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 13:33:23.957917 stock-indicators-1.2.1/stock_indicators/
--rw-r--r--   0 runner    (1001) docker     (127)      744 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/stock_indicators/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 13:33:23.961917 stock-indicators-1.2.1/stock_indicators/_cslib/
--rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/stock_indicators/_cslib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 13:33:23.961917 stock-indicators-1.2.1/stock_indicators/_cslib/lib/
--rw-r--r--   0 runner    (1001) docker     (127)   219648 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/stock_indicators/_cslib/lib/Skender.Stock.Indicators.dll
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 13:33:23.961917 stock-indicators-1.2.1/stock_indicators/_cstypes/
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/stock_indicators/_cstypes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/stock_indicators/_cstypes/datetime.py
--rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/stock_indicators/_cstypes/decimal.py
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/stock_indicators/_cstypes/list.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 13:33:23.977917 stock-indicators-1.2.1/stock_indicators/indicators/
--rw-r--r--   0 runner    (1001) docker     (127)     2846 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/stock_indicators/indicators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2340 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/stock_indicators/indicators/adl.py
--rw-r--r--   0 runner    (1001) docker     (127)     2369 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/stock_indicators/indicators/adx.py
--rw-r--r--   0 runner    (1001) docker     (127)     3178 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/stock_indicators/indicators/alligator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2103 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/stock_indicators/indicators/alma.py
--rw-r--r--   0 runner    (1001) docker     (127)     2217 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/stock_indicators/indicators/aroon.py
--rw-r--r--   0 runner    (1001) docker     (127)     2105 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/stock_indicators/indicators/atr.py
--rw-r--r--   0 runner    (1001) docker     (127)     2273 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/stock_indicators/indicators/awesome.py
--rw-r--r--   0 runner    (1001) docker     (127)     1927 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/stock_indicators/indicators/basic_quotes.py
--rw-r--r--   0 runner    (1001) docker     (127)     3334 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/stock_indicators/indicators/beta.py
--rw-r--r--   0 runner    (1001) docker     (127)     3114 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/stock_indicators/indicators/bollinger_bands.py
--rw-r--r--   0 runner    (1001) docker     (127)     1865 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/stock_indicators/indicators/bop.py
--rw-r--r--   0 runner    (1001) docker     (127)     1849 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/stock_indicators/indicators/cci.py
--rw-r--r--   0 runner    (1001) docker     (127)     2734 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/stock_indicators/indicators/chaikin_oscillator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2385 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/stock_indicators/indicators/chandelier.py
--rw-r--r--   0 runner    (1001) docker     (127)     1857 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/stock_indicators/indicators/chop.py
--rw-r--r--   0 runner    (1001) docker     (127)     2266 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/stock_indicators/indicators/cmf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 13:33:23.977917 stock-indicators-1.2.1/stock_indicators/indicators/common/
--rw-r--r--   0 runner    (1001) docker     (127)      543 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/stock_indicators/indicators/common/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 13:33:23.977917 stock-indicators-1.2.1/stock_indicators/indicators/common/_contrib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/stock_indicators/indicators/common/_contrib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/stock_indicators/indicators/common/_contrib/enum.py
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/stock_indicators/indicators/common/_contrib/type_resolver.py
--rw-r--r--   0 runner    (1001) docker     (127)     3586 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/stock_indicators/indicators/common/candles.py
--rw-r--r--   0 runner    (1001) docker     (127)     2489 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/stock_indicators/indicators/common/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)      836 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/stock_indicators/indicators/common/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2802 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/stock_indicators/indicators/common/quote.py
--rw-r--r--   0 runner    (1001) docker     (127)     3644 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/stock_indicators/indicators/common/results.py
--rw-r--r--   0 runner    (1001) docker     (127)     2844 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/stock_indicators/indicators/connors_rsi.py
--rw-r--r--   0 runner    (1001) docker     (127)     2941 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/stock_indicators/indicators/correlation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1797 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/stock_indicators/indicators/dema.py
--rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/stock_indicators/indicators/doji.py
--rw-r--r--   0 runner    (1001) docker     (127)     2738 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/stock_indicators/indicators/donchian.py
--rw-r--r--   0 runner    (1001) docker     (127)     1880 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/stock_indicators/indicators/dpo.py
--rw-r--r--   0 runner    (1001) docker     (127)     2234 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/stock_indicators/indicators/elder_ray.py
--rw-r--r--   0 runner    (1001) docker     (127)     1955 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/stock_indicators/indicators/ema.py
--rw-r--r--   0 runner    (1001) docker     (127)     1877 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/stock_indicators/indicators/epma.py
--rw-r--r--   0 runner    (1001) docker     (127)     2282 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/stock_indicators/indicators/fcb.py
--rw-r--r--   0 runner    (1001) docker     (127)     2075 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/stock_indicators/indicators/fisher_transform.py
--rw-r--r--   0 runner    (1001) docker     (127)     1867 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/stock_indicators/indicators/force_index.py
--rw-r--r--   0 runner    (1001) docker     (127)     3222 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/stock_indicators/indicators/fractal.py
--rw-r--r--   0 runner    (1001) docker     (127)     2913 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/stock_indicators/indicators/gator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2516 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/stock_indicators/indicators/heikin_ashi.py
--rw-r--r--   0 runner    (1001) docker     (127)     1804 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/stock_indicators/indicators/hma.py
--rw-r--r--   0 runner    (1001) docker     (127)     2263 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/stock_indicators/indicators/ht_trendline.py
--rw-r--r--   0 runner    (1001) docker     (127)     1886 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/stock_indicators/indicators/hurst.py
--rw-r--r--   0 runner    (1001) docker     (127)     4806 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/stock_indicators/indicators/ichimoku.py
--rw-r--r--   0 runner    (1001) docker     (127)     2556 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/stock_indicators/indicators/kama.py
--rw-r--r--   0 runner    (1001) docker     (127)     2795 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/stock_indicators/indicators/keltner.py
--rw-r--r--   0 runner    (1001) docker     (127)     2329 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/stock_indicators/indicators/kvo.py
--rw-r--r--   0 runner    (1001) docker     (127)     2737 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/stock_indicators/indicators/ma_envelopes.py
--rw-r--r--   0 runner    (1001) docker     (127)     3138 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/stock_indicators/indicators/macd.py
--rw-r--r--   0 runner    (1001) docker     (127)     2145 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/stock_indicators/indicators/mama.py
--rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/stock_indicators/indicators/marubozu.py
--rw-r--r--   0 runner    (1001) docker     (127)     1794 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/stock_indicators/indicators/mfi.py
--rw-r--r--   0 runner    (1001) docker     (127)     1871 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/stock_indicators/indicators/obv.py
--rw-r--r--   0 runner    (1001) docker     (127)     3212 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/stock_indicators/indicators/parabolic_sar.py
--rw-r--r--   0 runner    (1001) docker     (127)     3854 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/stock_indicators/indicators/pivot_points.py
--rw-r--r--   0 runner    (1001) docker     (127)     3889 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/stock_indicators/indicators/pivots.py
--rw-r--r--   0 runner    (1001) docker     (127)     2294 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/stock_indicators/indicators/pmo.py
--rw-r--r--   0 runner    (1001) docker     (127)     2782 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/stock_indicators/indicators/prs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2556 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/stock_indicators/indicators/pvo.py
--rw-r--r--   0 runner    (1001) docker     (127)     4055 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/stock_indicators/indicators/renko.py
--rw-r--r--   0 runner    (1001) docker     (127)     4579 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/stock_indicators/indicators/roc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4092 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/stock_indicators/indicators/rolling_pivots.py
--rw-r--r--   0 runner    (1001) docker     (127)     1862 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/stock_indicators/indicators/rsi.py
--rw-r--r--   0 runner    (1001) docker     (127)     2740 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/stock_indicators/indicators/slope.py
--rw-r--r--   0 runner    (1001) docker     (127)     4020 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/stock_indicators/indicators/sma.py
--rw-r--r--   0 runner    (1001) docker     (127)     2578 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/stock_indicators/indicators/smi.py
--rw-r--r--   0 runner    (1001) docker     (127)     1829 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/stock_indicators/indicators/smma.py
--rw-r--r--   0 runner    (1001) docker     (127)     2896 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/stock_indicators/indicators/starc_bands.py
--rw-r--r--   0 runner    (1001) docker     (127)     2116 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/stock_indicators/indicators/stc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2523 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/stock_indicators/indicators/stdev.py
--rw-r--r--   0 runner    (1001) docker     (127)     2866 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/stock_indicators/indicators/stdev_channels.py
--rw-r--r--   0 runner    (1001) docker     (127)     2736 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/stock_indicators/indicators/stoch.py
--rw-r--r--   0 runner    (1001) docker     (127)     2446 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/stock_indicators/indicators/stoch_rsi.py
--rw-r--r--   0 runner    (1001) docker     (127)     2753 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/stock_indicators/indicators/super_trend.py
--rw-r--r--   0 runner    (1001) docker     (127)     1821 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/stock_indicators/indicators/t3.py
--rw-r--r--   0 runner    (1001) docker     (127)     1868 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/stock_indicators/indicators/tema.py
--rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/stock_indicators/indicators/tr.py
--rw-r--r--   0 runner    (1001) docker     (127)     2357 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/stock_indicators/indicators/trix.py
--rw-r--r--   0 runner    (1001) docker     (127)     2302 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/stock_indicators/indicators/tsi.py
--rw-r--r--   0 runner    (1001) docker     (127)     1874 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/stock_indicators/indicators/ulcer_index.py
--rw-r--r--   0 runner    (1001) docker     (127)     2285 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/stock_indicators/indicators/ultimate.py
--rw-r--r--   0 runner    (1001) docker     (127)     2689 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/stock_indicators/indicators/volatility_stop.py
--rw-r--r--   0 runner    (1001) docker     (127)     2048 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/stock_indicators/indicators/vortex.py
--rw-r--r--   0 runner    (1001) docker     (127)     2541 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/stock_indicators/indicators/vwap.py
--rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/stock_indicators/indicators/vwma.py
--rw-r--r--   0 runner    (1001) docker     (127)     1978 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/stock_indicators/indicators/williams_r.py
--rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/stock_indicators/indicators/wma.py
--rw-r--r--   0 runner    (1001) docker     (127)     2926 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/stock_indicators/indicators/zig_zag.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 13:33:23.993917 stock-indicators-1.2.1/stock_indicators.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4295 2024-03-07 13:33:23.000000 stock-indicators-1.2.1/stock_indicators.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10597 2024-03-07 13:33:23.000000 stock-indicators-1.2.1/stock_indicators.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-07 13:33:23.000000 stock-indicators-1.2.1/stock_indicators.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-03-07 13:33:23.000000 stock-indicators-1.2.1/stock_indicators.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-03-07 13:33:23.000000 stock-indicators-1.2.1/stock_indicators.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 13:33:23.993917 stock-indicators-1.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 13:33:23.993917 stock-indicators-1.2.1/tests/common/
--rw-r--r--   0 runner    (1001) docker     (127)     1972 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/tests/common/test_candle.py
--rw-r--r--   0 runner    (1001) docker     (127)      846 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/tests/common/test_common.py
--rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/tests/common/test_cstypes.py
--rw-r--r--   0 runner    (1001) docker     (127)     2056 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/tests/common/test_indicator_results.py
--rw-r--r--   0 runner    (1001) docker     (127)      997 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/tests/common/test_type_compatibility.py
--rw-r--r--   0 runner    (1001) docker     (127)     5563 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2233 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/tests/test_adl.py
--rw-r--r--   0 runner    (1001) docker     (127)     1993 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/tests/test_adx.py
--rw-r--r--   0 runner    (1001) docker     (127)     3454 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/tests/test_alligator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1571 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/tests/test_alma.py
--rw-r--r--   0 runner    (1001) docker     (127)     1843 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/tests/test_aroon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1709 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/tests/test_atr.py
--rw-r--r--   0 runner    (1001) docker     (127)     1540 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/tests/test_awesome.py
--rw-r--r--   0 runner    (1001) docker     (127)     1666 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/tests/test_basic_quote.py
--rw-r--r--   0 runner    (1001) docker     (127)     4735 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/tests/test_beta.py
--rw-r--r--   0 runner    (1001) docker     (127)     2439 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/tests/test_bollinger_bands.py
--rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/tests/test_bop.py
--rw-r--r--   0 runner    (1001) docker     (127)      944 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/tests/test_cci.py
--rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/tests/test_chaikin_oscillator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/tests/test_chandelier.py
--rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/tests/test_chop.py
--rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/tests/test_cmf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2378 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/tests/test_connors_rsi.py
--rw-r--r--   0 runner    (1001) docker     (127)     1783 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/tests/test_correlation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/tests/test_dema.py
--rw-r--r--   0 runner    (1001) docker     (127)     1774 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/tests/test_doji.py
--rw-r--r--   0 runner    (1001) docker     (127)     2534 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/tests/test_donchian.py
--rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/tests/test_dpo.py
--rw-r--r--   0 runner    (1001) docker     (127)     2223 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/tests/test_elder_ray.py
--rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/tests/test_ema.py
--rw-r--r--   0 runner    (1001) docker     (127)     1283 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/tests/test_epma.py
--rw-r--r--   0 runner    (1001) docker     (127)     1844 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/tests/test_fcb.py
--rw-r--r--   0 runner    (1001) docker     (127)     2169 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/tests/test_fisher_transform.py
--rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/tests/test_force_index.py
--rw-r--r--   0 runner    (1001) docker     (127)     2665 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/tests/test_fractal.py
--rw-r--r--   0 runner    (1001) docker     (127)     3381 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/tests/test_gator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/tests/test_heikin_ashi.py
--rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/tests/test_hma.py
--rw-r--r--   0 runner    (1001) docker     (127)     2611 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/tests/test_ht_trendline.py
--rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/tests/test_hurst.py
--rw-r--r--   0 runner    (1001) docker     (127)     3125 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/tests/test_ichimoku.py
--rw-r--r--   0 runner    (1001) docker     (127)     2609 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/tests/test_kama.py
--rw-r--r--   0 runner    (1001) docker     (127)     2820 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/tests/test_keltner.py
--rw-r--r--   0 runner    (1001) docker     (127)     2409 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/tests/test_kvo.py
--rw-r--r--   0 runner    (1001) docker     (127)     8555 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/tests/test_ma_envelopes.py
--rw-r--r--   0 runner    (1001) docker     (127)     2262 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/tests/test_macd.py
--rw-r--r--   0 runner    (1001) docker     (127)     2291 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/tests/test_mama.py
--rw-r--r--   0 runner    (1001) docker     (127)     1689 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/tests/test_marubozu.py
--rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/tests/test_mfi.py
--rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/tests/test_obv.py
--rw-r--r--   0 runner    (1001) docker     (127)     2668 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/tests/test_parabolic_sar.py
--rw-r--r--   0 runner    (1001) docker     (127)    13490 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/tests/test_pivot_points.py
--rw-r--r--   0 runner    (1001) docker     (127)     3803 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/tests/test_pivots.py
--rw-r--r--   0 runner    (1001) docker     (127)     1732 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/tests/test_pmo.py
--rw-r--r--   0 runner    (1001) docker     (127)     2104 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/tests/test_prs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2660 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/tests/test_pvo.py
--rw-r--r--   0 runner    (1001) docker     (127)     3856 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/tests/test_renko.py
--rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/tests/test_roc.py
--rw-r--r--   0 runner    (1001) docker     (127)    13157 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/tests/test_rolling_pivots.py
--rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/tests/test_rsi.py
--rw-r--r--   0 runner    (1001) docker     (127)     2152 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/tests/test_slope.py
--rw-r--r--   0 runner    (1001) docker     (127)     2731 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/tests/test_sma.py
--rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/tests/test_sma_extended.py
--rw-r--r--   0 runner    (1001) docker     (127)     3280 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/tests/test_smi.py
--rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/tests/test_smma.py
--rw-r--r--   0 runner    (1001) docker     (127)     2988 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/tests/test_starc_bands.py
--rw-r--r--   0 runner    (1001) docker     (127)     1826 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/tests/test_stc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3261 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/tests/test_stdev.py
--rw-r--r--   0 runner    (1001) docker     (127)     4235 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/tests/test_stdev_channels.py
--rw-r--r--   0 runner    (1001) docker     (127)     3069 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/tests/test_stoch.py
--rw-r--r--   0 runner    (1001) docker     (127)     3297 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/tests/test_stoch_rsi.py
--rw-r--r--   0 runner    (1001) docker     (127)     2267 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/tests/test_super_trend.py
--rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/tests/test_t3.py
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/tests/test_tema.py
--rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/tests/test_tr.py
--rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/tests/test_trix.py
--rw-r--r--   0 runner    (1001) docker     (127)     2369 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/tests/test_tsi.py
--rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/tests/test_ulcer_index.py
--rw-r--r--   0 runner    (1001) docker     (127)     1649 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/tests/test_ultimate.py
--rw-r--r--   0 runner    (1001) docker     (127)     2696 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/tests/test_volatility_stop.py
--rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/tests/test_vortex.py
--rw-r--r--   0 runner    (1001) docker     (127)     3590 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/tests/test_vwap.py
--rw-r--r--   0 runner    (1001) docker     (127)     1554 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/tests/test_vwma.py
--rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/tests/test_williams_r.py
--rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/tests/test_wma.py
--rw-r--r--   0 runner    (1001) docker     (127)     5403 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/tests/test_zig_zag.py
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-03-07 13:33:16.000000 stock-indicators-1.2.1/tests/utiltest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:40:11.765451 stock_indicators-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (127)     2518 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:40:11.693450 stock_indicators-1.3.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)     5311 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/.github/CODE_OF_CONDUCT.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:40:11.697450 stock_indicators-1.3.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/.github/SECURITY.md
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:40:11.697450 stock_indicators-1.3.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2186 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/.github/workflows/deploy-package.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1871 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/.github/workflows/deploy-website.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2984 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/.github/workflows/lint-pull-request.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/.github/workflows/lock-issue-pr.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/.github/workflows/test-docs-a11y.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2067 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/.github/workflows/test-docs-links.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/.github/workflows/test-indicators-all-env.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/.github/workflows/test-indicators-coverage.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1942 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/.github/workflows/test-indicators.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1854 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4277 2024-05-06 11:40:11.765451 stock_indicators-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1709 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:40:11.697450 stock_indicators-1.3.0/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/benchmarks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2024 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/benchmarks/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8016 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/benchmarks/test_benchmark_indicators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:40:11.697450 stock_indicators-1.3.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:40:11.701450 stock_indicators-1.3.0/docs/.offline/
+-rw-r--r--   0 runner    (1001) docker     (127)  1336525 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/docs/.offline/social-banner.pptx
+-rw-r--r--   0 runner    (1001) docker     (127)     2013 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/docs/.offline/social-banner.svg
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/docs/.pa11yci
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/docs/404.html
+-rw-r--r--   0 runner    (1001) docker     (127)      544 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/docs/GemFile
+-rw-r--r--   0 runner    (1001) docker     (127)     8376 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/docs/GemFile.lock
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/docs/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/docs/_config.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:40:11.701450 stock_indicators-1.3.0/docs/_data/
+-rw-r--r--   0 runner    (1001) docker     (127)     1924 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/docs/_data/aliases.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/docs/_data/categories.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:40:11.701450 stock_indicators-1.3.0/docs/_includes/
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/docs/_includes/candle-result.md
+-rw-r--r--   0 runner    (1001) docker     (127)      514 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/docs/_includes/candlepart-options.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/docs/_includes/cyclotron.html
+-rw-r--r--   0 runner    (1001) docker     (127)      533 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/docs/_includes/footer.html
+-rw-r--r--   0 runner    (1001) docker     (127)     5297 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/docs/_includes/head-style.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1741 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/docs/_includes/head.html
+-rw-r--r--   0 runner    (1001) docker     (127)      849 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/docs/_includes/header.html
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/docs/_includes/scripts.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:40:11.717450 stock_indicators-1.3.0/docs/_indicators/
+-rw-r--r--   0 runner    (1001) docker     (127)     2995 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/docs/_indicators/Adl.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3309 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/docs/_indicators/Adx.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3982 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/docs/_indicators/Alligator.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3069 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/docs/_indicators/Alma.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2790 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/docs/_indicators/Aroon.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3297 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/docs/_indicators/Atr.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2925 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/docs/_indicators/Awesome.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4503 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/docs/_indicators/Beta.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3645 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/docs/_indicators/BollingerBands.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2748 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/docs/_indicators/Bop.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2676 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/docs/_indicators/Cci.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3664 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/docs/_indicators/ChaikinOsc.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3403 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/docs/_indicators/Chandelier.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2628 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/docs/_indicators/Chop.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2864 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/docs/_indicators/Cmf.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3718 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/docs/_indicators/ConnorsRsi.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3711 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/docs/_indicators/Correlation.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3099 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/docs/_indicators/Dema.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2827 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/docs/_indicators/Doji.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3139 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/docs/_indicators/Donchian.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2773 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/docs/_indicators/Dpo.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3262 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/docs/_indicators/ElderRay.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3379 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/docs/_indicators/Ema.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2699 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/docs/_indicators/Epma.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2966 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/docs/_indicators/Fcb.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3066 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/docs/_indicators/FisherTransform.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3081 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/docs/_indicators/ForceIndex.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3646 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/docs/_indicators/Fractal.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3303 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/docs/_indicators/Gator.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2761 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/docs/_indicators/HeikinAshi.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2664 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/docs/_indicators/Hma.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3122 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/docs/_indicators/HtTrendline.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3117 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/docs/_indicators/Hurst.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4327 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/docs/_indicators/Ichimoku.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3722 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/docs/_indicators/Kama.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3686 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/docs/_indicators/Keltner.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3384 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/docs/_indicators/Kvo.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4533 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/docs/_indicators/MaEnvelopes.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3889 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/docs/_indicators/Macd.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3027 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/docs/_indicators/Mama.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2839 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/docs/_indicators/Marubozu.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2595 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/docs/_indicators/Mfi.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2893 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/docs/_indicators/Obv.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3538 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/docs/_indicators/ParabolicSar.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4670 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/docs/_indicators/PivotPoints.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4660 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/docs/_indicators/Pivots.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3151 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/docs/_indicators/Pmo.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3941 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/docs/_indicators/Prs.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3579 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/docs/_indicators/Pvo.md
+-rw-r--r--   0 runner    (1001) docker     (127)     6188 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/docs/_indicators/Renko.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4665 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/docs/_indicators/Roc.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4394 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/docs/_indicators/RollingPivots.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3213 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/docs/_indicators/Rsi.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3510 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/docs/_indicators/Slope.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3684 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/docs/_indicators/Sma.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3317 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/docs/_indicators/Smi.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3196 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/docs/_indicators/Smma.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3695 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/docs/_indicators/StarcBands.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3372 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/docs/_indicators/Stc.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3285 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/docs/_indicators/StdDev.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3754 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/docs/_indicators/StdDevChannels.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4393 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/docs/_indicators/Stoch.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4273 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/docs/_indicators/StochRsi.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3739 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/docs/_indicators/SuperTrend.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3192 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/docs/_indicators/T3.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3444 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/docs/_indicators/Tema.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3403 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/docs/_indicators/Trix.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3409 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/docs/_indicators/Tsi.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2670 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/docs/_indicators/UlcerIndex.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3020 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/docs/_indicators/Ultimate.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4022 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/docs/_indicators/VolatilityStop.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2829 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/docs/_indicators/Vortex.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3375 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/docs/_indicators/Vwap.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2578 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/docs/_indicators/Vwma.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2846 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/docs/_indicators/WilliamsR.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2980 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/docs/_indicators/Wma.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4173 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/docs/_indicators/ZigZag.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:40:11.717450 stock_indicators-1.3.0/docs/_layouts/
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/docs/_layouts/base.html
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/docs/_layouts/indicator.html
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/docs/_layouts/page.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:40:11.717450 stock_indicators-1.3.0/docs/assets/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:40:11.717450 stock_indicators-1.3.0/docs/assets/css/
+-rw-r--r--   0 runner    (1001) docker     (127)     7485 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/docs/assets/css/normalize.css
+-rw-r--r--   0 runner    (1001) docker     (127)     2903 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/docs/assets/css/rouge-github.css
+-rw-r--r--   0 runner    (1001) docker     (127)     9652 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/docs/assets/css/style.scss
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:40:11.721450 stock_indicators-1.3.0/docs/assets/icons/
+-rw-r--r--   0 runner    (1001) docker     (127)     6223 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/docs/assets/icons/android-chrome-192x192.png
+-rw-r--r--   0 runner    (1001) docker     (127)    15305 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/docs/assets/icons/android-chrome-512x512.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3862 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/docs/assets/icons/apple-touch-icon.png
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/docs/assets/icons/browserconfig.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      973 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/docs/assets/icons/favicon-16x16.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/docs/assets/icons/favicon-32x32.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7352 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/docs/assets/icons/maskable_icon_x192.png
+-rw-r--r--   0 runner    (1001) docker     (127)    21568 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/docs/assets/icons/maskable_icon_x512.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3711 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/docs/assets/icons/mstile-144x144.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3785 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/docs/assets/icons/mstile-150x150.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3924 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/docs/assets/icons/mstile-310x150.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6454 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/docs/assets/icons/mstile-310x310.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2972 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/docs/assets/icons/mstile-70x70.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6147 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/docs/assets/icons/safari-pinned-tab.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:40:11.721450 stock_indicators-1.3.0/docs/assets/js/
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/docs/assets/js/ga.js
+-rw-r--r--   0 runner    (1001) docker     (127)     7889 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/docs/assets/js/lazysizes.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/docs/assets/manifest.json
+-rw-r--r--   0 runner    (1001) docker     (127)    38959 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/docs/assets/social-banner.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8782 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/docs/contributing.md
+-rw-r--r--   0 runner    (1001) docker     (127)    15086 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/docs/favicon.ico
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:40:11.721450 stock_indicators-1.3.0/docs/pages/
+-rw-r--r--   0 runner    (1001) docker     (127)    14091 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/docs/pages/guide.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4674 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/docs/pages/home.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1700 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/docs/pages/indicators.html
+-rw-r--r--   0 runner    (1001) docker     (127)    34393 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/docs/pages/performance.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3576 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/docs/pages/utilities.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3140 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:40:11.693450 stock_indicators-1.3.0/samples/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:40:11.729450 stock_indicators-1.3.0/samples/quotes/
+-rw-r--r--   0 runner    (1001) docker     (127)    32824 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/samples/quotes/Bad.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    75494 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/samples/quotes/Bitcoin.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    28127 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/samples/quotes/Compare.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    26480 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/samples/quotes/Default.csv
+-rw-r--r--   0 runner    (1001) docker     (127)  2350932 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/samples/quotes/History.xlsx
+-rw-r--r--   0 runner    (1001) docker     (127)    94960 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/samples/quotes/Intraday.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   909185 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/samples/quotes/Longest.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   332796 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/samples/quotes/Longish.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   357981 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/samples/quotes/MSFT.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    53463 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/samples/quotes/Max.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    24574 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/samples/quotes/Mismatch.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    22595 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/samples/quotes/Penny.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   411660 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/samples/quotes/SPX.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   132770 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/samples/quotes/TooBig.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    33255 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/samples/quotes/ZigZag.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:40:11.733451 stock_indicators-1.3.0/samples/zig_zag/
+-rw-r--r--   0 runner    (1001) docker     (127)    83092 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/samples/zig_zag/data.ethusdt.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3045 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/samples/zig_zag/data.issue632.json
+-rw-r--r--   0 runner    (1001) docker     (127)    55992 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/samples/zig_zag/data.schrodinger.json
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 11:40:11.765451 stock_indicators-1.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:40:11.733451 stock_indicators-1.3.0/stock_indicators/
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/stock_indicators/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:40:11.733451 stock_indicators-1.3.0/stock_indicators/_cslib/
+-rw-r--r--   0 runner    (1001) docker     (127)     2134 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/stock_indicators/_cslib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:40:11.733451 stock_indicators-1.3.0/stock_indicators/_cslib/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)   219648 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/stock_indicators/_cslib/lib/Skender.Stock.Indicators.dll
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:40:11.733451 stock_indicators-1.3.0/stock_indicators/_cstypes/
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/stock_indicators/_cstypes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/stock_indicators/_cstypes/datetime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/stock_indicators/_cstypes/decimal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/stock_indicators/_cstypes/list.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:40:11.749451 stock_indicators-1.3.0/stock_indicators/indicators/
+-rw-r--r--   0 runner    (1001) docker     (127)     2945 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/stock_indicators/indicators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2424 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/stock_indicators/indicators/adl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2399 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/stock_indicators/indicators/adx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3208 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/stock_indicators/indicators/alligator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2133 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/stock_indicators/indicators/alma.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2247 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/stock_indicators/indicators/aroon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2135 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/stock_indicators/indicators/atr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2971 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/stock_indicators/indicators/atr_stop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2303 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/stock_indicators/indicators/awesome.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1927 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/stock_indicators/indicators/basic_quotes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3364 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/stock_indicators/indicators/beta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3144 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/stock_indicators/indicators/bollinger_bands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1895 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/stock_indicators/indicators/bop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1879 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/stock_indicators/indicators/cci.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2764 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/stock_indicators/indicators/chaikin_oscillator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2415 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/stock_indicators/indicators/chandelier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1887 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/stock_indicators/indicators/chop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2296 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/stock_indicators/indicators/cmf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1864 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/stock_indicators/indicators/cmo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:40:11.749451 stock_indicators-1.3.0/stock_indicators/indicators/common/
+-rw-r--r--   0 runner    (1001) docker     (127)      543 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/stock_indicators/indicators/common/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:40:11.749451 stock_indicators-1.3.0/stock_indicators/indicators/common/_contrib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/stock_indicators/indicators/common/_contrib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/stock_indicators/indicators/common/_contrib/enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/stock_indicators/indicators/common/_contrib/type_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3462 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/stock_indicators/indicators/common/candles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2489 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/stock_indicators/indicators/common/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1652 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/stock_indicators/indicators/common/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2802 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/stock_indicators/indicators/common/quote.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3614 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/stock_indicators/indicators/common/results.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2874 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/stock_indicators/indicators/connors_rsi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2971 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/stock_indicators/indicators/correlation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/stock_indicators/indicators/dema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/stock_indicators/indicators/doji.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2768 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/stock_indicators/indicators/donchian.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/stock_indicators/indicators/dpo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1943 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/stock_indicators/indicators/dynamic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2264 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/stock_indicators/indicators/elder_ray.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1985 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/stock_indicators/indicators/ema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1907 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/stock_indicators/indicators/epma.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2312 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/stock_indicators/indicators/fcb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2159 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/stock_indicators/indicators/fisher_transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1897 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/stock_indicators/indicators/force_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3306 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/stock_indicators/indicators/fractal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2946 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/stock_indicators/indicators/gator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2516 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/stock_indicators/indicators/heikin_ashi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1834 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/stock_indicators/indicators/hma.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2293 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/stock_indicators/indicators/ht_trendline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1916 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/stock_indicators/indicators/hurst.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4890 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/stock_indicators/indicators/ichimoku.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2586 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/stock_indicators/indicators/kama.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2825 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/stock_indicators/indicators/keltner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2359 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/stock_indicators/indicators/kvo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2821 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/stock_indicators/indicators/ma_envelopes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3168 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/stock_indicators/indicators/macd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/stock_indicators/indicators/mama.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/stock_indicators/indicators/marubozu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/stock_indicators/indicators/mfi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1955 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/stock_indicators/indicators/obv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3242 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/stock_indicators/indicators/parabolic_sar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3854 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/stock_indicators/indicators/pivot_points.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3973 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/stock_indicators/indicators/pivots.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2324 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/stock_indicators/indicators/pmo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2866 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/stock_indicators/indicators/prs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2586 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/stock_indicators/indicators/pvo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4055 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/stock_indicators/indicators/renko.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4624 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/stock_indicators/indicators/roc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4092 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/stock_indicators/indicators/rolling_pivots.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/stock_indicators/indicators/rsi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2770 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/stock_indicators/indicators/slope.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4061 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/stock_indicators/indicators/sma.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2608 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/stock_indicators/indicators/smi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1859 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/stock_indicators/indicators/smma.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2926 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/stock_indicators/indicators/starc_bands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2146 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/stock_indicators/indicators/stc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2553 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/stock_indicators/indicators/stdev.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2896 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/stock_indicators/indicators/stdev_channels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3321 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/stock_indicators/indicators/stoch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2476 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/stock_indicators/indicators/stoch_rsi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2783 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/stock_indicators/indicators/super_trend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1905 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/stock_indicators/indicators/t3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/stock_indicators/indicators/tema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/stock_indicators/indicators/tr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2387 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/stock_indicators/indicators/trix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2332 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/stock_indicators/indicators/tsi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1904 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/stock_indicators/indicators/ulcer_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2315 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/stock_indicators/indicators/ultimate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2719 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/stock_indicators/indicators/volatility_stop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2078 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/stock_indicators/indicators/vortex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2571 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/stock_indicators/indicators/vwap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/stock_indicators/indicators/vwma.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2008 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/stock_indicators/indicators/williams_r.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2118 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/stock_indicators/indicators/wma.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3010 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/stock_indicators/indicators/zig_zag.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:40:11.765451 stock_indicators-1.3.0/stock_indicators.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4277 2024-05-06 11:40:11.000000 stock_indicators-1.3.0/stock_indicators.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10856 2024-05-06 11:40:11.000000 stock_indicators-1.3.0/stock_indicators.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 11:40:11.000000 stock_indicators-1.3.0/stock_indicators.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-06 11:40:11.000000 stock_indicators-1.3.0/stock_indicators.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-06 11:40:11.000000 stock_indicators-1.3.0/stock_indicators.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:40:11.765451 stock_indicators-1.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:40:11.765451 stock_indicators-1.3.0/tests/common/
+-rw-r--r--   0 runner    (1001) docker     (127)     1972 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/tests/common/test_candle.py
+-rw-r--r--   0 runner    (1001) docker     (127)      846 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/tests/common/test_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/tests/common/test_cstypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2271 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/tests/common/test_indicator_results.py
+-rw-r--r--   0 runner    (1001) docker     (127)      997 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/tests/common/test_type_compatibility.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5563 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2639 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/tests/test_adl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/tests/test_adx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3768 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/tests/test_alligator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/tests/test_alma.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2128 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/tests/test_aroon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2026 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/tests/test_atr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3679 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/tests/test_atr_stop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/tests/test_awesome.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1666 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/tests/test_basic_quote.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5197 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/tests/test_beta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2968 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/tests/test_bollinger_bands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/tests/test_bop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/tests/test_cci.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/tests/test_chaikin_oscillator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/tests/test_chandelier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/tests/test_chop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2169 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/tests/test_cmf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/tests/test_cmo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2821 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/tests/test_connors_rsi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2091 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/tests/test_correlation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1353 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/tests/test_dema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1774 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/tests/test_doji.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2931 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/tests/test_donchian.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/tests/test_dpo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/tests/test_dynamic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2558 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/tests/test_elder_ray.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1980 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/tests/test_ema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1493 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/tests/test_epma.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2115 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/tests/test_fcb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2449 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/tests/test_fisher_transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/tests/test_force_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2930 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/tests/test_fractal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3745 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/tests/test_gator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/tests/test_heikin_ashi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1430 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/tests/test_hma.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2893 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/tests/test_ht_trendline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/tests/test_hurst.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3586 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/tests/test_ichimoku.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2892 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/tests/test_kama.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3223 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/tests/test_keltner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2695 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/tests/test_kvo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8935 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/tests/test_ma_envelopes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2600 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/tests/test_macd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2545 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/tests/test_mama.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1689 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/tests/test_marubozu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1801 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/tests/test_mfi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1983 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/tests/test_obv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2935 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/tests/test_parabolic_sar.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13490 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/tests/test_pivot_points.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4244 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/tests/test_pivots.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2000 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/tests/test_pmo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2464 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/tests/test_prs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2980 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/tests/test_pvo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3856 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/tests/test_renko.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2495 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/tests/test_roc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13157 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/tests/test_rolling_pivots.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2040 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/tests/test_rsi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2597 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/tests/test_slope.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2937 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/tests/test_sma.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1871 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/tests/test_sma_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3552 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/tests/test_smi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1875 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/tests/test_smma.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3348 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/tests/test_starc_bands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2045 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/tests/test_stc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3623 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/tests/test_stdev.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4637 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/tests/test_stdev_channels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5323 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/tests/test_stoch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3590 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/tests/test_stoch_rsi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2593 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/tests/test_super_trend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1595 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/tests/test_t3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/tests/test_tema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/tests/test_tr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1999 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/tests/test_trix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2615 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/tests/test_tsi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/tests/test_ulcer_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1848 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/tests/test_ultimate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2939 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/tests/test_volatility_stop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1998 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/tests/test_vortex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3965 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/tests/test_vwap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1767 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/tests/test_vwma.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/tests/test_williams_r.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1428 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/tests/test_wma.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5803 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/tests/test_zig_zag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-05-06 11:40:02.000000 stock_indicators-1.3.0/tests/utiltest.py
```

### Comparing `stock-indicators-1.2.1/.github/CODE_OF_CONDUCT.md` & `stock_indicators-1.3.0/.github/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `stock-indicators-1.2.1/.github/PULL_REQUEST_TEMPLATE.md` & `stock_indicators-1.3.0/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `stock-indicators-1.2.1/.github/workflows/deploy.yml` & `stock_indicators-1.3.0/.github/workflows/deploy-package.yml`

 * *Files 12% similar despite different names*

```diff
@@ -1,96 +1,97 @@
 # ref: https://packaging.python.org/en/latest/guides/publishing-package-distribution-releases-using-github-actions-ci-cd-workflows
 
-name: Build and Publish
+name: Deploy PyPI package
 
 on:
   push:
     branches:
       - main
-    tags: 
+    tags:
       - '[0-9]+.[0-9]+.[0-9]+'
 
 jobs:
 
   # production build
   build:
-    name: Build distribution 📦
+    name: Create package 📦
     runs-on: ubuntu-latest
 
     steps:
 
-    - uses: actions/checkout@v4
+    - name: Checkout source
+      uses: actions/checkout@v4
       with:
         fetch-tags: true
         fetch-depth: 0
 
-    - name: Set up Python
-      uses: actions/setup-python@v4
+    - name: Setup Python
+      uses: actions/setup-python@v5
       with:
         python-version: "3.x"
 
-    - name: Install pypa/build
+    - name: Build library
       run: python3 -m pip install build --user
 
-    - name: Build a binary wheel and a source tarball
+    - name: Build wheel and tarball
       run: python3 -m build
 
-    - name: Store the distribution packages
-      uses: actions/upload-artifact@v3
+    - name: Save package
+      uses: actions/upload-artifact@v4
       with:
         name: python-package-distributions
         path: dist/
 
 
   # This will be triggered only when a tag is pushed
   publish-to-pypi:
-    name: Publish to PyPI 🐍
+    name: Publish to PyPI 🐍 (pypi.org)
     if: startsWith(github.ref, 'refs/tags/')
     needs:
     - build
     runs-on: ubuntu-latest
 
     environment:
       name: pypi
       url: https://pypi.org/p/stock-indicators
 
     permissions:
       id-token: write  # IMPORTANT: mandatory for trusted publishing
 
     steps:
 
-    - name: Download all the dists
-      uses: actions/download-artifact@v3
+    - name: Download package
+      uses: actions/download-artifact@v4
       with:
         name: python-package-distributions
         path: dist/
 
-    - name: Publish distribution 📦 to PyPI
+    - name: Publish package 📦 to pypi.org
       uses: pypa/gh-action-pypi-publish@release/v1
 
 
   # This will be triggered everytime when commit is pushed on main branch
   publish-to-testpypi:
-    name: Publish to TestPyPI 🐍
+    name: Publish to PyPI 🐍 (test.pypi.org)
     needs:
     - build
     runs-on: ubuntu-latest
 
     environment:
       name: pypi-test
       url: https://test.pypi.org/p/stock-indicators
 
     permissions:
       id-token: write  # IMPORTANT: mandatory for trusted publishing
 
     steps:
 
-    - name: Download all the dists
-      uses: actions/download-artifact@v3
+    - name: Download package
+      uses: actions/download-artifact@v4
       with:
         name: python-package-distributions
         path: dist/
 
-    - name: Publish distribution 📦 to TestPyPI
+    - name: Publish package 📦 to test.pypi.org
       uses: pypa/gh-action-pypi-publish@release/v1
       with:
         repository-url: https://test.pypi.org/legacy/
```

### Comparing `stock-indicators-1.2.1/.github/workflows/docs-deploy.yml` & `stock_indicators-1.3.0/.github/workflows/deploy-website.yml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 name: Deploy website
 
-on: [workflow_dispatch]
+on: workflow_dispatch
 
 concurrency:
   group: docs-website
 
 env:
   JEKYLL_GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
 
@@ -16,15 +16,15 @@
     environment:
       name: docs-website
 
     steps:
       - name: Checkout source
         uses: actions/checkout@v4
 
-      - name: Install Ruby
+      - name: Setup Ruby
         uses: ruby/setup-ruby@v1
         with:
           working-directory: docs
           ruby-version: 3.1.3
           bundler-cache: false
 
       - name: Define tag
@@ -34,15 +34,15 @@
       - name: Replace cache markers
         uses: jacobtomlinson/gha-find-replace@v3
         with:
           find: "YYYY.MM.DD"
           replace: "${{ steps.tag.outputs.version }}"
           regex: false
 
-      - name: Install GEMs
+      - name: Setup GEMs
         working-directory: docs
         env:
           BUNDLE_GEMFILE: ${{github.workspace}}/docs/GemFile
         run: |
           pwd
           bundle install
```

### Comparing `stock-indicators-1.2.1/.github/workflows/docs-test-a11y.yml` & `stock_indicators-1.3.0/.github/workflows/test-docs-a11y.yml`

 * *Files 8% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     name: test a11y
     runs-on: ubuntu-latest
 
     steps:
       - name: Checkout source
         uses: actions/checkout@v4
 
-      - name: Install Ruby
+      - name: Setup Ruby
         uses: ruby/setup-ruby@v1
         with:
           working-directory: docs
           ruby-version: 3.1.3
           bundler-cache: false
 
       - name: Install GEMs
@@ -52,7 +52,11 @@
 
       - name: Test accessibility
         working-directory: docs
         run: |
           npx pa11y-ci \
             --sitemap http://127.0.0.1:4000/sitemap.xml \
             --sitemap-exclude "/*.pdf"
+
+      - name: Kill site (failsafe)
+        if: always()
+        run: pkill -f jekyll
```

### Comparing `stock-indicators-1.2.1/.github/workflows/docs-test-links.yml` & `stock_indicators-1.3.0/.github/workflows/test-docs-links.yml`

 * *Files 13% similar despite different names*

```diff
@@ -1,44 +1,47 @@
 name: Website
+
 on:
   pull_request:
     branches: [main]
     paths:
       - 'docs/**'
       - ".github/workflows/docs-test-links.yml"
 
 env:
   JEKYLL_GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
 
 jobs:
-  testing:
+  test:
     name: test URLs
     runs-on: ubuntu-latest
 
     steps:
       - name: Checkout source
-        uses: actions/checkout@v2
+        uses: actions/checkout@v4
 
-      - name: Install Ruby
+      - name: Setup Ruby
         uses: ruby/setup-ruby@v1
         with:
           working-directory: docs
           ruby-version: 3.1.3
           bundler-cache: false
 
       - name: Install GEMs
         working-directory: docs
         env:
           BUNDLE_GEMFILE: ${{github.workspace}}/docs/GemFile
         run: |
           pwd
           bundle install
 
-      - name: Install HTML Proofer
-        run: gem install html-proofer
+      - name: Setup HTML Proofer
+        run: |
+          gem install html-proofer
+          htmlproofer --help
 
       - name: Replace "data-src"
         uses: jacobtomlinson/gha-find-replace@v3
         with:
           find: "data-src"
           replace: "src"
           regex: false
@@ -58,15 +61,21 @@
 
       - name: Serve site
         working-directory: docs
         env:
           BUNDLE_GEMFILE: ${{github.workspace}}/docs/GemFile
         run: bundle exec jekyll serve --detach
 
+        # see help in setup step
       - name: Test for broken URLs
         working-directory: docs
         run: |
           htmlproofer _site \
             --no-enforce-https \
+            --no-check-external-hash \
             --ignore-status-codes "0,302,403,406,408,429,503,999" \
             --swap-urls "https\://python.stockindicators.dev:http\://127.0.0.1:4000" \
             --ignore-urls "/fonts.gstatic.com/"
+
+      - name: Kill site (failsafe)
+        if: always()
+        run: pkill -f jekyll
```

### Comparing `stock-indicators-1.2.1/.github/workflows/semantic-pr-linter.yml` & `stock_indicators-1.3.0/.github/workflows/lint-pull-request.yml`

 * *Files 18% similar despite different names*

```diff
@@ -1,70 +1,76 @@
-name: "Lint PR"
-
-on:
-  pull_request_target:
-    types:
-      - opened
-      - edited
-      - synchronize
-
-permissions:
-  pull-requests: write
-
-jobs:
-  main:
-    name: validate PR title
-    runs-on: ubuntu-latest
-    steps:
-      - uses: amannn/action-semantic-pull-request@v5
-        id: lint_pr_title
-        env:
-          GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
-        with:
-
-          # Configure additional validation for the subject based on a regex.
-          # We enforce that the subject starts with an uppercase character.
-          subjectPattern: ^([A-Z]).+$
-
-          # If `subjectPattern` is configured, you can use this property to override
-          # the default error message that is shown when the pattern doesn't match.
-          # The variables `subject` and `title` can be used within the message.
-          subjectPatternError: >
-            The subject "**{subject}**" found in the pull request title "*{title}*"
-            didn't match the configured pattern. Please ensure that the subject
-            starts with an uppercase character.
-
-          # If the PR contains one of these newline-delimited labels, the
-          # validation is skipped. If you want to rerun the validation when
-          # labels change, you might want to use the `labeled` and `unlabeled`
-          # event triggers in your workflow.
-          ignoreLabels: |
-            bot
-            ignore-semantic-pull-request
-
-      - uses: marocchino/sticky-pull-request-comment@v2
-        # When the previous steps fails, the workflow would stop. By adding this
-        # condition you can continue the execution with the populated error message.
-        if: always() && (steps.lint_pr_title.outputs.error_message != null)
-        with:
-          header: pr-title-lint-error
-          message: >
-            ### Hey there and thank you for opening this pull request! 👋🏼
-
-            It looks like your proposed **_Pull request title_** needs to be adjusted.
-
-            >🚩 **Error** » ${{ steps.lint_pr_title.outputs.error_message }}
-
-            #### Pull request title naming convention
-
-            Our PR title name taxonomy is `type: Subject`, where **type** is typically
-            *feat*, *fix*, or *chore*, and **subject** is a phrase (proper noun) that starts with a capitalized letter.
-            The *chore* type usually has a subject that starts with an action verb like *Add* or *Update*.
-            Examples: `feat: Admin portal login`, `fix: Divide by zero bug in SMA`, and `chore: Update user docs`.
-            See the [Conventional Commits specification](https://www.conventionalcommits.org) for more information.
-
-      # Delete a previous comment when the issue has been resolved
-      - if: ${{ steps.lint_pr_title.outputs.error_message == null }}
-        uses: marocchino/sticky-pull-request-comment@v2
-        with:
-          header: pr-title-lint-error
-          delete: true
+name: "Pull request"
+
+on:
+  pull_request_target:
+    types:
+      - opened
+      - edited
+      - synchronize
+
+permissions:
+  pull-requests: write
+
+jobs:
+  main:
+    name: lint PR title
+    runs-on: ubuntu-latest
+    steps:
+      - uses: amannn/action-semantic-pull-request@v5
+        id: lint_pr_title
+        env:
+          GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
+        with:
+
+          # Configure additional validation for the subject based on a regex.
+          # We enforce that the subject starts with an uppercase character.
+          subjectPattern: ^([A-Z]).+$
+
+          # If `subjectPattern` is configured, you can use this property to override
+          # the default error message that is shown when the pattern doesn't match.
+          # The variables `subject` and `title` can be used within the message.
+          subjectPatternError: >
+            The subject "**{subject}**" found in the pull request title "*{title}*"
+            didn't match the configured pattern. Please ensure that the subject
+            starts with an uppercase character.
+
+          # If the PR contains one of these newline-delimited labels, the
+          # validation is skipped. If you want to rerun the validation when
+          # labels change, you might want to use the `labeled` and `unlabeled`
+          # event triggers in your workflow.
+          ignoreLabels: |
+            bot
+            dependencies
+
+      - uses: marocchino/sticky-pull-request-comment@v2
+        # When the previous steps fails, the workflow would stop. By adding this
+        # condition you can continue the execution with the populated error message.
+        if: always() && (steps.lint_pr_title.outputs.error_message != null)
+        with:
+          header: pr-title-lint-error
+          message: >
+            ### Hey there and thank you for opening this pull request! 👋🏼
+
+            It looks like your proposed **_Pull request title_** needs to be adjusted.
+
+            >🚩 **Error** » ${{ steps.lint_pr_title.outputs.error_message }}
+
+            #### Pull request title naming convention
+
+            Our PR title name taxonomy is `type: Subject`, where **type** is typically
+            *feat*, *fix*, or *chore*, and **subject** is a phrase (proper noun) that starts
+            with a capitalized letter.  The *chore* type usually has a subject that starts
+            with an action verb like *Add* or *Update*. Examples:
+
+            - _feat: Admin portal login_
+            - _fix: Divide by zero bug in SMA_
+            - _chore: Update packages_
+            - _docs: Improve setup guidance_
+
+            See the [Conventional Commits specification](https://www.conventionalcommits.org) for more information.
+
+      # Delete a previous comment when the issue has been resolved
+      - if: ${{ steps.lint_pr_title.outputs.error_message == null }}
+        uses: marocchino/sticky-pull-request-comment@v2
+        with:
+          header: pr-title-lint-error
+          delete: true
```

### Comparing `stock-indicators-1.2.1/.github/workflows/test-all-env.yml` & `stock_indicators-1.3.0/.github/workflows/test-indicators-all-env.yml`

 * *Files 25% similar despite different names*

```diff
@@ -1,43 +1,46 @@
 # For more information see: https://docs.github.com/en/actions/automating-builds-and-tests/building-and-testing-python
 
-name: Run all tests
+name: Test all environments
 
 on:
   workflow_dispatch:
 
+  push:
+    branches: ["main"]
+
 permissions:
   contents: read
 
 jobs:
   test:
     runs-on: ${{ matrix.os }}
     strategy:
         matrix:
             os: [windows-latest, ubuntu-latest, macos-latest]
             python-version: ["3.8", "3.9", "3.10", "3.11", "3.12"]
-            dotnet-version: ["6.0.x", "7.0.x", "8.0.x"]
+            dotnet-version: ["6.x", "7.x", "8.x"]
 
     steps:
-      - name: Checkout Repository
-        uses: actions/checkout@v2
+      - name: Checkout source
+        uses: actions/checkout@v4
 
-      - name: Setup .NET SDK
-        uses: actions/setup-dotnet@v3
+      - name: Setup .NET
+        uses: actions/setup-dotnet@v4
         with:
           dotnet-version: ${{ matrix.dotnet-version }}
           dotnet-quality: "ga"
 
       - name: Setup Python
         uses: actions/setup-python@v5
         with:
           cache: "pip"
           python-version: ${{ matrix.python-version }}
 
-      - name: Install Dependencies
+      - name: Install requirements
         run: |
           pip install -r requirements.txt
           pip install -r requirements-test.txt
 
-      - name: Run Tests
+      - name: Test indicators
         run: |
           pytest -vr A tests
```

### Comparing `stock-indicators-1.2.1/.github/workflows/test-coverage.yml` & `stock_indicators-1.3.0/.github/workflows/test-indicators-coverage.yml`

 * *Files 6% similar despite different names*

```diff
@@ -1,42 +1,44 @@
 # For more information see: https://docs.github.com/en/actions/automating-builds-and-tests/building-and-testing-python
 
-name: Test code coverage
+name: Indicators
 
 on: ["push"]
 
 permissions:
   contents: read
 
 jobs:
   test:
+    name: code coverage
     runs-on: ubuntu-latest
 
     steps:
-      - name: Checkout Repository
-        uses: actions/checkout@v2
+      - name: Checkout source
+        uses: actions/checkout@v4
 
       - name: Setup .NET
-        uses: actions/setup-dotnet@v1
+        uses: actions/setup-dotnet@v4
         with:
           dotnet-version: 8.x
+          dotnet-quality: "ga"
 
       - name: Setup Python
-        uses: actions/setup-python@v2
+        uses: actions/setup-python@v5
         with:
           python-version: 3.12
 
-      - name: Install Dependencies
+      - name: Install requirements
         run: |
           pip install -r requirements.txt
           pip install -r requirements-test.txt
 
-      - name: Run Tests
+      - name: Test indicators
         run: |
           coverage run -m --source=stock_indicators pytest -svr A tests
           coverage xml
 
-      - name: Post coverage to Codacy
+      - name: Publish coverage to Codacy
         uses: codacy/codacy-coverage-reporter-action@v1
         with:
           project-token: ${{ secrets.CODACY_PROJECT_TOKEN }}
           coverage-reports: coverage.xml
```

### Comparing `stock-indicators-1.2.1/.gitignore` & `stock_indicators-1.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `stock-indicators-1.2.1/LICENSE` & `stock_indicators-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `stock-indicators-1.2.1/benchmarks/conftest.py` & `stock_indicators-1.3.0/benchmarks/conftest.py`

 * *Files identical despite different names*

### Comparing `stock-indicators-1.2.1/benchmarks/test_benchmark_indicators.py` & `stock_indicators-1.3.0/benchmarks/test_benchmark_indicators.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,14 +12,17 @@
 
 def test_benchmark_alma(benchmark, quotes):
     benchmark(indicators.get_alma, quotes)
 
 def test_benchmark_aroon(benchmark, quotes):
     benchmark(indicators.get_aroon, quotes)
 
+def test_benchmark_atr_stop(benchmark, quotes):
+    benchmark(indicators.get_atr_stop, quotes)
+
 def test_benchmark_atr(benchmark, quotes):
     benchmark(indicators.get_atr, quotes)
 
 def test_benchmark_awesome(benchmark, quotes):
     benchmark(indicators.get_awesome, quotes)
 
 def test_benchmark_beta(benchmark, quotes, other_quotes):
@@ -42,14 +45,17 @@
 
 def test_benchmark_chop(benchmark, quotes):
     benchmark(indicators.get_chop, quotes)
 
 def test_benchmark_cmf(benchmark, quotes):
     benchmark(indicators.get_cmf, quotes)
 
+def test_benchmark_cmo(benchmark, quotes):
+    benchmark(indicators.get_cmo, quotes, 14)
+
 def test_benchmark_connors_rsi(benchmark, quotes):
     benchmark(indicators.get_connors_rsi, quotes)
 
 def test_benchmark_correlation(benchmark, quotes, other_quotes):
     benchmark(indicators.get_correlation, quotes, other_quotes, 20)
 
 def test_benchmark_doji(benchmark, quotes):
@@ -60,14 +66,17 @@
 
 def test_benchmark_dema(benchmark, quotes):
     benchmark(indicators.get_dema, quotes, 20)
 
 def test_benchmark_dpo(benchmark, quotes):
     benchmark(indicators.get_dpo, quotes, 14)
 
+def test_benchmark_dynamic(benchmark, quotes):
+    benchmark(indicators.get_dynamic, quotes, 14)
+
 def test_benchmark_elder_ray(benchmark, quotes):
     benchmark(indicators.get_elder_ray, quotes)
 
 def test_benchmark_ema(benchmark, quotes):
     benchmark(indicators.get_ema, quotes, 20)
 
 def test_benchmark_epma(benchmark, quotes):
```

### Comparing `stock-indicators-1.2.1/docs/GemFile` & `stock_indicators-1.3.0/docs/GemFile`

 * *Files identical despite different names*

### Comparing `stock-indicators-1.2.1/docs/GemFile.lock` & `stock_indicators-1.3.0/docs/GemFile.lock`

 * *Files 1% similar despite different names*

```diff
@@ -17,39 +17,38 @@
       i18n (>= 1.6, < 2)
       minitest (>= 5.1)
       mutex_m
       tzinfo (~> 2.0)
     addressable (2.8.6)
       public_suffix (>= 2.0.2, < 6.0)
     base64 (0.2.0)
-    bigdecimal (3.1.6)
+    bigdecimal (3.1.7)
     coffee-script (2.4.1)
       coffee-script-source
       execjs
     coffee-script-source (1.12.2)
     colorator (1.1.0)
     commonmarker (0.23.10)
     concurrent-ruby (1.2.3)
     connection_pool (2.4.1)
     cssminify2 (2.0.1)
-    dnsruby (1.70.0)
+    dnsruby (1.72.1)
       simpleidn (~> 0.2.1)
-    drb (2.2.0)
-      ruby2_keywords
+    drb (2.2.1)
     em-websocket (0.5.3)
       eventmachine (>= 0.12.9)
       http_parser.rb (~> 0)
     ethon (0.16.0)
       ffi (>= 1.15.0)
     execjs (2.9.1)
     faraday (2.9.0)
       faraday-net_http (>= 2.0, < 3.2)
     faraday-net_http (3.1.0)
       net-http
-    faraday-retry (2.2.0)
+    faraday-retry (2.2.1)
       faraday (~> 2.0)
     ffi (1.16.3)
     forwardable-extended (2.6.0)
     gemoji (4.1.0)
     github-pages (231)
       github-pages-health-check (= 1.18.2)
       jekyll (= 3.9.5)
@@ -102,15 +101,15 @@
       public_suffix (>= 3.0, < 6.0)
       typhoeus (~> 1.3)
     html-pipeline (2.14.3)
       activesupport (>= 2)
       nokogiri (>= 1.4)
     htmlcompressor (0.4.0)
     http_parser.rb (0.8.0)
-    i18n (1.14.1)
+    i18n (1.14.4)
       concurrent-ruby (~> 1.0)
     jekyll (3.9.5)
       addressable (~> 2.4)
       colorator (~> 1.0)
       em-websocket (~> 0.5)
       i18n (>= 0.7, < 2)
       jekyll-sass-converter (~> 1.0)
@@ -221,52 +220,51 @@
       jekyll (>= 3.3, < 5.0)
     jekyll-watch (2.2.1)
       listen (~> 3.0)
     jemoji (0.13.0)
       gemoji (>= 3, < 5)
       html-pipeline (~> 2.2)
       jekyll (>= 3.0, < 5.0)
-    json (2.7.1)
+    json (2.7.2)
     json-minify (0.0.3)
       json (> 0)
     kramdown (2.4.0)
       rexml
     kramdown-parser-gfm (1.1.0)
       kramdown (~> 2.0)
     liquid (4.0.4)
     listen (3.9.0)
       rb-fsevent (~> 0.10, >= 0.10.3)
       rb-inotify (~> 0.9, >= 0.9.10)
     mercenary (0.3.6)
-    mini_portile2 (2.8.5)
+    mini_portile2 (2.8.6)
     minima (2.5.1)
       jekyll (>= 3.5, < 5.0)
       jekyll-feed (~> 0.9)
       jekyll-seo-tag (~> 2.1)
-    minitest (5.22.2)
+    minitest (5.22.3)
     mutex_m (0.2.0)
     net-http (0.4.1)
       uri
-    nokogiri (1.16.2)
+    nokogiri (1.16.4)
       mini_portile2 (~> 2.8.2)
       racc (~> 1.4)
     octokit (4.25.1)
       faraday (>= 1, < 3)
       sawyer (~> 0.9)
     pathutil (0.16.2)
       forwardable-extended (~> 2.6)
     posix-spawn (0.3.15)
-    public_suffix (5.0.4)
+    public_suffix (5.0.5)
     racc (1.7.3)
     rb-fsevent (0.11.2)
     rb-inotify (0.10.1)
       ffi (~> 1.0)
     rexml (3.2.6)
     rouge (3.30.0)
-    ruby2_keywords (0.0.5)
     rubyzip (2.3.2)
     safe_yaml (1.0.5)
     sass (3.7.4)
       sass-listen (~> 4.0.0)
     sass-listen (4.0.0)
       rb-fsevent (~> 0.9, >= 0.9.4)
       rb-inotify (~> 0.9, >= 0.9.7)
```

### Comparing `stock-indicators-1.2.1/docs/_config.yml` & `stock_indicators-1.3.0/docs/_config.yml`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Ref: https://jekyllrb.com/docs/usage/
 # Local dev: bundle exec jekyll serve --livereload
 
 title: Stock Indicators for Python
 tagline: "Transform price quotes into trading insights."
-repository: DaveSkender/Stock.Indicators.Python
+repository: facioquo/stock-indicators-python
 locale: en_US
 baseurl: ""
 url: "https://python.stockindicators.dev"
 
 # social media information
 image:
   path: /assets/social-banner.png
@@ -20,15 +20,15 @@
 dotnet:
   repo: "https://github.com/DaveSkender/Stock.Indicators"
   src: "https://github.com/DaveSkender/Stock.Indicators/blob/main/src"
   charts: "https://raw.githubusercontent.com/DaveSkender/Stock.Indicators/main/docs/assets/charts"
 
  # this site URL refs
 python:
-  src: "https://github.com/DaveSkender/Stock.Indicators.Python/blob/main/stock_indicators/indicators"
+  src: "https://github.com/facioquo/stock-indicators-python/blob/main/stock_indicators/indicators"
 
 clarity: false
 
 # site plugins and settings
 plugins:
   - jekyll-github-metadata
   - jekyll-seo-tag
```

### Comparing `stock-indicators-1.2.1/docs/_data/aliases.yml` & `stock_indicators-1.3.0/docs/_data/aliases.yml`

 * *Files identical despite different names*

### Comparing `stock-indicators-1.2.1/docs/_data/categories.yml` & `stock_indicators-1.3.0/docs/_data/categories.yml`

 * *Files identical despite different names*

### Comparing `stock-indicators-1.2.1/docs/_includes/candlepart-options.md` & `stock_indicators-1.3.0/docs/_includes/candlepart-options.md`

 * *Files identical despite different names*

### Comparing `stock-indicators-1.2.1/docs/_includes/cyclotron.html` & `stock_indicators-1.3.0/docs/_includes/cyclotron.html`

 * *Files identical despite different names*

### Comparing `stock-indicators-1.2.1/docs/_includes/footer.html` & `stock_indicators-1.3.0/docs/_includes/footer.html`

 * *Files identical despite different names*

### Comparing `stock-indicators-1.2.1/docs/_includes/head-style.html` & `stock_indicators-1.3.0/docs/_includes/head-style.html`

 * *Files identical despite different names*

### Comparing `stock-indicators-1.2.1/docs/_includes/head.html` & `stock_indicators-1.3.0/docs/_includes/head.html`

 * *Files identical despite different names*

### Comparing `stock-indicators-1.2.1/docs/_includes/header.html` & `stock_indicators-1.3.0/docs/_includes/header.html`

 * *Files identical despite different names*

### Comparing `stock-indicators-1.2.1/docs/_includes/scripts.html` & `stock_indicators-1.3.0/docs/_includes/scripts.html`

 * *Files identical despite different names*

### Comparing `stock-indicators-1.2.1/docs/_indicators/Adl.md` & `stock_indicators-1.3.0/docs/_indicators/Adl.md`

 * *Files 1% similar despite different names*

```diff
@@ -55,15 +55,15 @@
 
 ## Example
 
 ```python
 from stock_indicators import indicators
 
 # This method is NOT a part of the library.
-quotes = get_history_from_feed("SPY")
+quotes = get_historical_quotes("SPY")
 
 # calculate
 results = indicators.get_adl(quotes)
 ```
 
 ## About {{ page.title }}
```

### Comparing `stock-indicators-1.2.1/docs/_indicators/Adx.md` & `stock_indicators-1.3.0/docs/_indicators/Adx.md`

 * *Files 2% similar despite different names*

```diff
@@ -56,15 +56,15 @@
 
 ## Example
 
 ```python
 from stock_indicators import indicators
 
 # This method is NOT a part of the library.
-quotes = get_history_from_feed("SPY")
+quotes = get_historical_quotes("SPY")
 
 # calculate 14-period ADX
 results = indicators.get_adx(quotes, lookback_periods)
 ```
 
 ## About {{ page.title }}
```

### Comparing `stock-indicators-1.2.1/docs/_indicators/Alligator.md` & `stock_indicators-1.3.0/docs/_indicators/Alligator.md`

 * *Files 1% similar despite different names*

```diff
@@ -60,15 +60,15 @@
 
 ## Example
 
 ```python
 from stock_indicators import indicators
 
 # This method is NOT a part of the library.
-quotes = get_history_from_feed("SPY")
+quotes = get_historical_quotes("SPY")
 
 # calculate the Williams Alligator
 results = indicators.get_alligator(quotes)
 ```
 
 ## About {{ page.title }}
```

### Comparing `stock-indicators-1.2.1/docs/_indicators/Alma.md` & `stock_indicators-1.3.0/docs/_indicators/Alma.md`

 * *Files 2% similar despite different names*

```diff
@@ -53,15 +53,15 @@
 
 ## Example
 
 ```python
 from stock_indicators import indicators
 
 # This method is NOT a part of the library.
-quotes = get_history_from_feed("SPY")
+quotes = get_historical_quotes("SPY")
 
 # calculate Alma
 results = indicators.get_alma(quotes, 10, 0.5, 6)
 ```
 
 ### About {{ page.title }}
```

### Comparing `stock-indicators-1.2.1/docs/_indicators/Aroon.md` & `stock_indicators-1.3.0/docs/_indicators/Aroon.md`

 * *Files 2% similar despite different names*

```diff
@@ -53,15 +53,15 @@
 
 ## Example
 
 ```python
 from stock_indicators import indicators
 
 # This method is NOT a part of the library.
-quotes = get_history_from_feed("SPY")
+quotes = get_historical_quotes("SPY")
 
 results = indicators.get_aroon(quotes, lookback_periods)
 ```
 
 ## About {{ page.title }}
 
 Created by Tushar Chande, [Aroon](https://school.stockcharts.com/doku.php?id=technical_indicators:aroon) is a oscillator view of how long ago the new high or low price occurred over a lookback window.
```

### Comparing `stock-indicators-1.2.1/docs/_indicators/Atr.md` & `stock_indicators-1.3.0/docs/_indicators/Atr.md`

 * *Files 1% similar despite different names*

```diff
@@ -60,15 +60,15 @@
 
 ## Example
 
 ```python
 from stock_indicators import indicators
 
 # This method is NOT a part of the library.
-quotes = get_history_from_feed("SPY")
+quotes = get_historical_quotes("SPY")
 
 # calculate 14-period ATR
 results = indicators.get_atr(quotes, 14)
 ```
 
 ## About {{ page.title }}
```

### Comparing `stock-indicators-1.2.1/docs/_indicators/Awesome.md` & `stock_indicators-1.3.0/docs/_indicators/Awesome.md`

 * *Files 2% similar despite different names*

```diff
@@ -54,15 +54,15 @@
 
 ## Example
 
 ```python
 from stock_indicators import indicators
 
 # This method is NOT a part of the library.
-quotes = get_history_from_feed("SPY")
+quotes = get_historical_quotes("SPY")
 
 # calculate
 results = indicators.get_awesome(quotes, 5, 34)
 ```
 
 ## About {{ page.title }}
```

### Comparing `stock-indicators-1.2.1/docs/_indicators/Beta.md` & `stock_indicators-1.3.0/docs/_indicators/Beta.md`

 * *Files 1% similar despite different names*

```diff
@@ -72,16 +72,16 @@
 ## Example
 
 ```python
 from stock_indicators import indicators
 from stock_indicators import BetaType      # Short path, version >= 0.8.1
 
 # This method is NOT a part of the library.
-history_SPX = get_history_from_feed("SPX")
-history_TSLA = get_history_from_feed("TSLA")
+history_SPX = get_historical_quotes("SPX")
+history_TSLA = get_historical_quotes("TSLA")
 
 # calculate 20-period Beta coefficient
 results = indicators.get_beta(history_SPX, history_TSLA, 20, BetaType.STANDARD)
 ```
 
 ## About {{ page.title }}
```

### Comparing `stock-indicators-1.2.1/docs/_indicators/BollingerBands.md` & `stock_indicators-1.3.0/docs/_indicators/BollingerBands.md`

 * *Files 1% similar despite different names*

```diff
@@ -57,15 +57,15 @@
 
 ## Example
 
 ```python
 from stock_indicators import indicators
 
 # This method is NOT a part of the library.
-quotes = get_history_from_feed("SPY")
+quotes = get_historical_quotes("SPY")
 
 # calculate BollingerBands(20, 2)
 results = indicators.get_bollinger_bands(quotes, 20, 2)
 ```
 
 ## About {{ page.title }}
```

### Comparing `stock-indicators-1.2.1/docs/_indicators/Bop.md` & `stock_indicators-1.3.0/docs/_indicators/Bop.md`

 * *Files 2% similar despite different names*

```diff
@@ -52,15 +52,15 @@
 
 ## Example
 
 ```python
 from stock_indicators import indicators
 
 # This method is NOT a part of the library.
-quotes = get_history_from_feed("SPY")
+quotes = get_historical_quotes("SPY")
 
 # Calculate 14-period BOP
 results = indicators.get_bop(quotes, 14)
 ```
 
 ## About {{ page.title }}
```

### Comparing `stock-indicators-1.2.1/docs/_indicators/Cci.md` & `stock_indicators-1.3.0/docs/_indicators/Cci.md`

 * *Files 2% similar despite different names*

```diff
@@ -51,15 +51,15 @@
 
 ## Example
 
 ```python
 from stock_indicators import indicators
 
 # This method is NOT a part of the library.
-quotes = get_history_from_feed("SPY")
+quotes = get_historical_quotes("SPY")
 
 # Calculate 20-period CCI
 results = indicators.get_cci(quotes, 20)
 ```
 
 ## About {{ page.title }}
```

### Comparing `stock-indicators-1.2.1/docs/_indicators/ChaikinOsc.md` & `stock_indicators-1.3.0/docs/_indicators/ChaikinOsc.md`

 * *Files 0% similar despite different names*

```diff
@@ -59,15 +59,15 @@
 
 ## Example
 
 ```python
 from stock_indicators import indicators
 
 # This method is NOT a part of the library.
-quotes = get_history_from_feed("SPY")
+quotes = get_historical_quotes("SPY")
 
 # Calculate 20-period Chaikin Oscillator
 results = indicators.get_chaikin_osc(quotes, 20)
 ```
 
 ## About {{ page.title }}
```

### Comparing `stock-indicators-1.2.1/docs/_indicators/Chandelier.md` & `stock_indicators-1.3.0/docs/_indicators/Chandelier.md`

 * *Files 1% similar despite different names*

```diff
@@ -65,15 +65,15 @@
 ## Example
 
 ```python
 from stock_indicators import indicators
 from stock_indicators import ChandelierType     # Short path, version >= 0.8.1
 
 # This method is NOT a part of the library.
-quotes = get_history_from_feed("SPY")
+quotes = get_historical_quotes("SPY")
 
 # calculate Chandelier(22,3)
 results = indicators.get_chandelier(quotes, 22, 3, ChandelierType.LONG)
 ```
 
 ## About {{ page.title }}
```

### Comparing `stock-indicators-1.2.1/docs/_indicators/Chop.md` & `stock_indicators-1.3.0/docs/_indicators/Chop.md`

 * *Files 3% similar despite different names*

```diff
@@ -51,15 +51,15 @@
 
 ## Example
 
 ```python
 from stock_indicators import indicators
 
 # This method is NOT a part of the library.
-quotes = get_history_from_feed("SPY")
+quotes = get_historical_quotes("SPY")
 
 # Calculate CHOP(14)
 results = indicators.get_chop(quotes, 14)
 ```
 
 ## About {{ page.title }}
```

### Comparing `stock-indicators-1.2.1/docs/_indicators/Cmf.md` & `stock_indicators-1.3.0/docs/_indicators/Cmf.md`

 * *Files 2% similar despite different names*

```diff
@@ -55,15 +55,15 @@
 
 ## Example
 
 ```python
 from stock_indicators import indicators
 
 # This method is NOT a part of the library.
-quotes = get_history_from_feed("SPY")
+quotes = get_historical_quotes("SPY")
 
 # Calculate 20-period CMF
 results = indicators.get_cmf(quotes, 20)
 ```
 
 ## About {{ page.title }}
```

### Comparing `stock-indicators-1.2.1/docs/_indicators/ConnorsRsi.md` & `stock_indicators-1.3.0/docs/_indicators/ConnorsRsi.md`

 * *Files 3% similar despite different names*

```diff
@@ -58,15 +58,15 @@
 
 ## Example
 
 ```python
 from stock_indicators import indicators
 
 # This method is NOT a part of the library.
-quotes = get_history_from_feed("SPY")
+quotes = get_historical_quotes("SPY")
 
 # Calculate ConnorsRsi(3,2.100)
 results = indicators.get_connors_rsi(quotes, 3, 2, 100)
 ```
 
 ## About {{ page.title }}
```

### Comparing `stock-indicators-1.2.1/docs/_indicators/Correlation.md` & `stock_indicators-1.3.0/docs/_indicators/Correlation.md`

 * *Files 3% similar despite different names*

```diff
@@ -57,16 +57,16 @@
 
 ## Example
 
 ```python
 from stock_indicators import indicators
 
 # This method is NOT a part of the library.
-quotes_spx = get_history_from_feed("SPX")
-quotes_tsla = get_history_from_feed("TSLA")
+quotes_spx = get_historical_quotes("SPX")
+quotes_tsla = get_historical_quotes("TSLA")
 
 # Calculate 20-period Correlation
 results = indicators.get_correlation(quotes_spx, quotes_tsla, 20)
 ```
 
 ## About {{ page.title }}
```

### Comparing `stock-indicators-1.2.1/docs/_indicators/Dema.md` & `stock_indicators-1.3.0/docs/_indicators/Dema.md`

 * *Files 1% similar despite different names*

```diff
@@ -53,15 +53,15 @@
 
 ## Example
 
 ```python
 from stock_indicators import indicators
 
 # This method is NOT a part of the library.
-quotes = get_history_from_feed("SPY")
+quotes = get_historical_quotes("SPY")
 
 # calculate 20-period DEMA
 results = indicators.get_dema(quotes, 20)
 ```
 
 ## About {{ page.title }}
```

### Comparing `stock-indicators-1.2.1/docs/_indicators/Doji.md` & `stock_indicators-1.3.0/docs/_indicators/Doji.md`

 * *Files 5% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 
 ## Example
 
 ```python
 from stock_indicators import indicators
 
 # This method is NOT a part of the library.
-quotes = get_history_from_feed("SPY")
+quotes = get_historical_quotes("SPY")
 
 # Calculate
 results = indicators.get_doji(quotes);
 ```
 
 ## About {{ page.title }}
```

### Comparing `stock-indicators-1.2.1/docs/_indicators/Donchian.md` & `stock_indicators-1.3.0/docs/_indicators/Donchian.md`

 * *Files 1% similar despite different names*

```diff
@@ -55,15 +55,15 @@
 
 ## Example
 
 ```python
 from stock_indicators import indicators
 
 # This method is NOT a part of the library.
-quotes = get_history_from_feed("SPY")
+quotes = get_historical_quotes("SPY")
 
 # calculate Donchian(20)
 results = indicators.get_donchian(quotes, 20)
 ```
 
 ## About {{ page.title }}
```

### Comparing `stock-indicators-1.2.1/docs/_indicators/Dpo.md` & `stock_indicators-1.3.0/docs/_indicators/Dpo.md`

 * *Files 4% similar despite different names*

```diff
@@ -52,15 +52,15 @@
 
 ## Example
 
 ```python
 from stock_indicators import indicators
 
 # This method is NOT a part of the library.
-quotes = get_history_from_feed("SPY")
+quotes = get_historical_quotes("SPY")
 
 # Calculate
 results = indicators.get_dpo(quotes, 14)
 ```
 
 ## About {{ page.title }}
```

### Comparing `stock-indicators-1.2.1/docs/_indicators/ElderRay.md` & `stock_indicators-1.3.0/docs/_indicators/ElderRay.md`

 * *Files 1% similar despite different names*

```diff
@@ -56,15 +56,15 @@
 
 ## Example
 
 ```python
 from stock_indicators import indicators
 
 # This method is NOT a part of the library.
-quotes = get_history_from_feed("SPY")
+quotes = get_historical_quotes("SPY")
 
 # calculate ElderRay(13)
 results = indicators.get_elder_ray(quotes, 13)
 ```
 
 ## About {{ page.title }}
```

### Comparing `stock-indicators-1.2.1/docs/_indicators/Ema.md` & `stock_indicators-1.3.0/docs/_indicators/Ema.md`

 * *Files 2% similar despite different names*

```diff
@@ -57,15 +57,15 @@
 ## Example
 
 ```python
 from stock_indicators import indicators
 from stock_indicators import CandlePart     # Short path, version >= 0.8.1
 
 # This method is NOT a part of the library.
-quotes = get_history_from_feed("SPY")
+quotes = get_historical_quotes("SPY")
 
 # calculate 20-period EMA
 results = indicators.get_ema(quotes, 20, CandlePart.CLOSE)
 ```
 
 ### About {{ page.title }}
```

### Comparing `stock-indicators-1.2.1/docs/_indicators/Epma.md` & `stock_indicators-1.3.0/docs/_indicators/Epma.md`

 * *Files 2% similar despite different names*

```diff
@@ -52,15 +52,15 @@
 
 ## Example
 
 ```python
 from stock_indicators import indicators
 
 # This method is NOT a part of the library.
-quotes = get_history_from_feed("SPY")
+quotes = get_historical_quotes("SPY")
 
 # Calculate 20-period EPMA
 results = indicators.get_epma(quotes, 20)
 ```
 
 ## About {{ page.title }}
```

### Comparing `stock-indicators-1.2.1/docs/_indicators/Fcb.md` & `stock_indicators-1.3.0/docs/_indicators/Fcb.md`

 * *Files 2% similar despite different names*

```diff
@@ -54,15 +54,15 @@
 
 ## Example
 
 ```python
 from stock_indicators import indicators
 
 # This method is NOT a part of the library.
-quotes = get_history_from_feed("SPY")
+quotes = get_historical_quotes("SPY")
 
 # Calculate Fcb(14)
 results = indicators.get_fcb(quotes, 14)
 ```
 
 ## About {{ page.title }}
```

### Comparing `stock-indicators-1.2.1/docs/_indicators/FisherTransform.md` & `stock_indicators-1.3.0/docs/_indicators/FisherTransform.md`

 * *Files 4% similar despite different names*

```diff
@@ -59,15 +59,15 @@
 
 ## Example
 
 ```python
 from stock_indicators import indicators
 
 # This method is NOT a part of the library.
-quotes = get_history_from_feed("SPY")
+quotes = get_historical_quotes("SPY")
 
 # Calculate 10-period FisherTransform
 results = indicators.get_fisher_transform(quotes, 10)
 ```
 
 ## About {{ page.title }}
```

### Comparing `stock-indicators-1.2.1/docs/_indicators/ForceIndex.md` & `stock_indicators-1.3.0/docs/_indicators/ForceIndex.md`

 * *Files 2% similar despite different names*

```diff
@@ -53,15 +53,15 @@
 
 ## Example
 
 ```python
 from stock_indicators import indicators
 
 # This method is NOT a part of the library.
-quotes = get_history_from_feed("SPY")
+quotes = get_historical_quotes("SPY")
 
 # Calculate ForceIndex(13)
 results = indicators.get_force_index(quotes, 13)
 ```
 
 ## About {{ page.title }}
```

### Comparing `stock-indicators-1.2.1/docs/_indicators/Fractal.md` & `stock_indicators-1.3.0/docs/_indicators/Fractal.md`

 * *Files 2% similar despite different names*

```diff
@@ -71,15 +71,15 @@
 
 ## Example
 
 ```python
 from stock_indicators import indicators
 
 # This method is NOT a part of the library.
-quotes = get_history_from_feed("SPY")
+quotes = get_historical_quotes("SPY")
 
 # calculate Fractal
 results = indicators.get_fractal(quotes, 5)
 ```
 
 ## About {{ page.title }}
```

### Comparing `stock-indicators-1.2.1/docs/_indicators/Gator.md` & `stock_indicators-1.3.0/docs/_indicators/Gator.md`

 * *Files 1% similar despite different names*

```diff
@@ -57,15 +57,15 @@
 
 ## Example
 
 ```python
 from stock_indicators import indicators
 
 # This method is NOT a part of the library.
-quotes = get_history_from_feed("SPY")
+quotes = get_historical_quotes("SPY")
 
 # Calculate the Gator Oscillator
 results = indicators.get_gator(quotes)
 ```
 
 ## About {{ page.title }}
```

### Comparing `stock-indicators-1.2.1/docs/_indicators/HeikinAshi.md` & `stock_indicators-1.3.0/docs/_indicators/HeikinAshi.md`

 * *Files 5% similar despite different names*

```diff
@@ -53,15 +53,15 @@
 
 ## Example
 
 ```python
 from stock_indicators import indicators
 
 # This method is NOT a part of the library.
-quotes = get_history_from_feed("SPY")
+quotes = get_historical_quotes("SPY")
 
 # calculate
 results = indicators.get_heikin_ashi(quotes)
 ```
 
 ## About {{ page.title }}
```

### Comparing `stock-indicators-1.2.1/docs/_indicators/Hma.md` & `stock_indicators-1.3.0/docs/_indicators/Hma.md`

 * *Files 4% similar despite different names*

```diff
@@ -51,15 +51,15 @@
 
 ## Example
 
 ```python
 from stock_indicators import indicators
 
 # This method is NOT a part of the library.
-quotes = get_history_from_feed("SPY")
+quotes = get_historical_quotes("SPY")
 
 # Calculate 20-period HMA
 results = indicators.get_hma(quotes, 20)
 ```
 
 ## About {{ page.title }}
```

### Comparing `stock-indicators-1.2.1/docs/_indicators/HtTrendline.md` & `stock_indicators-1.3.0/docs/_indicators/HtTrendline.md`

 * *Files 8% similar despite different names*

```diff
@@ -55,15 +55,15 @@
 
 ## Example
 
 ```python
 from stock_indicators import indicators
 
 # This method is NOT a part of the library.
-quotes = get_history_from_feed("SPY")
+quotes = get_historical_quotes("SPY")
 
 # Calculate HT Trendline
 results = indicators.get_ht_trendline(quotes)
 ```
 
 ## About {{ page.title }}
```

### Comparing `stock-indicators-1.2.1/docs/_indicators/Hurst.md` & `stock_indicators-1.3.0/docs/_indicators/Hurst.md`

 * *Files 2% similar despite different names*

```diff
@@ -53,15 +53,15 @@
 
 ## Example
 
 ```python
 from stock_indicators import indicators
 
 # This method is NOT a part of the library.
-quotes = get_history_from_feed("SPY")
+quotes = get_historical_quotes("SPY")
 
 # Calculate 20-period Hurst
 results = indicators.get_hurst(quotes, 20)
 ```
 
 ## About {{ page.title }}
```

### Comparing `stock-indicators-1.2.1/docs/_indicators/Ichimoku.md` & `stock_indicators-1.3.0/docs/_indicators/Ichimoku.md`

 * *Files 2% similar despite different names*

```diff
@@ -69,15 +69,15 @@
 
 ## Example
 
 ```python
 from stock_indicators import indicators
 
 # This method is NOT a part of the library.
-quotes = get_history_from_feed("SPY")
+quotes = get_historical_quotes("SPY")
 
 # calculate ICHIMOKU(9,26,52)
 results = indicators.get_ichimoku(quotes, 9, 26, 52)
 ```
 
 ## About {{ page.title }}
```

### Comparing `stock-indicators-1.2.1/docs/_indicators/Kama.md` & `stock_indicators-1.3.0/docs/_indicators/Kama.md`

 * *Files 2% similar despite different names*

```diff
@@ -58,15 +58,15 @@
 
 ## Example
 
 ```python
 from stock_indicators import indicators
 
 # This method is NOT a part of the library.
-quotes = get_history_from_feed("SPY")
+quotes = get_historical_quotes("SPY")
 
 # Calculate KAMA(10,2,30)
 results = indicators.get_kama(quotes, 10,2,30)
 ```
 
 ## About {{ page.title }}
```

### Comparing `stock-indicators-1.2.1/docs/_indicators/Keltner.md` & `stock_indicators-1.3.0/docs/_indicators/Keltner.md`

 * *Files 2% similar despite different names*

```diff
@@ -58,15 +58,15 @@
 
 ## Example
 
 ```python
 from stock_indicators import indicators
 
 # This method is NOT a part of the library.
-quotes = get_history_from_feed("SPY")
+quotes = get_historical_quotes("SPY")
 
 # Calculate Keltner(20)
 results = indicators.get_keltner(quotes, 20,2.0,10)
 ```
 
 ## About {{ page.title }}
```

### Comparing `stock-indicators-1.2.1/docs/_indicators/Kvo.md` & `stock_indicators-1.3.0/docs/_indicators/Kvo.md`

 * *Files 2% similar despite different names*

```diff
@@ -56,15 +56,15 @@
 
 ## Example
 
 ```python
 from stock_indicators import indicators
 
 # This method is NOT a part of the library.
-quotes = get_history_from_feed("SPY")
+quotes = get_historical_quotes("SPY")
 
 # Calculate Klinger(34,55,13)
 results = indicators.get_kvo(quotes, 34, 55, 13)
 ```
 
 ## About {{ page.title }}
```

### Comparing `stock-indicators-1.2.1/docs/_indicators/MaEnvelopes.md` & `stock_indicators-1.3.0/docs/_indicators/MaEnvelopes.md`

 * *Files 3% similar despite different names*

```diff
@@ -79,15 +79,15 @@
 ## Example
 
 ```python
 from stock_indicators import indicators
 from stock_indicators import MAType     # Short path, version >= 0.8.1
 
 # This method is NOT a part of the library.
-quotes = get_history_from_feed("SPY")
+quotes = get_historical_quotes("SPY")
 
 # Calculate 20-period SMA envelopes with 2.5% offset
 results = indicators.get_ma_envelopes(quotes, 20, 2.5, MAType.SMA);
 ```
 
 ## About {{ page.title }}
```

### Comparing `stock-indicators-1.2.1/docs/_indicators/Macd.md` & `stock_indicators-1.3.0/docs/_indicators/Macd.md`

 * *Files 2% similar despite different names*

```diff
@@ -62,15 +62,15 @@
 
 ## Example
 
 ```python
 from stock_indicators import indicators
 
 # This method is NOT a part of the library.
-quotes = get_history_from_feed("SPY")
+quotes = get_historical_quotes("SPY")
 
 # calculate MACD(12,26,9)
 results = indicators.get_macd(quotes, 12, 26, 9)
 ```
 
 ## About {{ page.title }}
```

### Comparing `stock-indicators-1.2.1/docs/_indicators/Mama.md` & `stock_indicators-1.3.0/docs/_indicators/Mama.md`

 * *Files 3% similar despite different names*

```diff
@@ -55,15 +55,15 @@
 
 ## Example
 
 ```python
 from stock_indicators import indicators
 
 # This method is NOT a part of the library.
-quotes = get_history_from_feed("SPY")
+quotes = get_historical_quotes("SPY")
 
 # Calculate Mama(0.5,0.05)
 results = indicators.get_mama(quotes, 0.5,0.05)
 ```
 
 ## About {{ page.title }}
```

### Comparing `stock-indicators-1.2.1/docs/_indicators/Marubozu.md` & `stock_indicators-1.3.0/docs/_indicators/Marubozu.md`

 * *Files 3% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 
 ## Example
 
 ```python
 from stock_indicators import indicators
 
 # This method is NOT a part of the library.
-quotes = get_history_from_feed("SPY")
+quotes = get_historical_quotes("SPY")
 
 # Calculate
 results = indicators.get_marubozu(quotes);
 ```
 
 ## About {{ page.title }}
```

### Comparing `stock-indicators-1.2.1/docs/_indicators/Mfi.md` & `stock_indicators-1.3.0/docs/_indicators/Mfi.md`

 * *Files 2% similar despite different names*

```diff
@@ -51,15 +51,15 @@
 
 ## Example
 
 ```python
 from stock_indicators import indicators
 
 # This method is NOT a part of the library.
-quotes = get_history_from_feed("SPY")
+quotes = get_historical_quotes("SPY")
 
 # Calculate
 results = indicators.get_mfi(quotes, 14)
 ```
 
 ## About {{ page.title }}
```

### Comparing `stock-indicators-1.2.1/docs/_indicators/Obv.md` & `stock_indicators-1.3.0/docs/_indicators/Obv.md`

 * *Files 2% similar despite different names*

```diff
@@ -54,15 +54,15 @@
 
 ## Example
 
 ```python
 from stock_indicators import indicators
 
 # This method is NOT a part of the library.
-quotes = get_history_from_feed("SPY")
+quotes = get_historical_quotes("SPY")
 
 # Calculate
 results = indicators.get_obv(quotes)
 ```
 
 ## About {{ page.title }}
```

### Comparing `stock-indicators-1.2.1/docs/_indicators/ParabolicSar.md` & `stock_indicators-1.3.0/docs/_indicators/ParabolicSar.md`

 * *Files 1% similar despite different names*

```diff
@@ -58,15 +58,15 @@
 
 ## Example
 
 ```python
 from stock_indicators import indicators
 
 # This method is NOT a part of the library.
-quotes = get_history_from_feed("SPY")
+quotes = get_historical_quotes("SPY")
 
 # calculate ParabolicSar(0.02,0.2)
 results = indicators.get_parabolic_sar(quotes, 0.02, 0.2)
 ```
 
 ## About {{ page.title }}
```

### Comparing `stock-indicators-1.2.1/docs/_indicators/PivotPoints.md` & `stock_indicators-1.3.0/docs/_indicators/PivotPoints.md`

 * *Files 1% similar despite different names*

```diff
@@ -90,15 +90,15 @@
 ## Example
 
 ```python
 from stock_indicators import indicators
 from stock_indicators import PeriodSize, PivotPointType      # Short path, version >= 0.8.1
 
 # This method is NOT a part of the library.
-quotes = get_history_from_feed("SPY")
+quotes = get_historical_quotes("SPY")
 
 # Calculate Woodie-style month-based Pivot Points
 results = indicators.get_pivot_points(quotes, PeriodSize.MONTH, PivotPointType.WOODIE);
 ```
 
 ## About {{ page.title }}
```

### Comparing `stock-indicators-1.2.1/docs/_indicators/Pivots.md` & `stock_indicators-1.3.0/docs/_indicators/Pivots.md`

 * *Files 2% similar despite different names*

```diff
@@ -87,15 +87,15 @@
 ## Example
 
 ```python
 from stock_indicators import indicators
 from stock_indicators import EndType     # Short path, version >= 0.8.1
 
 # This method is NOT a part of the library.
-quotes = get_history_from_feed("SPY")
+quotes = get_historical_quotes("SPY")
 
 # Calculate Pivots(2,2,20) using High/Low values
 results = indicators.get_pivots(quotes, 2, 2, 20, EndType.HIGH_LOW);
 ```
 
 ## About {{ page.title }}
```

### Comparing `stock-indicators-1.2.1/docs/_indicators/Pmo.md` & `stock_indicators-1.3.0/docs/_indicators/Pmo.md`

 * *Files 2% similar despite different names*

```diff
@@ -54,15 +54,15 @@
 
 ## Example
 
 ```python
 from stock_indicators import indicators
 
 # This method is NOT a part of the library.
-quotes = get_history_from_feed("SPY")
+quotes = get_historical_quotes("SPY")
 
 # Calculate 20-period PMO
 results = indicators.get_pmo(quotes, 35,20,10)
 ```
 
 ## About {{ page.title }}
```

### Comparing `stock-indicators-1.2.1/docs/_indicators/Prs.md` & `stock_indicators-1.3.0/docs/_indicators/Prs.md`

 * *Files 3% similar despite different names*

```diff
@@ -54,16 +54,16 @@
 
 ## Example
 
 ```python
 from stock_indicators import indicators
 
 # This method is NOT a part of the library.
-history_SPX = get_history_from_feed("SPX")
-history_TSLA = get_history_from_feed("TSLA")
+history_SPX = get_historical_quotes("SPX")
+history_TSLA = get_historical_quotes("TSLA")
 
 # Calculate 14-period PRS
 results = indicators.get_prs(history_SPX, history_TSLA, 14)
 ```
 
 ## About {{ page.title }}
```

### Comparing `stock-indicators-1.2.1/docs/_indicators/Pvo.md` & `stock_indicators-1.3.0/docs/_indicators/Pvo.md`

 * *Files 2% similar despite different names*

```diff
@@ -57,15 +57,15 @@
 
 ## Example
 
 ```python
 from stock_indicators import indicators
 
 # This method is NOT a part of the library.
-quotes = get_history_from_feed("SPY")
+quotes = get_historical_quotes("SPY")
 
 # Calculate Pvo(12,26,9)
 results = indicators.get_pvo(quotes, 12, 26, 9);
 ```
 
 ## About {{ page.title }}
```

### Comparing `stock-indicators-1.2.1/docs/_indicators/Renko.md` & `stock_indicators-1.3.0/docs/_indicators/Renko.md`

 * *Files 2% similar despite different names*

```diff
@@ -73,15 +73,15 @@
 ## Example
 
 ```python
 from stock_indicators import indicators
 from stock_indicators import EndType     # Short path, version >= 0.8.1
 
 # This method is NOT a part of the library.
-quotes = get_history_from_feed("SPY")
+quotes = get_historical_quotes("SPY")
 
 # Calculate
 results = indicators.get_renko(quotes, 2.5, EndType.CLOSE);
 ```
 
 ## ATR Variant
 
@@ -115,15 +115,15 @@
 
 ## Example for ATR variant
 
 ```python
 from stock_indicators import indicators
 
 # This method is NOT a part of the library.
-quotes = get_history_from_feed("SPY")
+quotes = get_historical_quotes("SPY")
 
 # Calculate
 results = indicators.get_renko_atr(quotes, atr_periods);
 ```
 
 ## About {{ page.title }}
```

### Comparing `stock-indicators-1.2.1/docs/_indicators/Roc.md` & `stock_indicators-1.3.0/docs/_indicators/Roc.md`

 * *Files 2% similar despite different names*

```diff
@@ -55,15 +55,15 @@
 
 ## Example
 
 ```python
 from stock_indicators import indicators
 
 # This method is NOT a part of the library.
-quotes = get_history_from_feed("SPY")
+quotes = get_historical_quotes("SPY")
 
 # calculate 20-period ROC
 results = indicators.get_roc(quotes, 20)
 ```
 
 # ROC with Bands
```

### Comparing `stock-indicators-1.2.1/docs/_indicators/RollingPivots.md` & `stock_indicators-1.3.0/docs/_indicators/RollingPivots.md`

 * *Files 1% similar despite different names*

```diff
@@ -76,15 +76,15 @@
 ## Example
 
 ```python
 from stock_indicators import indicators
 from stock_indicators import PivotPointType     # Short path, version >= 0.8.1
 
 # This method is NOT a part of the library.
-quotes = get_history_from_feed("SPY")
+quotes = get_historical_quotes("SPY")
 
 # Calculate Woodie-style 14 period Rolling Pivot Points
 results = indicators.get_rolling_pivots(quotes, 14, 0, PivotPointType.Woodie);
 ```
 
 ## About {{ page.title }}
```

### Comparing `stock-indicators-1.2.1/docs/_indicators/Rsi.md` & `stock_indicators-1.3.0/docs/_indicators/Rsi.md`

 * *Files 6% similar despite different names*

```diff
@@ -54,15 +54,15 @@
 
 ## Example
 
 ```python
 from stock_indicators import indicators
 
 # This method is NOT a part of the library.
-quotes = get_history_from_feed("SPY")
+quotes = get_historical_quotes("SPY")
 
 # calculate RSI(14)
 results = indicators.get_rsi(quotes, 14)
 ```
 
 ## About {{ page.title }}
```

### Comparing `stock-indicators-1.2.1/docs/_indicators/Slope.md` & `stock_indicators-1.3.0/docs/_indicators/Slope.md`

 * *Files 2% similar despite different names*

```diff
@@ -57,15 +57,15 @@
 
 ## Example
 
 ```python
 from stock_indicators import indicators
 
 # This method is NOT a part of the library.
-quotes = get_history_from_feed("SPY")
+quotes = get_historical_quotes("SPY")
 
 # calculate 20-period Slope
 results = indicators.get_slope(quotes, 20)
 ```
 
 ## About {{ page.title }}
```

### Comparing `stock-indicators-1.2.1/docs/_indicators/Sma.md` & `stock_indicators-1.3.0/docs/_indicators/Sma.md`

 * *Files 2% similar despite different names*

```diff
@@ -55,15 +55,15 @@
 ## Example
 
 ```python
 from stock_indicators import indicators
 from stock_indicators import CandlePart     # Short path, version >= 0.8.1
 
 # This method is NOT a part of the library.
-quotes = get_history_from_feed("SPY")
+quotes = get_historical_quotes("SPY")
 
 # calculate 20-period SMA
 results = indicators.get_sma(quotes, 20, CandlePart.CLOSE)
 ```
 
 <hr>
 # Extended analysis
```

### Comparing `stock-indicators-1.2.1/docs/_indicators/Smi.md` & `stock_indicators-1.3.0/docs/_indicators/Smi.md`

 * *Files 8% similar despite different names*

```diff
@@ -57,15 +57,15 @@
 
 ## Example
 
 ```python
 from stock_indicators import indicators
 
 # This method is NOT a part of the library.
-quotes = get_history_from_feed("SPY")
+quotes = get_historical_quotes("SPY")
 
 # Calculate SMI(14,20,5,3)
 results = indicators.get_smi(quotes, 14, 20, 5, 3)
 ```
 
 ## About {{ page.title }}
```

### Comparing `stock-indicators-1.2.1/docs/_indicators/Smma.md` & `stock_indicators-1.3.0/docs/_indicators/Smma.md`

 * *Files 8% similar despite different names*

```diff
@@ -54,15 +54,15 @@
 
 ## Example
 
 ```python
 from stock_indicators import indicators
 
 # This method is NOT a part of the library.
-quotes = get_history_from_feed("SPY")
+quotes = get_historical_quotes("SPY")
 
 # Calculate 20-period SMMA
 results = indicators.get_smma(quotes, 20)
 ```
 
 ## About {{ page.title }}
```

### Comparing `stock-indicators-1.2.1/docs/_indicators/StarcBands.md` & `stock_indicators-1.3.0/docs/_indicators/StarcBands.md`

 * *Files 5% similar despite different names*

```diff
@@ -57,15 +57,15 @@
 
 ## Example
 
 ```python
 from stock_indicators import indicators
 
 # This method is NOT a part of the library.
-quotes = get_history_from_feed("SPY")
+quotes = get_historical_quotes("SPY")
 
 # Calculate StarcBands(20)
 results = indicators.get_starc_bands(quotes, 20, 2.0, 10)
 ```
 
 ## About {{ page.title }}
```

### Comparing `stock-indicators-1.2.1/docs/_indicators/Stc.md` & `stock_indicators-1.3.0/docs/_indicators/Stc.md`

 * *Files 4% similar despite different names*

```diff
@@ -55,15 +55,15 @@
 
 ## Example
 
 ```python
 from stock_indicators import indicators
 
 # This method is NOT a part of the library.
-quotes = get_history_from_feed("SPY")
+quotes = get_historical_quotes("SPY")
 
 # Calculate STC(12,26,9)
 results = indicators.get_stc(quotes, 10, 23, 50)
 ```
 
 ## About {{ page.title }}
```

### Comparing `stock-indicators-1.2.1/docs/_indicators/StdDev.md` & `stock_indicators-1.3.0/docs/_indicators/StdDev.md`

 * *Files 1% similar despite different names*

```diff
@@ -56,15 +56,15 @@
 
 ## Example
 
 ```python
 from stock_indicators import indicators
 
 # This method is NOT a part of the library.
-quotes = get_history_from_feed("SPY")
+quotes = get_historical_quotes("SPY")
 
 # Calculate 10-period Standard Deviation
 results = indicators.get_stdev(quotes, 10)
 ```
 
 ## About {{ page.title }}
```

### Comparing `stock-indicators-1.2.1/docs/_indicators/StdDevChannels.md` & `stock_indicators-1.3.0/docs/_indicators/StdDevChannels.md`

 * *Files 2% similar despite different names*

```diff
@@ -57,15 +57,15 @@
 
 ## Example
 
 ```python
 from stock_indicators import indicators
 
 # This method is NOT a part of the library.
-quotes = get_history_from_feed("SPY")
+quotes = get_historical_quotes("SPY")
 
 # calculate StdDevChannels(20,2)
 results = indicators.get_stdev_channels(quotes, 20,2)
 ```
 
 ## Alternative depiction for full quotes variant
```

### Comparing `stock-indicators-1.2.1/docs/_indicators/Stoch.md` & `stock_indicators-1.3.0/docs/_indicators/Stoch.md`

 * *Files 2% similar despite different names*

```diff
@@ -73,15 +73,15 @@
 
 ## Example
 
 ```python
 from stock_indicators import indicators
 
 # This method is NOT a part of the library.
-quotes = get_history_from_feed("SPY")
+quotes = get_historical_quotes("SPY")
 
 # calculate STO %K(14),%D(3) (slow)
 results = indicators.get_stoch(quotes, 14, 3, 3)
 ```
 
 ## About {{ page.title }}
```

### Comparing `stock-indicators-1.2.1/docs/_indicators/StochRsi.md` & `stock_indicators-1.3.0/docs/_indicators/StochRsi.md`

 * *Files 4% similar despite different names*

```diff
@@ -59,15 +59,15 @@
 
 ## Example
 
 ```python
 from stock_indicators import indicators
 
 # This method is NOT a part of the library.
-quotes = get_history_from_feed("SPY")
+quotes = get_historical_quotes("SPY")
 
 # calculate StochRSI
 results = indicators.get_stoch_rsi(quotes, 14, 14, 1, 1)
 ```
 
 ## About {{ page.title }}
```

### Comparing `stock-indicators-1.2.1/docs/_indicators/SuperTrend.md` & `stock_indicators-1.3.0/docs/_indicators/SuperTrend.md`

 * *Files 1% similar despite different names*

```diff
@@ -58,15 +58,15 @@
 
 ## Example
 
 ```python
 from stock_indicators import indicators
 
 # This method is NOT a part of the library.
-quotes = get_history_from_feed("SPY")
+quotes = get_historical_quotes("SPY")
 
 # calculate SuperTrend(14,3)
 results = indicators.get_super_trend(quotes, 14, 3)
 ```
 
 ## About {{ page.title }}
```

### Comparing `stock-indicators-1.2.1/docs/_indicators/T3.md` & `stock_indicators-1.3.0/docs/_indicators/T3.md`

 * *Files 8% similar despite different names*

```diff
@@ -54,15 +54,15 @@
 
 ## Example
 
 ```python
 from stock_indicators import indicators
 
 # This method is NOT a part of the library.
-quotes = get_history_from_feed("SPY")
+quotes = get_historical_quotes("SPY")
 
 # Calculate 5-period T3
 results = indicators.get_t3(quotes, 5, 0.7)
 ```
 
 ## About {{ page.title }}
```

### Comparing `stock-indicators-1.2.1/docs/_indicators/Tema.md` & `stock_indicators-1.3.0/docs/_indicators/Tema.md`

 * *Files 1% similar despite different names*

```diff
@@ -53,15 +53,15 @@
 
 ## Example
 
 ```python
 from stock_indicators import indicators
 
 # This method is NOT a part of the library.
-quotes = get_history_from_feed("SPY")
+quotes = get_historical_quotes("SPY")
 
 # calculate 20-period TEMA
 results = indicators.get_tema(quotes, 20)
 ```
 
 ## About {{ page.title }}
```

### Comparing `stock-indicators-1.2.1/docs/_indicators/Trix.md` & `stock_indicators-1.3.0/docs/_indicators/Trix.md`

 * *Files 1% similar despite different names*

```diff
@@ -56,15 +56,15 @@
 
 ## Example
 
 ```python
 from stock_indicators import indicators
 
 # This method is NOT a part of the library.
-quotes = get_history_from_feed("SPY")
+quotes = get_historical_quotes("SPY")
 
 # calculate 20-period Trix
 results = indicators.get_trix(quotes, 14)
 ```
 
 ## About {{ page.title }}
```

### Comparing `stock-indicators-1.2.1/docs/_indicators/Tsi.md` & `stock_indicators-1.3.0/docs/_indicators/Tsi.md`

 * *Files 2% similar despite different names*

```diff
@@ -57,15 +57,15 @@
 
 ## Example
 
 ```python
 from stock_indicators import indicators
 
 # This method is NOT a part of the library.
-quotes = get_history_from_feed("SPY")
+quotes = get_historical_quotes("SPY")
 
 # Calculate 20-period TSI
 results = indicators.get_tsi(quotes, 25, 13, 7)
 ```
 
 ## About {{ page.title }}
```

### Comparing `stock-indicators-1.2.1/docs/_indicators/UlcerIndex.md` & `stock_indicators-1.3.0/docs/_indicators/UlcerIndex.md`

 * *Files 4% similar despite different names*

```diff
@@ -51,15 +51,15 @@
 
 ## Example
 
 ```python
 from stock_indicators import indicators
 
 # This method is NOT a part of the library.
-quotes = get_history_from_feed("SPY")
+quotes = get_historical_quotes("SPY")
 
 # Calculate UI(14)
 results = indicators.get_ulcer_index(quotes, 14)
 ```
 
 ## About {{ page.title }}
```

### Comparing `stock-indicators-1.2.1/docs/_indicators/Ultimate.md` & `stock_indicators-1.3.0/docs/_indicators/Ultimate.md`

 * *Files 1% similar despite different names*

```diff
@@ -53,15 +53,15 @@
 
 ## Example
 
 ```python
 from stock_indicators import indicators
 
 # This method is NOT a part of the library.
-quotes = get_history_from_feed("SPY")
+quotes = get_historical_quotes("SPY")
 
 # calculate 20-period Ultimate
 results = indicators.get_ultimate(quotes, 7, 14, 28)
 ```
 
 ## About {{ page.title }}
```

### Comparing `stock-indicators-1.2.1/docs/_indicators/VolatilityStop.md` & `stock_indicators-1.3.0/docs/_indicators/VolatilityStop.md`

 * *Files 1% similar despite different names*

```diff
@@ -59,15 +59,15 @@
 
 ## Example
 
 ```python
 from stock_indicators import indicators
 
 # This method is NOT a part of the library.
-quotes = get_history_from_feed("SPY")
+quotes = get_historical_quotes("SPY")
 
 # Calculate VolatilityStop(20,2.5)
 results = indicators.get_volatility_stop(quotes, 20, 2.5)
 ```
 
 ## About {{ page.title }}
```

### Comparing `stock-indicators-1.2.1/docs/_indicators/Vortex.md` & `stock_indicators-1.3.0/docs/_indicators/Vortex.md`

 * *Files 2% similar despite different names*

```diff
@@ -52,15 +52,15 @@
 
 ## Example
 
 ```python
 from stock_indicators import indicators
 
 # This method is NOT a part of the library.
-quotes = get_history_from_feed("SPY")
+quotes = get_historical_quotes("SPY")
 
 # Calculate 14-period VI
 results = indicators.get_vortex(quotes, 14);
 ```
 
 ## About {{ page.title }}
```

### Comparing `stock-indicators-1.2.1/docs/_indicators/Vwap.md` & `stock_indicators-1.3.0/docs/_indicators/Vwap.md`

 * *Files 1% similar despite different names*

```diff
@@ -55,15 +55,15 @@
 
 ## Example
 
 ```python
 from stock_indicators import indicators
 
 # This method is NOT a part of the library.
-quotes = get_history_from_feed("SPY")
+quotes = get_historical_quotes("SPY")
 
 # Calculate
 results = indicators.get_vwap(quotes);
 ```
 
 ## About {{ page.title }}
```

### Comparing `stock-indicators-1.2.1/docs/_indicators/Vwma.md` & `stock_indicators-1.3.0/docs/_indicators/Vwma.md`

 * *Files 2% similar despite different names*

```diff
@@ -51,15 +51,15 @@
 
 ## Example
 
 ```python
 from stock_indicators import indicators
 
 # This method is NOT a part of the library.
-quotes = get_history_from_feed("SPY")
+quotes = get_historical_quotes("SPY")
 
 # Calculate 10-period VWMA
 results = indicators.get_vwma(quotes, 10)
 ```
 
 ## About {{ page.title }}
```

### Comparing `stock-indicators-1.2.1/docs/_indicators/WilliamsR.md` & `stock_indicators-1.3.0/docs/_indicators/WilliamsR.md`

 * *Files 6% similar despite different names*

```diff
@@ -51,15 +51,15 @@
 
 ## Example
 
 ```python
 from stock_indicators import indicators
 
 # This method is NOT a part of the library.
-quotes = get_history_from_feed("SPY")
+quotes = get_historical_quotes("SPY")
 
 # Calculate WilliamsR(14)
 results = indicators.get_williams_r(quotes, 14)
 ```
 
 ## About {{ page.title }}
```

### Comparing `stock-indicators-1.2.1/docs/_indicators/Wma.md` & `stock_indicators-1.3.0/docs/_indicators/Wma.md`

 * *Files 2% similar despite different names*

```diff
@@ -55,15 +55,15 @@
 ## Example
 
 ```python
 from stock_indicators import indicators
 from stock_indicators import CandlePart     # Short path, version >= 0.8.1
 
 # This method is NOT a part of the library.
-quotes = get_history_from_feed("SPY")
+quotes = get_historical_quotes("SPY")
 
 # Calculate 20-period WMA
 results = indicators.get_wma(quotes, 20, CandlePart.CLOSE)
 ```
 
 ## About {{ page.title }}
```

### Comparing `stock-indicators-1.2.1/docs/_indicators/ZigZag.md` & `stock_indicators-1.3.0/docs/_indicators/ZigZag.md`

 * *Files 2% similar despite different names*

```diff
@@ -72,15 +72,15 @@
 ## Example
 
 ```python
 from stock_indicators import indicators
 from stock_indicators import EndType     # Short path, version >= 0.8.1
 
 # This method is NOT a part of the library.
-quotes = get_history_from_feed("SPY")
+quotes = get_historical_quotes("SPY")
 
 # Calculate 3% change ZIGZAG
 results = indicators.get_zig_zag(quotes, EndType.CLOSE, 3);
 ```
 
 ## About {{ page.title }}
```

### Comparing `stock-indicators-1.2.1/docs/assets/css/normalize.css` & `stock_indicators-1.3.0/docs/assets/css/normalize.css`

 * *Files identical despite different names*

### Comparing `stock-indicators-1.2.1/docs/assets/css/rouge-github.css` & `stock_indicators-1.3.0/docs/assets/css/rouge-github.css`

 * *Files identical despite different names*

### Comparing `stock-indicators-1.2.1/docs/assets/css/style.scss` & `stock_indicators-1.3.0/docs/assets/css/style.scss`

 * *Files identical despite different names*

### Comparing `stock-indicators-1.2.1/docs/assets/icons/android-chrome-192x192.png` & `stock_indicators-1.3.0/docs/assets/icons/android-chrome-192x192.png`

 * *Files identical despite different names*

### Comparing `stock-indicators-1.2.1/docs/assets/icons/android-chrome-512x512.png` & `stock_indicators-1.3.0/docs/assets/icons/android-chrome-512x512.png`

 * *Files identical despite different names*

### Comparing `stock-indicators-1.2.1/docs/assets/icons/apple-touch-icon.png` & `stock_indicators-1.3.0/docs/assets/icons/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `stock-indicators-1.2.1/docs/assets/icons/favicon-16x16.png` & `stock_indicators-1.3.0/docs/assets/icons/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `stock-indicators-1.2.1/docs/assets/icons/favicon-32x32.png` & `stock_indicators-1.3.0/docs/assets/icons/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `stock-indicators-1.2.1/docs/assets/icons/maskable_icon_x192.png` & `stock_indicators-1.3.0/docs/assets/icons/maskable_icon_x192.png`

 * *Files identical despite different names*

### Comparing `stock-indicators-1.2.1/docs/assets/icons/maskable_icon_x512.png` & `stock_indicators-1.3.0/docs/assets/icons/maskable_icon_x512.png`

 * *Files identical despite different names*

### Comparing `stock-indicators-1.2.1/docs/assets/icons/mstile-144x144.png` & `stock_indicators-1.3.0/docs/assets/icons/mstile-144x144.png`

 * *Files identical despite different names*

### Comparing `stock-indicators-1.2.1/docs/assets/icons/mstile-150x150.png` & `stock_indicators-1.3.0/docs/assets/icons/mstile-150x150.png`

 * *Files identical despite different names*

### Comparing `stock-indicators-1.2.1/docs/assets/icons/mstile-310x150.png` & `stock_indicators-1.3.0/docs/assets/icons/mstile-310x150.png`

 * *Files identical despite different names*

### Comparing `stock-indicators-1.2.1/docs/assets/icons/mstile-310x310.png` & `stock_indicators-1.3.0/docs/assets/icons/mstile-310x310.png`

 * *Files identical despite different names*

### Comparing `stock-indicators-1.2.1/docs/assets/icons/mstile-70x70.png` & `stock_indicators-1.3.0/docs/assets/icons/mstile-70x70.png`

 * *Files identical despite different names*

### Comparing `stock-indicators-1.2.1/docs/assets/icons/safari-pinned-tab.svg` & `stock_indicators-1.3.0/docs/assets/icons/safari-pinned-tab.svg`

 * *Files identical despite different names*

### Comparing `stock-indicators-1.2.1/docs/assets/js/lazysizes.min.js` & `stock_indicators-1.3.0/docs/assets/js/lazysizes.min.js`

 * *Files identical despite different names*

### Comparing `stock-indicators-1.2.1/docs/assets/manifest.json` & `stock_indicators-1.3.0/docs/assets/manifest.json`

 * *Files identical despite different names*

### Comparing `stock-indicators-1.2.1/docs/contributing.md` & `stock_indicators-1.3.0/docs/contributing.md`

 * *Files 15% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 permalink: /contributing/
 relative_path: pages/contributing.md
 layout: page
 ---
 
 # Contributing guidelines
 
-[![Codacy quality grade](https://app.codacy.com/project/badge/Grade/2b48204b1e304e3bac977fbc92b19c14)](https://app.codacy.com/gh/DaveSkender/Stock.Indicators.Python/dashboard)
-[![Codacy code coverage](https://app.codacy.com/project/badge/Coverage/2b48204b1e304e3bac977fbc92b19c14)](https://app.codacy.com/gh/DaveSkender/Stock.Indicators.Python/dashboard)
+[![Codacy quality grade](https://app.codacy.com/project/badge/Grade/3f55a14f5dc14a0eba41f86006c1185b)](https://app.codacy.com/gh/facioquo/stock-indicators-python/dashboard)
+[![Codacy code coverage](https://app.codacy.com/project/badge/Coverage/3f55a14f5dc14a0eba41f86006c1185b)](https://app.codacy.com/gh/facioquo/stock-indicators-python/dashboard)
 
 **Thanks for taking the time to contribute!**
 
 This project is simpler than most, so it's a good place to start contributing to the open source community, even if you're a newbie.
 
 We are accepting these sorts of changes and requests:
 
@@ -30,21 +30,21 @@
 
 We have different places to take issues by its category.
 
 ### Bug Report
 
 If you are reporting a bug or suspect a problem, please submit an issue with a detailed description of the problem + include steps to reproduce, code samples, and any reference materials.  
 
-🔧 [Report bugs](https://github.com/DaveSkender/Stock.Indicators.Python/issues/new?labels=bug&template=bug_report.md)
+🔧 [Report bugs](https://github.com/facioquo/stock-indicators-python/issues/new?labels=bug&template=bug_report.md)
 
 ### Feature Request
 
 For new features, submit an issue with the `enhancement` label.
 
-💡 [Request features](https://github.com/DaveSkender/Stock.Indicators.Python/issues/new?labels=enhancement&template=feature_request.md)
+💡 [Request features](https://github.com/facioquo/stock-indicators-python/issues/new?labels=enhancement&template=feature_request.md)
 
 ## Project management
 
 - Planned work is managed in [the backlog](https://github.com/users/DaveSkender/projects/2).
 - Work items are primarily [entered as Notes](https://docs.github.com/issues/organizing-your-work-with-project-boards/tracking-work-with-project-boards/adding-notes-to-a-project-board) (not Issues), except where an issue or feature is user reported.  With that said, Notes can be converted to Issues if in-progress and collaborative discussion is needed.
 - Use the [Discussions](https://github.com/DaveSkender/Stock.Indicators/discussions) area for general ideation and unrelated questions.
 
@@ -125,25 +125,25 @@
 - [PEP 8 -- Style Guide for Python Code](https://www.python.org/dev/peps/pep-0008/)
 - [PEP 440 -- Version Identification and Dependency Specification](https://www.python.org/dev/peps/pep-0440/)
 - [Semantic Version 2.0](https://semver.org)
 - [Python Packaging User Guide](https://packaging.python.org/)
 
 ## Versioning
 
-We use the `setuptools_scm` tool for [semantic versioning](https://semver.org).  It detects the version number from `git tag` in the [GitHub Actions build](https://github.com/DaveSkender/Stock.Indicators.Python/deployments/pypi).
+We use the `setuptools_scm` tool for [semantic versioning](https://semver.org).  It detects the version number from `git tag` in the [GitHub Actions build](https://github.com/facioquo/stock-indicators-python/deployments/pypi).
 
 Type | Format | Description
 ------------ | ------ | -----------
 Major | `x.-.-` | A significant deviation with major breaking changes.
-Minor | `-.x.-` | A new feature, usually new non-breaking change, such as adding an indicator.  Minor breaking changes may occur here and are denoted in the [release notes](https://github.com/DaveSkender/Stock.Indicators.Python/releases).
+Minor | `-.x.-` | A new feature, usually new non-breaking change, such as adding an indicator.  Minor breaking changes may occur here and are denoted in the [release notes](https://github.com/facioquo/stock-indicators-python/releases).
 Patch | `-.-.x` | A small bug fix, chore, or documentation change.
 
 After one of our repository administrators creates a `git tag` on the `main` branch,
 reflecting the new version number, the `PyPI` deployment workflow will start.
-After the new package is published, they'll publicly post the [release record](https://github.com/DaveSkender/Stock.Indicators.Python/releases) with [automatically generated notes](https://docs.github.com/en/repositories/releasing-projects-on-github/automatically-generated-release-notes) and other information.
+After the new package is published, they'll publicly post the [release record](https://github.com/facioquo/stock-indicators-python/releases) with [automatically generated notes](https://docs.github.com/en/repositories/releasing-projects-on-github/automatically-generated-release-notes) and other information.
 
 ## License
 
 [![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 
 This repository uses a standard Apache 2.0 open-source license.  It enables open-source community development by protecting the project and contributors from certain legal risks while allowing the widest range of uses, including in closed source software.  Please review the [license](https://opensource.org/licenses/Apache-2.0) before using or contributing to the software.
```

### Comparing `stock-indicators-1.2.1/docs/favicon.ico` & `stock_indicators-1.3.0/docs/favicon.ico`

 * *Files identical despite different names*

### Comparing `stock-indicators-1.2.1/docs/pages/guide.md` & `stock_indicators-1.3.0/docs/pages/guide.md`

 * *Files 4% similar despite different names*

```diff
@@ -21,41 +21,39 @@
 
 ## Getting started
 
 ### Installation and setup
 
 1. Install prerequisite framework dependencies
 
-    Stock Indicators for Python has dependency on on the [Common Language Runtime (CLR)](https://learn.microsoft.com/dotnet/standard/clr).  You'll need to install the .NET SDK in your environment to get required CLR capability.
+    Stock Indicators for Python has dependency on on the [Common Language Runtime (CLR)](https://learn.microsoft.com/dotnet/standard/clr).  You'll need to install the .NET SDK in your environment to get required CLR capability. Check that you've installed the following prerequisite software:
 
-    Check that you've installed the following prerequisite software:
-
-    > Install the latest **Python** and **.NET SDK** for best performance.
+    > Install **Python** and the **.NET SDK**.  Use the latest versions for better performance.
 
     | Installer | Min | Latest | Download |
     |---| :---: | :---: | --- |
     | Python | 3.8 | 3.12 | [@python.org](https://www.python.org/downloads/) |
     | .NET SDK | 6.0 | 8.0 | [@microsoft.com](https://dotnet.microsoft.com/en-us/download) |
 
     Note: we do not support the open source [Mono .NET Framework](https://www.mono-project.com).
 
-2. Find and install the **stock-indicators** Python package into your environment.
+2. Install the **stock-indicators** Python package into your environment.
 
     ```bash
-    # pip example
+    # bash CLI command
     pip install stock-indicators
     ```
 
     > See [Python documentation](https://packaging.python.org/en/latest/tutorials/installing-packages/) for more help with installing packages.
 
 ### Prerequisite data
 
 Most indicators require that you provide historical quote data and additional configuration parameters.
 
-You must get historical quotes from your own market data provider.  For clarification, the `get_history_from_feed()` method shown in the example below and throughout our documentation **is not part of this library**, but rather an example to represent your own acquisition of historical quotes.
+You must get historical quotes from your own market data provider.  For clarification, the `get_historical_quotes()` method shown in the example below and throughout our documentation **is not part of this library**, but rather an example to represent your own acquisition of historical quotes.
 
 Historical price data can be provided as an `Iterable`(such as `List` or an object having `__iter__()`) of the `Quote` class or its sub-class ([see below](#historical-quotes)); be aware that you **have to** inherit `Quote` class when you [make custom quote class](#using-custom-quote-classes).
 
 For additional configuration parameters, default values are provided when there is an industry standard.  You can, of course, override these and provide your own values.
 
 ### Example usage
 
@@ -84,29 +82,32 @@
 SMA on 2018-04-25 was $255.6570
 SMA on 2018-04-26 was $255.9705
 ..
 ```
 
 See [individual indicator pages]({{site.baseurl}}/indicators/) for specific usage guidance.
 
-More examples available:
-
-- [Demo site](https://charts.stockindicators.dev) (a stock chart)
+> **More help**: if you're having trouble getting started, see our
+> **[QuickStart guide](https://github.com/facioquo/stock-indicators-python-quickstart#readme)**
+> for step-by-step instructions to setup up your environment,
+> and for calculating your first indicator using this library.
+>
+> We also have a [demo site](https://charts.stockindicators.dev) (a stock chart) where you can visualize and experiment with different indicator settings.
 
 ## Historical quotes
 
 You must provide historical price quotes to the library in the standard [OHLCV](https://acronyms.thefreedictionary.com/OHLCV) `Iterable[Quote]`(such as a list of `Quote`) format.  It should have a consistent period frequency (day, hour, minute, etc).
 
 <!-- ### stock_indicators.indicators.common.quote.**Quote** -->
 ```python
 from stock_indicators.indicators.common.quote import Quote
 ```
 
 **class Quote(date, open=None, high=None, low=None, close=None, volume=None)**
-[[source]](https://github.com/DaveSkender/Stock.Indicators.Python/blob/main/stock_indicators/indicators/common/quote.py)
+[[source]](https://github.com/facioquo/stock-indicators-python/blob/main/stock_indicators/indicators/common/quote.py)
 
 | name | type | notes |
 | -- |-- |-- |
 | date | [`datetime.datetime`](https://docs.python.org/3.8/library/datetime.html#datetime.datetime) | Date |
 | open | [`decimal.Decimal`](https://docs.python.org/3.8/library/decimal.html?highlight=decimal#decimal.Decimal), Optional | Open price |
 | high | [`decimal.Decimal`](https://docs.python.org/3.8/library/decimal.html?highlight=decimal#decimal.Decimal), Optional | High price |
 | low | [`decimal.Decimal`](https://docs.python.org/3.8/library/decimal.html?highlight=decimal#decimal.Decimal), Optional | Low price |
@@ -114,34 +115,29 @@
 | volume | [`decimal.Decimal`](https://docs.python.org/3.8/library/decimal.html?highlight=decimal#decimal.Decimal), Optional | Volume |
 
 Note that:
 
 1. `date` is always required, while each ohlcv values are optional.
 2. ohlcv can be provided by `float`, `Decimal` and `str` representing number, but these are always stored as `Decimal`.
 
-> If you're having trouble converting into `Quote` format, see our GitHub discussion on
-> [Converting Pandas DataFrame to iterable Quotes]({{site.dotnet.repo}}/discussions/1165) for more information and troubleshooting support.
-
 ### Where can I get historical quote data?
 
 There are many places to get stock market data.  Check with your brokerage or other commercial sites.  If you're looking for a free developer API, see our ongoing [discussion on market data]({{site.dotnet.repo}}/discussions/579) for ideas.
 
 ### How much historical quote data do I need?
 
-Each indicator will need different amounts of price `quotes` to calculate.  You can find guidance on the individual indicator documentation pages for minimum requirements; however, **most use cases will require that you provide more than the minimum**.  As a general rule of thumb, you will be safe if you provide 750 points of historical quote data (e.g. 3 years of daily data).  A `BadQuotesException` will be thrown if you do not provide sufficient historical quotes to produce any results.
-
->&#128681; IMPORTANT! Some indicators use a smoothing technique that converges to better precision over time.  While you can calculate these with the minimum amount of quote data, the precision to two decimal points often requires 250 or more preceding historical records.
+Each indicator will need different amounts of price `quotes` to calculate.  You can find guidance on the individual indicator documentation pages for minimum requirements; however, **most use cases will require that you provide more than the minimum**.  As a general rule of thumb, you will be safe if you provide 750 points of historical quote data (e.g. 3 years of daily data).
 
-For example, if you are using daily data and want one year of precise EMA(250) data, you need to provide 3 years of historical quotes (1 extra year for the lookback period and 1 extra year for convergence); thereafter, you would discard or not use the first two years of results.  Occassionally, even more is required for optimal precision.
+> &#128681; **IMPORTANT! Applying the _minimum_ amount of quote history as possible is NOT a good way to optimize your system.**  Some indicators use a smoothing technique that converges to better precision over time.  While you can calculate these with the minimum amount of quote data, the precision to two decimal points often requires 250 or more preceding historical records.
+>
+> For example, if you are using daily data and want one year of precise EMA(250) data, you need to provide 3 years of historical quotes (1 extra year for the lookback period and 1 extra year for convergence); thereafter, you would discard or not use the first two years of results.  Occasionally, even more is required for optimal precision.
 
-### Using Pandas.Dataframe
+### Using pandas.DataFrame
 
-If you are using `Pandas.Dataframe` to hold quote data, you have to convert it into our `Quote` instance. That means you must iterate them row by row. There's [an awesome article](https://towardsdatascience.com/efficiently-iterating-over-rows-in-a-pandas-dataframe-7dd5f9992c01) that introduces the best-efficiency way to iterate `Dataframe`.
-
-Here's an example we'd like to suggest: **use list comprehension**
+If you are using `pandas.DataFrame` to hold quote data, you have to convert it into an iterable `Quote` list. Here's [an efficient way](https://towardsdatascience.com/efficiently-iterating-over-rows-in-a-pandas-dataframe-7dd5f9992c01) to iterate `DataFrame` using _list comprehension_.
 
 ```python
 # Suppose that you have dataframe like the below.
 #             date    open    high     low   close     volume
 # 0     2018-12-31  244.92  245.54  242.87  245.28  147031456
 # 1     2018-12-28  244.94  246.73  241.87  243.15  155998912
 # 2     2018-12-27  238.06  243.68  234.52  243.46  189794032
@@ -152,34 +148,37 @@
 quotes_list = [
     Quote(d,o,h,l,c,v) 
     for d,o,h,l,c,v 
     in zip(df['date'], df['open'], df['high'], df['low'], df['close'], df['volume'])
 ]
 ```
 
-You can also use `numpy.vectorize()`, its gain is too slight and hard to apply in this case.
+> For a quickstart that uses **pandas.DataFrame**, see our online _ReplIt_ code example for the [Williams Fractal indicator](https://replit.com/@daveskender/Stock-Indicators-for-Python-Williams-Fractal).
+>
+> _For more help_, see our GitHub community discussion on
+> [Converting pandas.DataFrame to iterable Quotes]({{site.dotnet.repo}}/discussions/1165).
 
 ### Using custom quote classes
 
-If you would like to use your own custom `MyCustomQuote` _quote_ class, you **have to** inherit `Quote` class. The `Quote` class is a special class which converts OHLCV properties existing as Python objects to C# objects and which is concrete class of `IQuote` of C# implementation. It enables PythonNet to work with our C# implementation using generics.
+If you would like to use your own custom `MyCustomQuote` _quote_ class, you **have to** inherit `Quote` class. The `Quote` class is a special class which converts OHLCV properties existing as Python objects to C# objects and which is concrete class of `IQuote` of C# implementation. It enables Python.Net to work with our C# implementation using generics.
 
 ```python
 from stock_indicators.indicators.common import Quote
 
 class MyCustomQuote(Quote):
     def foo(self): ...
     ... add your own attributes.
 
 ```
 
 ```python
 from stock_indicators import indicators
 
 # fetch historical quotes from your favorite feed
-quotes: Iterable[MyCustomQuote] = get_history_from_feed("MSFT");
+quotes: Iterable[MyCustomQuote] = get_historical_quotes("MSFT");
 
 # example: get 20-period simple moving average
 results = indicators.get_sma(quotes, 20);
 ```
 
 #### Using custom quote property names
 
@@ -208,15 +207,15 @@
 from stock_indicators.indicators.ema import EMAResult
 
 class ExtendedEMA(EMAResult):
     def __str__(self):
         return f"EMA on {self.date.date()} was ${self.ema or 0:.4f}"
     
 # compute indicator
-quotes = get_history_from_feed("MSFT")
+quotes = get_historical_quotes("MSFT")
 results = indicators.get_ema(quotes, 20)
 
 # 1. list[ExtendedEMA]
 extended_results = [ ExtendedEMA(r._csdata) for r in results ]
 for r in extended_results:
     print(r)
 ```
@@ -237,15 +236,15 @@
 
 If you want to compute an indicator of indicators, such as an SMA of an ADX or an [RSI of an OBV](https://medium.com/@robswc/this-is-what-happens-when-you-combine-the-obv-and-rsi-indicators-6616d991773d), all you need to do is to take the results of one, reformat into a synthetic historical quotes, and send it through to another indicator.
 
 ```python
 from stock_indicators import indicators
 
 # fetch historical quotes from your feed (your method)
-quotes = get_history_from_feed("MSFT")
+quotes = get_historical_quotes("MSFT")
 
 # calculate EMA
 results = indicators.get_ema(quotes, 20)
 
 # convert to synthetic quotes
 quotes_from_ema = [ Quote(date=r.date, close=r.ema) for r in results ]
```

### Comparing `stock-indicators-1.2.1/docs/pages/home.md` & `stock_indicators-1.3.0/docs/pages/home.md`

 * *Files identical despite different names*

### Comparing `stock-indicators-1.2.1/docs/pages/indicators.html` & `stock_indicators-1.3.0/docs/pages/indicators.html`

 * *Files identical despite different names*

### Comparing `stock-indicators-1.2.1/docs/pages/performance.md` & `stock_indicators-1.3.0/docs/pages/performance.md`

 * *Files identical despite different names*

### Comparing `stock-indicators-1.2.1/docs/pages/utilities.md` & `stock_indicators-1.3.0/docs/pages/utilities.md`

 * *Files 2% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 
 ### Find indicator result by date
 
 `results.find(lookup_date)` is a simple lookup for your indicator results collection.  Just specify the date you want returned.
 
 ```python
 # fetch historical quotes from your favorite feed
-quotes = get_history_from_feed("MSFT")
+quotes = get_historical_quotes("MSFT")
 
 # calculate indicator series
 results = indicators.get_ema(quotes, 20)
 
 # find result on a specific date
 from datetime import datetime
 lookup_date = datetime(2018, 10, 12)
```

### Comparing `stock-indicators-1.2.1/pyproject.toml` & `stock_indicators-1.3.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     'Operating System :: Unix',
     'Operating System :: MacOS',
     'Typing :: Typed'
 ]
 requires-python = ">=3.8"
 dependencies = [
     "pythonnet>=3.0.0",
-    "typing_extensions>=4.0.0"
+    "typing_extensions>=4.4.0"
 ]
 keywords = [
 "Stock Indicators", "Technical Indicators", "Market", "Technical Analysis", "Algorithmic", "Trading", "Trade",
 "Momentum", "Finance", "Algorithm", "Algo", "AlgoTrading", "Financial", "Strategy", "Chart", "Charting",
 "Oscillator", "Overlay", "Equity", "Bitcoin", "Crypto", "Cryptocurrency", "Forex", "Quantitative",
 "Historical", "Quotes", "Accumulation", "Distribution", "ADL", "Aroon", "True Range", "ATR",
 "Bollinger Bands", "Commodity", "CCI", "Chandelier Exit", "Chaikin Money Flow", "CMF", "MFI",
@@ -46,18 +46,18 @@
 "Slope", "Standard Deviation", "Beta", "Convexity", "Correlation", "SuperTrend", "Ulcer", "Ultimate",
 "Vortex", "Williams %R", "Alligator", "Gator", "Fractal", "Chaos", "Choppiness", "Endpoint", "WMA", "ZigZag"]
 
 dynamic = ["version"]
 
 [project.urls]
 Homepage = "https://python.stockindicators.dev"
-"Bug Tracker" = "https://github.com/DaveSkender/Stock.Indicators.Python/issues"
+"Bug Tracker" = "https://github.com/facioquo/stock-indicators-python/issues"
 Documentation = "https://python.stockindicators.dev"
-"Source Code" = "https://github.com/DaveSkender/Stock.Indicators.Python/tree/main"
-"Release Notes" = "https://github.com/DaveSkender/Stock.Indicators.Python/releases"
+"Source Code" = "https://github.com/facioquo/stock-indicators-python/tree/main"
+"Release Notes" = "https://github.com/facioquo/stock-indicators-python/releases"
 
 [tool.setuptools.packages.find]
 exclude = ["tests*", "benchmarks*", "samples*", "docs*"]
 
 # can be empty if no extra settings are needed, presence enables setuptools_scm
 [tool.setuptools_scm]
 local_scheme = "no-local-version"
```

### Comparing `stock-indicators-1.2.1/samples/quotes/Bad.csv` & `stock_indicators-1.3.0/samples/quotes/Bad.csv`

 * *Files identical despite different names*

### Comparing `stock-indicators-1.2.1/samples/quotes/Bitcoin.csv` & `stock_indicators-1.3.0/samples/quotes/Bitcoin.csv`

 * *Files identical despite different names*

### Comparing `stock-indicators-1.2.1/samples/quotes/Compare.csv` & `stock_indicators-1.3.0/samples/quotes/Compare.csv`

 * *Files identical despite different names*

### Comparing `stock-indicators-1.2.1/samples/quotes/Default.csv` & `stock_indicators-1.3.0/samples/quotes/Default.csv`

 * *Files identical despite different names*

### Comparing `stock-indicators-1.2.1/samples/quotes/History.xlsx` & `stock_indicators-1.3.0/samples/quotes/History.xlsx`

 * *Files identical despite different names*

### Comparing `stock-indicators-1.2.1/samples/quotes/Intraday.csv` & `stock_indicators-1.3.0/samples/quotes/Intraday.csv`

 * *Files identical despite different names*

### Comparing `stock-indicators-1.2.1/samples/quotes/Longest.csv` & `stock_indicators-1.3.0/samples/quotes/Longest.csv`

 * *Files identical despite different names*

### Comparing `stock-indicators-1.2.1/samples/quotes/Longish.csv` & `stock_indicators-1.3.0/samples/quotes/Longish.csv`

 * *Files identical despite different names*

### Comparing `stock-indicators-1.2.1/samples/quotes/MSFT.csv` & `stock_indicators-1.3.0/samples/quotes/MSFT.csv`

 * *Files identical despite different names*

### Comparing `stock-indicators-1.2.1/samples/quotes/Max.csv` & `stock_indicators-1.3.0/samples/quotes/Max.csv`

 * *Files identical despite different names*

### Comparing `stock-indicators-1.2.1/samples/quotes/Mismatch.csv` & `stock_indicators-1.3.0/samples/quotes/Mismatch.csv`

 * *Files identical despite different names*

### Comparing `stock-indicators-1.2.1/samples/quotes/Penny.csv` & `stock_indicators-1.3.0/samples/quotes/Penny.csv`

 * *Files identical despite different names*

### Comparing `stock-indicators-1.2.1/samples/quotes/SPX.csv` & `stock_indicators-1.3.0/samples/quotes/SPX.csv`

 * *Files identical despite different names*

### Comparing `stock-indicators-1.2.1/samples/quotes/TooBig.csv` & `stock_indicators-1.3.0/samples/quotes/TooBig.csv`

 * *Files identical despite different names*

### Comparing `stock-indicators-1.2.1/samples/quotes/ZigZag.csv` & `stock_indicators-1.3.0/samples/quotes/ZigZag.csv`

 * *Files identical despite different names*

### Comparing `stock-indicators-1.2.1/samples/zig_zag/data.ethusdt.json` & `stock_indicators-1.3.0/samples/zig_zag/data.ethusdt.json`

 * *Files identical despite different names*

### Comparing `stock-indicators-1.2.1/samples/zig_zag/data.issue632.json` & `stock_indicators-1.3.0/samples/zig_zag/data.issue632.json`

 * *Files identical despite different names*

### Comparing `stock-indicators-1.2.1/samples/zig_zag/data.schrodinger.json` & `stock_indicators-1.3.0/samples/zig_zag/data.schrodinger.json`

 * *Files identical despite different names*

### Comparing `stock-indicators-1.2.1/stock_indicators/__init__.py` & `stock_indicators-1.3.0/stock_indicators/__init__.py`

 * *Files identical despite different names*

### Comparing `stock-indicators-1.2.1/stock_indicators/_cslib/__init__.py` & `stock_indicators-1.3.0/stock_indicators/_cslib/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,24 +26,24 @@
 clr.AddReference('System.Collections')
 
 # Built-in
 from System import DateTime as CsDateTime
 from System import Decimal as CsDecimal
 from System import Enum as CsEnum
 from System.Globalization import CultureInfo
+from System.Collections.Generic import IEnumerable as CsIEnumerable
 from System.Collections.Generic import List as CsList
 
 # Classes
 from Skender.Stock.Indicators import CandleProperties as CsCandleProperties
 from Skender.Stock.Indicators import Indicator as CsIndicator
 from Skender.Stock.Indicators import Quote as CsQuote
 from Skender.Stock.Indicators import QuoteUtility as CsQuoteUtility
 from Skender.Stock.Indicators import ResultBase as CsResultBase
-from Skender.Stock.Indicators import Pruning as CsPruning
-from Skender.Stock.Indicators import Seeking as CsSeeking
+from Skender.Stock.Indicators import ResultUtility as CsResultUtility
 
 # Enums
 from Skender.Stock.Indicators import BetaType as CsBetaType
 from Skender.Stock.Indicators import CandlePart as CsCandlePart
 from Skender.Stock.Indicators import ChandelierType as CsChandelierType
 from Skender.Stock.Indicators import EndType as CsEndType
 from Skender.Stock.Indicators import MaType as CsMaType
```

### Comparing `stock-indicators-1.2.1/stock_indicators/_cslib/lib/Skender.Stock.Indicators.dll` & `stock_indicators-1.3.0/stock_indicators/_cslib/lib/Skender.Stock.Indicators.dll`

 * *Files identical despite different names*

### Comparing `stock-indicators-1.2.1/stock_indicators/_cstypes/datetime.py` & `stock_indicators-1.3.0/stock_indicators/_cstypes/datetime.py`

 * *Files identical despite different names*

### Comparing `stock-indicators-1.2.1/stock_indicators/_cstypes/decimal.py` & `stock_indicators-1.3.0/stock_indicators/_cstypes/decimal.py`

 * *Files identical despite different names*

### Comparing `stock-indicators-1.2.1/stock_indicators/_cstypes/list.py` & `stock_indicators-1.3.0/stock_indicators/_cstypes/list.py`

 * *Files identical despite different names*

### Comparing `stock-indicators-1.2.1/stock_indicators/indicators/__init__.py` & `stock_indicators-1.3.0/stock_indicators/indicators/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,31 +3,34 @@
 from stock_indicators import _cslib
 
 from .adl import (get_adl)
 from .adx import (get_adx)
 from .alligator import (get_alligator)
 from .alma import (get_alma)
 from .aroon import (get_aroon)
+from .atr_stop import (get_atr_stop)
 from .atr import (get_atr)
 from .awesome import (get_awesome)
 from .basic_quotes import (get_basic_quote)
 from .beta import (get_beta)
 from .bollinger_bands import (get_bollinger_bands)
 from .bop import (get_bop)
 from .cci import (get_cci)
 from .chaikin_oscillator import (get_chaikin_osc)
 from .chandelier import (get_chandelier)
 from .chop import (get_chop)
 from .cmf import (get_cmf)
+from .cmo import (get_cmo)
 from .connors_rsi import (get_connors_rsi)
 from .correlation import (get_correlation)
 from .doji import (get_doji)
 from .donchian import (get_donchian)
 from .dema import (get_dema)
 from .dpo import (get_dpo)
+from .dynamic import (get_dynamic)
 from .elder_ray import (get_elder_ray)
 from .ema import (get_ema)
 from .epma import (get_epma)
 from .fcb import (get_fcb)
 from .fisher_transform import (get_fisher_transform)
 from .force_index import (get_force_index)
 from .fractal import (get_fractal)
```

### Comparing `stock-indicators-1.2.1/stock_indicators/indicators/adl.py` & `stock_indicators-1.3.0/stock_indicators/indicators/adl.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from typing import Iterable, Optional, TypeVar
 
 from stock_indicators._cslib import CsIndicator
 from stock_indicators._cstypes import List as CsList
+from stock_indicators.indicators.common.helpers import CondenseMixin
 from stock_indicators.indicators.common.results import IndicatorResults, ResultBase
 from stock_indicators.indicators.common.quote import Quote
 
 
 def get_adl(quotes: Iterable[Quote], sma_periods: Optional[int] = None):
     """Get ADL calculated.
 
@@ -65,13 +66,13 @@
 
     @adl_sma.setter
     def adl_sma(self, value):
         self._csdata.AdlSma = value
 
 
 _T = TypeVar("_T", bound=ADLResult)
-class ADLResults(IndicatorResults[_T]):
+class ADLResults(CondenseMixin, IndicatorResults[_T]):
     """
     A wrapper class for the list of ADL(Accumulation/Distribution Line) results.
     It is exactly same with built-in `list` except for that it provides
     some useful helper methods written in C# implementation.
     """
```

### Comparing `stock-indicators-1.2.1/stock_indicators/indicators/adx.py` & `stock_indicators-1.3.0/stock_indicators/indicators/adx.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Iterable, Optional, TypeVar
 
 from stock_indicators._cslib import CsIndicator
 from stock_indicators._cstypes import List as CsList
-from stock_indicators.indicators.common.helpers import RemoveWarmupMixin
+from stock_indicators.indicators.common.helpers import CondenseMixin, RemoveWarmupMixin
 from stock_indicators.indicators.common.results import IndicatorResults, ResultBase
 from stock_indicators.indicators.common.quote import Quote
 
 
 def get_adx(quotes: Iterable[Quote], lookback_periods: int = 14):
     """Get ADX calculated.
 
@@ -67,13 +67,13 @@
 
     @adxr.setter
     def adxr(self, value):
         self._csdata.Adxr = value
 
 
 _T = TypeVar("_T", bound=ADXResult)
-class ADXResults(RemoveWarmupMixin, IndicatorResults[_T]):
+class ADXResults(CondenseMixin, RemoveWarmupMixin, IndicatorResults[_T]):
     """
     A wrapper class for the list of ADX(Average Directional Movement Index) results.
     It is exactly same with built-in `list` except for that it provides
     some useful helper methods written in C# implementation.
     """
```

### Comparing `stock-indicators-1.2.1/stock_indicators/indicators/alligator.py` & `stock_indicators-1.3.0/stock_indicators/indicators/alligator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Iterable, Optional, TypeVar
 
 from stock_indicators._cslib import CsIndicator
 from stock_indicators._cstypes import List as CsList
-from stock_indicators.indicators.common.helpers import RemoveWarmupMixin
+from stock_indicators.indicators.common.helpers import CondenseMixin, RemoveWarmupMixin
 from stock_indicators.indicators.common.results import IndicatorResults, ResultBase
 from stock_indicators.indicators.common.quote import Quote
 
 
 def get_alligator(quotes: Iterable[Quote],
                   jaw_periods: int = 13, jaw_offset: int = 8,
                   teeth_periods: int = 8, teeth_offset: int = 5,
@@ -81,13 +81,13 @@
 
     @lips.setter
     def lips(self, value):
         self._csdata.Lips = value
 
 
 _T = TypeVar("_T", bound=AlligatorResult)
-class AlligatorResults(RemoveWarmupMixin, IndicatorResults[_T]):
+class AlligatorResults(CondenseMixin, RemoveWarmupMixin, IndicatorResults[_T]):
     """
     A wrapper class for the list of Williams Alligator results.
     It is exactly same with built-in `list` except for that it provides
     some useful helper methods written in C# implementation.
     """
```

### Comparing `stock-indicators-1.2.1/stock_indicators/indicators/alma.py` & `stock_indicators-1.3.0/stock_indicators/indicators/alma.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Iterable, Optional, TypeVar
 
 from stock_indicators._cslib import CsIndicator
 from stock_indicators._cstypes import List as CsList
-from stock_indicators.indicators.common.helpers import RemoveWarmupMixin
+from stock_indicators.indicators.common.helpers import CondenseMixin, RemoveWarmupMixin
 from stock_indicators.indicators.common.quote import Quote
 from stock_indicators.indicators.common.results import IndicatorResults, ResultBase
 
 
 def get_alma(quotes: Iterable[Quote], lookback_periods: int = 9, offset: float = .85, sigma : float = 6):
     """Get ALMA calculated.
 
@@ -49,13 +49,13 @@
 
     @alma.setter
     def alma(self, value):
         self._csdata.Alma = value
 
 
 _T = TypeVar("_T", bound=ALMAResult)
-class ALMAResults(RemoveWarmupMixin, IndicatorResults[_T]):
+class ALMAResults(CondenseMixin, RemoveWarmupMixin, IndicatorResults[_T]):
     """
     A wrapper class for the list of ALMA(Arnaud Legoux Moving Average) results.
     It is exactly same with built-in `list` except for that it provides
     some useful helper methods written in CSharp implementation.
     """
```

### Comparing `stock-indicators-1.2.1/stock_indicators/indicators/aroon.py` & `stock_indicators-1.3.0/stock_indicators/indicators/aroon.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Iterable, Optional, TypeVar
 
 from stock_indicators._cslib import CsIndicator
 from stock_indicators._cstypes import List as CsList
-from stock_indicators.indicators.common.helpers import RemoveWarmupMixin
+from stock_indicators.indicators.common.helpers import CondenseMixin, RemoveWarmupMixin
 from stock_indicators.indicators.common.results import IndicatorResults, ResultBase
 from stock_indicators.indicators.common.quote import Quote
 
 
 def get_aroon(quotes: Iterable[Quote], lookback_periods: int = 25):
     """Get Aroon calculated.
 
@@ -58,13 +58,13 @@
 
     @oscillator.setter
     def oscillator(self, value):
         self._csdata.Oscillator = value
 
 
 _T = TypeVar("_T", bound=AroonResult)
-class AroonResults(RemoveWarmupMixin, IndicatorResults[_T]):
+class AroonResults(CondenseMixin, RemoveWarmupMixin, IndicatorResults[_T]):
     """
     A wrapper class for the list of Aroon results.
     It is exactly same with built-in `list` except for that it provides
     some useful helper methods written in C# implementation.
     """
```

### Comparing `stock-indicators-1.2.1/stock_indicators/indicators/atr.py` & `stock_indicators-1.3.0/stock_indicators/indicators/atr.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Iterable, Optional, TypeVar
 
 from stock_indicators._cslib import CsIndicator
 from stock_indicators._cstypes import List as CsList
-from stock_indicators.indicators.common.helpers import RemoveWarmupMixin
+from stock_indicators.indicators.common.helpers import CondenseMixin, RemoveWarmupMixin
 from stock_indicators.indicators.common.results import IndicatorResults, ResultBase
 from stock_indicators.indicators.common.quote import Quote
 
 
 def get_atr(quotes: Iterable[Quote], lookback_periods: int = 14):
     """Get ATR calculated.
 
@@ -58,13 +58,13 @@
 
     @atrp.setter
     def atrp(self, value):
         self._csdata.Atrp = value
 
 
 _T = TypeVar("_T", bound=ATRResult)
-class ATRResults(RemoveWarmupMixin, IndicatorResults[_T]):
+class ATRResults(CondenseMixin, RemoveWarmupMixin, IndicatorResults[_T]):
     """
     A wrapper class for the list of ATR(Average True Range) results.
     It is exactly same with built-in `list` except for that it provides
     some useful helper methods written in C# implementation.
     """
```

### Comparing `stock-indicators-1.2.1/stock_indicators/indicators/awesome.py` & `stock_indicators-1.3.0/stock_indicators/indicators/awesome.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Iterable, Optional, TypeVar
 
 from stock_indicators._cslib import CsIndicator
 from stock_indicators._cstypes import List as CsList
-from stock_indicators.indicators.common.helpers import RemoveWarmupMixin
+from stock_indicators.indicators.common.helpers import CondenseMixin, RemoveWarmupMixin
 from stock_indicators.indicators.common.results import IndicatorResults, ResultBase
 from stock_indicators.indicators.common.quote import Quote
 
 
 def get_awesome(quotes: Iterable[Quote], fast_periods: int = 5, slow_periods: int = 34):
     """Get Awesome Oscillator calculated.
 
@@ -54,13 +54,13 @@
 
     @normalized.setter
     def normalized(self, value):
         self._csdata.Normalized = value
 
 
 _T = TypeVar("_T", bound=AwesomeResult)
-class AwesomeResults(RemoveWarmupMixin, IndicatorResults[_T]):
+class AwesomeResults(CondenseMixin, RemoveWarmupMixin, IndicatorResults[_T]):
     """
     A wrapper class for the list of Awesome Oscillator (aka Super AO) results.
     It is exactly same with built-in `list` except for that it provides
     some useful helper methods written in C# implementation.
     """
```

### Comparing `stock-indicators-1.2.1/stock_indicators/indicators/basic_quotes.py` & `stock_indicators-1.3.0/stock_indicators/indicators/basic_quotes.py`

 * *Files identical despite different names*

### Comparing `stock-indicators-1.2.1/stock_indicators/indicators/beta.py` & `stock_indicators-1.3.0/stock_indicators/indicators/beta.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import Iterable, Optional, TypeVar
 
 from stock_indicators._cslib import CsIndicator
 from stock_indicators._cstypes import List as CsList
 from stock_indicators.indicators.common.enums import BetaType
-from stock_indicators.indicators.common.helpers import RemoveWarmupMixin
+from stock_indicators.indicators.common.helpers import CondenseMixin, RemoveWarmupMixin
 from stock_indicators.indicators.common.results import IndicatorResults, ResultBase
 from stock_indicators.indicators.common.quote import Quote
 
 
 def get_beta(eval_quotes: Iterable[Quote], market_quotes: Iterable[Quote],
              lookback_periods: int, beta_type: BetaType = BetaType.STANDARD):
     """Get Beta calculated.
@@ -102,13 +102,13 @@
     def returns_mrkt(self, value):
         self._csdata.ReturnsMrkt = value
 
 
 _T = TypeVar("_T", bound=BetaResult)
 
 
-class BetaResults(RemoveWarmupMixin, IndicatorResults[_T]):
+class BetaResults(CondenseMixin, RemoveWarmupMixin, IndicatorResults[_T]):
     """
     A wrapper class for the list of Beta results.
     It is exactly same with built-in `list` except for that it provides
     some useful helper methods written in C# implementation.
     """
```

### Comparing `stock-indicators-1.2.1/stock_indicators/indicators/bollinger_bands.py` & `stock_indicators-1.3.0/stock_indicators/indicators/bollinger_bands.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Iterable, Optional, TypeVar
 
 from stock_indicators._cslib import CsIndicator
 from stock_indicators._cstypes import List as CsList
-from stock_indicators.indicators.common.helpers import RemoveWarmupMixin
+from stock_indicators.indicators.common.helpers import CondenseMixin, RemoveWarmupMixin
 from stock_indicators.indicators.common.results import IndicatorResults, ResultBase
 from stock_indicators.indicators.common.quote import Quote
 
 
 def get_bollinger_bands(quotes: Iterable[Quote], lookback_periods: int = 20, standard_deviations: float = 2):
     """Get Bollinger Bands&#174; calculated.
 
@@ -86,13 +86,13 @@
 
     @width.setter
     def width(self, value):
         self._csdata.Width = value
 
 
 _T = TypeVar("_T", bound=BollingerBandsResult)
-class BollingerBandsResults(RemoveWarmupMixin, IndicatorResults[_T]):
+class BollingerBandsResults(CondenseMixin, RemoveWarmupMixin, IndicatorResults[_T]):
     """
     A wrapper class for the list of Bollinger Bands results.
     It is exactly same with built-in `list` except for that it provides
     some useful helper methods written in C# implementation.
     """
```

### Comparing `stock-indicators-1.2.1/stock_indicators/indicators/bop.py` & `stock_indicators-1.3.0/stock_indicators/indicators/bop.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Iterable, Optional, TypeVar
 
 from stock_indicators._cslib import CsIndicator
 from stock_indicators._cstypes import List as CsList
-from stock_indicators.indicators.common.helpers import RemoveWarmupMixin
+from stock_indicators.indicators.common.helpers import CondenseMixin, RemoveWarmupMixin
 from stock_indicators.indicators.common.results import IndicatorResults, ResultBase
 from stock_indicators.indicators.common.quote import Quote
 
 
 def get_bop(quotes: Iterable[Quote], smooth_periods: int = 14):
     """Get BOP calculated.
 
@@ -44,13 +44,13 @@
 
     @bop.setter
     def bop(self, value):
         self._csdata.Bop = value
 
 
 _T = TypeVar("_T", bound=BOPResult)
-class BOPResults(RemoveWarmupMixin, IndicatorResults[_T]):
+class BOPResults(CondenseMixin, RemoveWarmupMixin, IndicatorResults[_T]):
     """
     A wrapper class for the list of Balance of Power (aka Balance of Market Power) results.
     It is exactly same with built-in `list` except for that it provides
     some useful helper methods written in C# implementation.
     """
```

### Comparing `stock-indicators-1.2.1/stock_indicators/indicators/cci.py` & `stock_indicators-1.3.0/stock_indicators/indicators/cci.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Iterable, Optional, TypeVar
 
 from stock_indicators._cslib import CsIndicator
 from stock_indicators._cstypes import List as CsList
-from stock_indicators.indicators.common.helpers import RemoveWarmupMixin
+from stock_indicators.indicators.common.helpers import CondenseMixin, RemoveWarmupMixin
 from stock_indicators.indicators.common.results import IndicatorResults, ResultBase
 from stock_indicators.indicators.common.quote import Quote
 
 
 def get_cci(quotes: Iterable[Quote], lookback_periods: int = 20):
     """Get CCI calculated.
 
@@ -43,13 +43,13 @@
 
     @cci.setter
     def cci(self, value):
         self._csdata.Cci = value
 
 
 _T = TypeVar("_T", bound=CCIResult)
-class CCIResults(RemoveWarmupMixin, IndicatorResults[_T]):
+class CCIResults(CondenseMixin, RemoveWarmupMixin, IndicatorResults[_T]):
     """
     A wrapper class for the list of Commodity Channel Index (CCI) results.
     It is exactly same with built-in `list` except for that it provides
     some useful helper methods written in CSharp implementation.
     """
```

### Comparing `stock-indicators-1.2.1/stock_indicators/indicators/chaikin_oscillator.py` & `stock_indicators-1.3.0/stock_indicators/indicators/chaikin_oscillator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Iterable, Optional, TypeVar
 
 from stock_indicators._cslib import CsIndicator
 from stock_indicators._cstypes import List as CsList
-from stock_indicators.indicators.common.helpers import RemoveWarmupMixin
+from stock_indicators.indicators.common.helpers import CondenseMixin, RemoveWarmupMixin
 from stock_indicators.indicators.common.results import IndicatorResults, ResultBase
 from stock_indicators.indicators.common.quote import Quote
 
 
 def get_chaikin_osc(quotes: Iterable[Quote], fast_periods: int = 3, slow_periods: int = 10):
     """Get Chaikin Oscillator calculated.
 
@@ -70,13 +70,13 @@
 
     @oscillator.setter
     def oscillator(self, value):
         self._csdata.Oscillator = value
 
 
 _T = TypeVar("_T", bound=ChaikinOscResult)
-class ChaikinOscResults(RemoveWarmupMixin, IndicatorResults[_T]):
+class ChaikinOscResults(CondenseMixin, RemoveWarmupMixin, IndicatorResults[_T]):
     """
     A wrapper class for the list of Chaikin Oscillator results.
     It is exactly same with built-in `list` except for that it provides
     some useful helper methods written in CSharp implementation.
     """
```

### Comparing `stock-indicators-1.2.1/stock_indicators/indicators/chandelier.py` & `stock_indicators-1.3.0/stock_indicators/indicators/chandelier.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import Iterable, Optional, TypeVar
 
 from stock_indicators._cslib import CsIndicator
 from stock_indicators._cstypes import List as CsList
 from stock_indicators.indicators.common.enums import ChandelierType
-from stock_indicators.indicators.common.helpers import RemoveWarmupMixin
+from stock_indicators.indicators.common.helpers import CondenseMixin, RemoveWarmupMixin
 from stock_indicators.indicators.common.results import IndicatorResults, ResultBase
 from stock_indicators.indicators.common.quote import Quote
 
 
 def get_chandelier(quotes: Iterable[Quote], lookback_periods: int = 22,
                    multiplier: float = 3, chandelier_type: ChandelierType = ChandelierType.LONG):
     """Get Chandelier Exit calculated.
@@ -52,13 +52,13 @@
 
     @chandelier_exit.setter
     def chandelier_exit(self, value):
         self._csdata.ChandelierExit = value
 
 
 _T = TypeVar("_T", bound=ChandelierResult)
-class ChandelierResults(RemoveWarmupMixin, IndicatorResults[_T]):
+class ChandelierResults(CondenseMixin, RemoveWarmupMixin, IndicatorResults[_T]):
     """
     A wrapper class for the list of Chandelier Exit results.
     It is exactly same with built-in `list` except for that it provides
     some useful helper methods written in C# implementation.
     """
```

### Comparing `stock-indicators-1.2.1/stock_indicators/indicators/chop.py` & `stock_indicators-1.3.0/stock_indicators/indicators/chop.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Iterable, Optional, TypeVar
 
 from stock_indicators._cslib import CsIndicator
 from stock_indicators._cstypes import List as CsList
-from stock_indicators.indicators.common.helpers import RemoveWarmupMixin
+from stock_indicators.indicators.common.helpers import CondenseMixin, RemoveWarmupMixin
 from stock_indicators.indicators.common.results import IndicatorResults, ResultBase
 from stock_indicators.indicators.common.quote import Quote
 
 
 def get_chop(quotes: Iterable[Quote], lookback_periods: int = 14):
     """Get Choppiness Index calculated.
 
@@ -43,13 +43,13 @@
 
     @chop.setter
     def chop(self, value):
         self._csdata.Chop = value
 
 
 _T = TypeVar("_T", bound=ChopResult)
-class ChopResults(RemoveWarmupMixin, IndicatorResults[_T]):
+class ChopResults(CondenseMixin, RemoveWarmupMixin, IndicatorResults[_T]):
     """
     A wrapper class for the list of Choppiness Index (CHOP) results.
     It is exactly same with built-in `list` except for that it provides
     some useful helper methods written in CSharp implementation.
     """
```

### Comparing `stock-indicators-1.2.1/stock_indicators/indicators/cmf.py` & `stock_indicators-1.3.0/stock_indicators/indicators/cmf.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Iterable, Optional, TypeVar
 
 from stock_indicators._cslib import CsIndicator
 from stock_indicators._cstypes import List as CsList
-from stock_indicators.indicators.common.helpers import RemoveWarmupMixin
+from stock_indicators.indicators.common.helpers import CondenseMixin, RemoveWarmupMixin
 from stock_indicators.indicators.common.results import IndicatorResults, ResultBase
 from stock_indicators.indicators.common.quote import Quote
 
 
 def get_cmf(quotes: Iterable[Quote], lookback_periods: int = 20):
     """Get CMF calculated.
 
@@ -59,13 +59,13 @@
 
     @cmf.setter
     def cmf(self, value):
         self._csdata.Cmf = value
 
 
 _T = TypeVar("_T", bound=CMFResult)
-class CMFResults(RemoveWarmupMixin, IndicatorResults[_T]):
+class CMFResults(CondenseMixin, RemoveWarmupMixin, IndicatorResults[_T]):
     """
     A wrapper class for the list of Chaikin Money Flow (CMF) results.
     It is exactly same with built-in `list` except for that it provides
     some useful helper methods written in CSharp implementation.
     """
```

### Comparing `stock-indicators-1.2.1/stock_indicators/indicators/common/__init__.py` & `stock_indicators-1.3.0/stock_indicators/indicators/common/__init__.py`

 * *Files identical despite different names*

### Comparing `stock-indicators-1.2.1/stock_indicators/indicators/common/candles.py` & `stock_indicators-1.3.0/stock_indicators/indicators/common/candles.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,31 +1,21 @@
 from decimal import Decimal
 from typing import Optional, TypeVar
-
-from typing_extensions import Self
+from typing_extensions import override
 
 from stock_indicators._cslib import CsCandleProperties
 from stock_indicators._cstypes import Decimal as CsDecimal
 from stock_indicators._cstypes import to_pydecimal
 from stock_indicators.indicators.common._contrib.type_resolver import generate_cs_inherited_class
 from stock_indicators.indicators.common.enums import Match
+from stock_indicators.indicators.common.helpers import CondenseMixin
 from stock_indicators.indicators.common.quote import _Quote
 from stock_indicators.indicators.common.results import IndicatorResults, ResultBase
 
 
-class CondenseMixin:
-    """Mixin for condense()."""
-    @IndicatorResults._verify_data
-    def condense(self) -> Self:
-        """
-        Remove results which have no match, so it only returns meaningful data records.
-        """
-        return self.__class__(filter(lambda x: x.match != Match.NONE, self), self._wrapper_class)
-
-
 class _CandleProperties(_Quote):
     @property
     def size(self) -> Optional[Decimal]:
         return to_pydecimal(self.high - self.low)
 
     @property
     def body(self) -> Optional[Decimal]:
@@ -111,7 +101,11 @@
 _T = TypeVar("_T", bound=CandleResult)
 class CandleResults(CondenseMixin, IndicatorResults[_T]):
     """
     A wrapper class for the list of Candlestick pattern results.
     It is exactly same with built-in `list` except for that it provides
     some useful helper methods written in CSharp implementation.
     """
+
+    @override
+    def condense(self):
+        return self.__class__(filter(lambda x: x.match != Match.NONE, self), self._wrapper_class)
```

### Comparing `stock-indicators-1.2.1/stock_indicators/indicators/common/enums.py` & `stock_indicators-1.3.0/stock_indicators/indicators/common/enums.py`

 * *Files identical despite different names*

### Comparing `stock-indicators-1.2.1/stock_indicators/indicators/common/quote.py` & `stock_indicators-1.3.0/stock_indicators/indicators/common/quote.py`

 * *Files identical despite different names*

### Comparing `stock-indicators-1.2.1/stock_indicators/indicators/common/results.py` & `stock_indicators-1.3.0/stock_indicators/indicators/common/results.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from datetime import datetime as PyDateTime
-from typing import Callable, Iterable, List, Type, TypeVar
+from typing import Callable, Iterable, List, Optional, Type, TypeVar
+from warnings import warn
 
-from stock_indicators._cslib import CsResultBase, CsPruning, CsSeeking
+from stock_indicators._cslib import CsResultBase
 from stock_indicators._cstypes import DateTime as CsDateTime
-from stock_indicators._cstypes import List as CsList
 from stock_indicators._cstypes import to_pydatetime
 
 
 class ResultBase:
     """A base wrapper class for a single unit of the results."""
     def __init__(self, base_result: CsResultBase):
         super().__init__()
@@ -32,25 +32,29 @@
         super().__init__([ wrapper_class(_) for _ in data ])
         self._csdata = data
         self._wrapper_class = wrapper_class
 
     def reload(self):
         """
         Reload a C# array of the results to perform more operations.
-        It is usually called after `done()`
+        It is usually called after `done()`.
+        This method is deprecated. It will be removed in the next version.
         """
+        warn('This method is deprecated.', DeprecationWarning, stacklevel=2)
         if self._csdata is None:
             self._csdata = [ _._csdata for _ in self ]
         return self
 
     def done(self):
         """
         Remove a C# array of the results after finishing all operations.
         It is not necessary but saves memory.
+        This method is deprecated. It will be removed in the next version.
         """
+        warn('This method is deprecated.', DeprecationWarning, stacklevel=2)
         self._csdata = None
         return self
 
     def _get_csdata_type(self):
         """Get C# result object type."""
         return type(self[0]._csdata)
 
@@ -74,33 +78,20 @@
         return self.__class__(list(self._csdata).__add__(list(other._csdata)), self._wrapper_class)
 
     @_verify_data
     def __mul__(self, value: int):
         return self.__class__(list(self._csdata).__mul__(value), self._wrapper_class)
 
     @_verify_data
-    def find(self, lookup_date: PyDateTime) -> _T:
-        """Find indicator values on a specific date."""
-        if not isinstance(lookup_date, PyDateTime):
-            raise TypeError(
-                "lookup_date must be an instance of datetime.datetime."
-            )
-
-        result = CsSeeking.Find[CsResultBase](
-            CsList(self._get_csdata_type(), self._csdata), CsDateTime(lookup_date)
-        )
-        return self._wrapper_class(result)
-
-    @_verify_data
     def remove_warmup_periods(self, remove_periods: int):
-        """
-        Remove a specific quantity of results from the beginning of the results list.
-        """
+        """Remove a specific quantity of results from the beginning of the results list."""
         if not isinstance(remove_periods, int):
-            raise TypeError(
-                "remove_periods must be an integer."
-            )
-
-        removed_results = CsPruning.RemoveWarmupPeriods[CsResultBase](
-            CsList(self._get_csdata_type(), self._csdata), remove_periods
-        )
-        return self.__class__(removed_results, self._wrapper_class)
+            raise TypeError("remove_periods must be an integer.")
+
+        return self.__class__(list(self._csdata)[remove_periods:], self._wrapper_class)
+
+    def find(self, lookup_date: PyDateTime) -> Optional[_T]:
+        """Find indicator values on a specific date. It returns `None` if no result found."""
+        if not isinstance(lookup_date, PyDateTime):
+            raise TypeError("lookup_date must be an instance of datetime.datetime.")
+
+        return next((r for r in self if r.date == lookup_date), None)
```

### Comparing `stock-indicators-1.2.1/stock_indicators/indicators/connors_rsi.py` & `stock_indicators-1.3.0/stock_indicators/indicators/connors_rsi.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Iterable, Optional, TypeVar
 
 from stock_indicators._cslib import CsIndicator
 from stock_indicators._cstypes import List as CsList
-from stock_indicators.indicators.common.helpers import RemoveWarmupMixin
+from stock_indicators.indicators.common.helpers import CondenseMixin, RemoveWarmupMixin
 from stock_indicators.indicators.common.results import IndicatorResults, ResultBase
 from stock_indicators.indicators.common.quote import Quote
 
 
 def get_connors_rsi(quotes: Iterable[Quote], rsi_periods: int = 3,
                     streak_periods: int = 2, rank_periods: int = 100):
     """Get Connors RSI calculated.
@@ -77,13 +77,13 @@
 
     @connors_rsi.setter
     def connors_rsi(self, value):
         self._csdata.ConnorsRsi = value
 
 
 _T = TypeVar("_T", bound=ConnorsRSIResult)
-class ConnorsRSIResults(RemoveWarmupMixin, IndicatorResults[_T]):
+class ConnorsRSIResults(CondenseMixin, RemoveWarmupMixin, IndicatorResults[_T]):
     """
     A wrapper class for the list of Connors RSI results.
     It is exactly same with built-in `list` except for that it provides
     some useful helper methods written in CSharp implementation.
     """
```

### Comparing `stock-indicators-1.2.1/stock_indicators/indicators/correlation.py` & `stock_indicators-1.3.0/stock_indicators/indicators/correlation.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Iterable, Optional, TypeVar
 
 from stock_indicators._cslib import CsIndicator
 from stock_indicators._cstypes import List as CsList
-from stock_indicators.indicators.common.helpers import RemoveWarmupMixin
+from stock_indicators.indicators.common.helpers import CondenseMixin, RemoveWarmupMixin
 from stock_indicators.indicators.common.results import IndicatorResults, ResultBase
 from stock_indicators.indicators.common.quote import Quote
 
 
 def get_correlation(quotes_a: Iterable[Quote], quotes_b: Iterable[Quote],
                     lookback_periods: int):
     """Get Correlation Coefficient calculated.
@@ -79,13 +79,13 @@
 
     @r_squared.setter
     def r_squared(self, value):
         self._csdata.RSquared = value
 
 
 _T = TypeVar("_T", bound=CorrelationResult)
-class CorrelationResults(RemoveWarmupMixin, IndicatorResults[_T]):
+class CorrelationResults(CondenseMixin, RemoveWarmupMixin, IndicatorResults[_T]):
     """
     A wrapper class for the list of Correlation Coefficient results.
     It is exactly same with built-in `list` except for that it provides
     some useful helper methods written in CSharp implementation.
     """
```

### Comparing `stock-indicators-1.2.1/stock_indicators/indicators/dema.py` & `stock_indicators-1.3.0/stock_indicators/indicators/dema.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Iterable, Optional, TypeVar
 
 from stock_indicators._cslib import CsIndicator
 from stock_indicators._cstypes import List as CsList
-from stock_indicators.indicators.common.helpers import RemoveWarmupMixin
+from stock_indicators.indicators.common.helpers import CondenseMixin, RemoveWarmupMixin
 from stock_indicators.indicators.common.results import IndicatorResults, ResultBase
 from stock_indicators.indicators.common.quote import Quote
 
 
 def get_dema(quotes: Iterable[Quote], lookback_periods: int):
     """Get DEMA calculated.
 
@@ -42,13 +42,13 @@
 
     @dema.setter
     def dema(self, value):
         self._csdata.Dema = value
 
 
 _T = TypeVar("_T", bound=DEMAResult)
-class DEMAResults(RemoveWarmupMixin, IndicatorResults[_T]):
+class DEMAResults(CondenseMixin, RemoveWarmupMixin, IndicatorResults[_T]):
     """
     A wrapper class for the list of Double Exponential Moving Average (DEMA) results.
     It is exactly same with built-in `list` except for that it provides
     some useful helper methods written in C# implementation.
     """
```

### Comparing `stock-indicators-1.2.1/stock_indicators/indicators/doji.py` & `stock_indicators-1.3.0/stock_indicators/indicators/doji.py`

 * *Files identical despite different names*

### Comparing `stock-indicators-1.2.1/stock_indicators/indicators/donchian.py` & `stock_indicators-1.3.0/stock_indicators/indicators/donchian.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from decimal import Decimal
 from typing import Iterable, Optional, TypeVar
 
 from stock_indicators._cslib import CsIndicator
 from stock_indicators._cstypes import List as CsList
 from stock_indicators._cstypes import Decimal as CsDecimal
 from stock_indicators._cstypes import to_pydecimal
-from stock_indicators.indicators.common.helpers import RemoveWarmupMixin
+from stock_indicators.indicators.common.helpers import CondenseMixin, RemoveWarmupMixin
 from stock_indicators.indicators.common.results import IndicatorResults, ResultBase
 from stock_indicators.indicators.common.quote import Quote
 
 
 def get_donchian(quotes: Iterable[Quote], lookback_periods: int = 20):
     """Get Donchian Channels calculated.
 
@@ -69,13 +69,13 @@
 
     @width.setter
     def width(self, value):
         self._csdata.Width = CsDecimal(value)
 
 
 _T = TypeVar("_T", bound=DonchianResult)
-class DonchianResults(RemoveWarmupMixin, IndicatorResults[_T]):
+class DonchianResults(CondenseMixin, RemoveWarmupMixin, IndicatorResults[_T]):
     """
     A wrapper class for the list of Donchian Channels results.
     It is exactly same with built-in `list` except for that it provides
     some useful helper methods written in C# implementation.
     """
```

### Comparing `stock-indicators-1.2.1/stock_indicators/indicators/dpo.py` & `stock_indicators-1.3.0/stock_indicators/indicators/dpo.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from typing import Iterable, Optional, TypeVar
 
 from stock_indicators._cslib import CsIndicator
 from stock_indicators._cstypes import List as CsList
+from stock_indicators.indicators.common.helpers import CondenseMixin
 from stock_indicators.indicators.common.results import IndicatorResults, ResultBase
 from stock_indicators.indicators.common.quote import Quote
 
 
 def get_dpo(quotes: Iterable[Quote], lookback_periods: int):
     """Get DPO calculated.
 
@@ -50,13 +51,13 @@
 
     @dpo.setter
     def dpo(self, value):
         self._csdata.Dpo = value
 
 
 _T = TypeVar("_T", bound=DPOResult)
-class DPOResults(IndicatorResults[_T]):
+class DPOResults(CondenseMixin, IndicatorResults[_T]):
     """
     A wrapper class for the list of Detrended Price Oscillator (DPO) results.
     It is exactly same with built-in `list` except for that it provides
     some useful helper methods written in CSharp implementation.
     """
```

### Comparing `stock-indicators-1.2.1/stock_indicators/indicators/elder_ray.py` & `stock_indicators-1.3.0/stock_indicators/indicators/elder_ray.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Iterable, Optional, TypeVar
 
 from stock_indicators._cslib import CsIndicator
 from stock_indicators._cstypes import List as CsList
-from stock_indicators.indicators.common.helpers import RemoveWarmupMixin
+from stock_indicators.indicators.common.helpers import CondenseMixin, RemoveWarmupMixin
 from stock_indicators.indicators.common.results import IndicatorResults, ResultBase
 from stock_indicators.indicators.common.quote import Quote
 
 
 def get_elder_ray(quotes: Iterable[Quote], lookback_periods: int = 13):
     """Get Elder-ray Index calculated.
 
@@ -58,13 +58,13 @@
 
     @bear_power.setter
     def bear_power(self, value):
         self._csdata.BearPower = value
 
 
 _T = TypeVar("_T", bound=ElderRayResult)
-class ElderRayResults(RemoveWarmupMixin, IndicatorResults[_T]):
+class ElderRayResults(CondenseMixin, RemoveWarmupMixin, IndicatorResults[_T]):
     """
     A wrapper class for the list of Elder-ray Index results.
     It is exactly same with built-in `list` except for that it provides
     some useful helper methods written in C# implementation.
     """
```

### Comparing `stock-indicators-1.2.1/stock_indicators/indicators/ema.py` & `stock_indicators-1.3.0/stock_indicators/indicators/ema.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Iterable, Optional, TypeVar
 
 from stock_indicators._cslib import CsIndicator
 from stock_indicators.indicators.common.enums import CandlePart
-from stock_indicators.indicators.common.helpers import RemoveWarmupMixin
+from stock_indicators.indicators.common.helpers import CondenseMixin, RemoveWarmupMixin
 from stock_indicators.indicators.common.results import IndicatorResults, ResultBase
 from stock_indicators.indicators.common.quote import Quote
 
 
 def get_ema(quotes: Iterable[Quote], lookback_periods: int,
             candle_part: CandlePart = CandlePart.CLOSE):
     """Get EMA calculated.
@@ -47,13 +47,13 @@
 
     @ema.setter
     def ema(self, value):
         self._csdata.Ema = value
 
 
 _T = TypeVar("_T", bound=EMAResult)
-class EMAResults(RemoveWarmupMixin, IndicatorResults[_T]):
+class EMAResults(CondenseMixin, RemoveWarmupMixin, IndicatorResults[_T]):
     """
     A wrapper class for the list of EMA(Exponential Moving Average) results.
     It is exactly same with built-in `list` except for that it provides
     some useful helper methods written in CSharp implementation.
     """
```

### Comparing `stock-indicators-1.2.1/stock_indicators/indicators/epma.py` & `stock_indicators-1.3.0/stock_indicators/indicators/epma.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Iterable, Optional, TypeVar
 
 from stock_indicators._cslib import CsIndicator
 from stock_indicators._cstypes import List as CsList
-from stock_indicators.indicators.common.helpers import RemoveWarmupMixin
+from stock_indicators.indicators.common.helpers import CondenseMixin, RemoveWarmupMixin
 from stock_indicators.indicators.common.results import IndicatorResults, ResultBase
 from stock_indicators.indicators.common.quote import Quote
 
 
 def get_epma(quotes: Iterable[Quote], lookback_periods: int):
     """Get EPMA calculated.
 
@@ -44,13 +44,13 @@
 
     @epma.setter
     def epma(self, value):
         self._csdata.Epma = value
 
 
 _T = TypeVar("_T", bound=EPMAResult)
-class EPMAResults(RemoveWarmupMixin, IndicatorResults[_T]):
+class EPMAResults(CondenseMixin, RemoveWarmupMixin, IndicatorResults[_T]):
     """
     A wrapper class for the list of Endpoint Moving Average (EPMA) results.
     It is exactly same with built-in `list` except for that it provides
     some useful helper methods written in CSharp implementation.
     """
```

### Comparing `stock-indicators-1.2.1/stock_indicators/indicators/fcb.py` & `stock_indicators-1.3.0/stock_indicators/indicators/fcb.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from decimal import Decimal
 from typing import Iterable, Optional, TypeVar
 
 from stock_indicators._cslib import CsIndicator
 from stock_indicators._cstypes import List as CsList
 from stock_indicators._cstypes import Decimal as CsDecimal
 from stock_indicators._cstypes import to_pydecimal
-from stock_indicators.indicators.common.helpers import RemoveWarmupMixin
+from stock_indicators.indicators.common.helpers import CondenseMixin, RemoveWarmupMixin
 from stock_indicators.indicators.common.results import IndicatorResults, ResultBase
 from stock_indicators.indicators.common.quote import Quote
 
 
 def get_fcb(quotes: Iterable[Quote], window_span: int = 2):
     """Get FCB calculated.
 
@@ -55,13 +55,13 @@
 
     @lower_band.setter
     def lower_band(self, value):
         self._csdata.LowerBand = CsDecimal(value)
 
 
 _T = TypeVar("_T", bound=FCBResult)
-class FCBResults(RemoveWarmupMixin, IndicatorResults[_T]):
+class FCBResults(CondenseMixin, RemoveWarmupMixin, IndicatorResults[_T]):
     """
     A wrapper class for the list of Fractal Chaos Bands (FCB) results.
     It is exactly same with built-in `list` except for that it provides
     some useful helper methods written in CSharp implementation.
     """
```

### Comparing `stock-indicators-1.2.1/stock_indicators/indicators/fisher_transform.py` & `stock_indicators-1.3.0/stock_indicators/indicators/fisher_transform.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from typing import Iterable, Optional, TypeVar
 
 from stock_indicators._cslib import CsIndicator
 from stock_indicators._cstypes import List as CsList
+from stock_indicators.indicators.common.helpers import CondenseMixin
 from stock_indicators.indicators.common.results import IndicatorResults, ResultBase
 from stock_indicators.indicators.common.quote import Quote
 
 
 def get_fisher_transform(quotes: Iterable[Quote], lookback_periods: int = 10):
     """Get Ehlers Fisher Transform calculated.
 
@@ -51,13 +52,13 @@
 
     @trigger.setter
     def trigger(self, value):
         self._csdata.Trigger = value
 
 
 _T = TypeVar("_T", bound=FisherTransformResult)
-class FisherTransformResults(IndicatorResults[_T]):
+class FisherTransformResults(CondenseMixin, IndicatorResults[_T]):
     """
     A wrapper class for the list of Ehlers Fisher Transform results.
     It is exactly same with built-in `list` except for that it provides
     some useful helper methods written in CSharp implementation.
     """
```

### Comparing `stock-indicators-1.2.1/stock_indicators/indicators/force_index.py` & `stock_indicators-1.3.0/stock_indicators/indicators/force_index.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Iterable, Optional, TypeVar
 
 from stock_indicators._cslib import CsIndicator
 from stock_indicators._cstypes import List as CsList
-from stock_indicators.indicators.common.helpers import RemoveWarmupMixin
+from stock_indicators.indicators.common.helpers import CondenseMixin, RemoveWarmupMixin
 from stock_indicators.indicators.common.results import IndicatorResults, ResultBase
 from stock_indicators.indicators.common.quote import Quote
 
 
 def get_force_index(quotes: Iterable[Quote], lookback_periods: int):
     """Get Force Index calculated.
 
@@ -42,13 +42,13 @@
 
     @force_index.setter
     def force_index(self, value):
         self._csdata.ForceIndex = value
 
 
 _T = TypeVar("_T", bound=ForceIndexResult)
-class ForceIndexResults(RemoveWarmupMixin, IndicatorResults[_T]):
+class ForceIndexResults(CondenseMixin, RemoveWarmupMixin, IndicatorResults[_T]):
     """
     A wrapper class for the list of Force Index results.
     It is exactly same with built-in `list` except for that it provides
     some useful helper methods written in CSharp implementation.
     """
```

### Comparing `stock-indicators-1.2.1/stock_indicators/indicators/fractal.py` & `stock_indicators-1.3.0/stock_indicators/indicators/fractal.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from typing import Iterable, Optional, TypeVar, overload
 
 from stock_indicators._cslib import CsIndicator
 from stock_indicators._cstypes import List as CsList
 from stock_indicators._cstypes import Decimal as CsDecimal
 from stock_indicators._cstypes import to_pydecimal
 from stock_indicators.indicators.common.enums import EndType
+from stock_indicators.indicators.common.helpers import CondenseMixin
 from stock_indicators.indicators.common.results import IndicatorResults, ResultBase
 from stock_indicators.indicators.common.quote import Quote
 
 
 @overload
 def get_fractal(quotes: Iterable[Quote], window_span: int = 2, end_type = EndType.HIGH_LOW) -> "FractalResults[FractalResult]": ...
 @overload
@@ -72,13 +73,13 @@
 
     @fractal_bull.setter
     def fractal_bull(self, value):
         self._csdata.FractalBull = CsDecimal(value)
 
 
 _T = TypeVar("_T", bound=FractalResult)
-class FractalResults(IndicatorResults[_T]):
+class FractalResults(CondenseMixin, IndicatorResults[_T]):
     """
     A wrapper class for the list of Williams Fractal results.
     It is exactly same with built-in `list` except for that it provides
     some useful helper methods written in C# implementation.
     """
```

### Comparing `stock-indicators-1.2.1/stock_indicators/indicators/gator.py` & `stock_indicators-1.3.0/stock_indicators/indicators/gator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import Iterable, Optional, TypeVar, overload
 
 from stock_indicators._cslib import CsIndicator
 from stock_indicators._cstypes import List as CsList
 from stock_indicators.indicators.alligator import AlligatorResult
-from stock_indicators.indicators.common.helpers import RemoveWarmupMixin
+from stock_indicators.indicators.common.helpers import CondenseMixin, RemoveWarmupMixin
 from stock_indicators.indicators.common.results import IndicatorResults, ResultBase
 from stock_indicators.indicators.common.quote import Quote
 
 @overload
 def get_gator(quotes: Iterable[Quote]) -> "GatorResults[GatorResult]": ...
 @overload
 def get_gator(quotes: Iterable[AlligatorResult]) -> "GatorResults[GatorResult]": ...
@@ -28,16 +28,15 @@
          - [Gator Oscillator Reference](https://python.stockindicators.dev/indicators/Gator/#content)
          - [Helper Methods](https://python.stockindicators.dev/utilities/#content)
     """
     if not quotes or isinstance(quotes[0], Quote):
         results = CsIndicator.GetGator[Quote](CsList(Quote, quotes))
     else:
         # Get C# objects.
-        if isinstance(quotes, IndicatorResults):
-            quotes.reload()
+        if isinstance(quotes, IndicatorResults) and quotes._csdata is not None:
             cs_results = quotes._csdata
         else:
             cs_results = [ q._csdata for q in quotes ]
 
         results = CsIndicator.GetGator(CsList(type(cs_results[0]), cs_results))
     return GatorResults(results, GatorResult)
 
@@ -77,13 +76,13 @@
 
     @is_lower_expanding.setter
     def is_lower_expanding(self, value):
         self._csdata.LowerIsExpanding = value
 
 
 _T = TypeVar("_T", bound=GatorResult)
-class GatorResults(RemoveWarmupMixin, IndicatorResults[_T]):
+class GatorResults(CondenseMixin, RemoveWarmupMixin, IndicatorResults[_T]):
     """
     A wrapper class for the list of Gator Oscillator results.
     It is exactly same with built-in `list` except for that it provides
     some useful helper methods written in C# implementation.
     """
```

### Comparing `stock-indicators-1.2.1/stock_indicators/indicators/heikin_ashi.py` & `stock_indicators-1.3.0/stock_indicators/indicators/heikin_ashi.py`

 * *Files identical despite different names*

### Comparing `stock-indicators-1.2.1/stock_indicators/indicators/hma.py` & `stock_indicators-1.3.0/stock_indicators/indicators/hma.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Iterable, Optional, TypeVar
 
 from stock_indicators._cslib import CsIndicator
 from stock_indicators._cstypes import List as CsList
-from stock_indicators.indicators.common.helpers import RemoveWarmupMixin
+from stock_indicators.indicators.common.helpers import CondenseMixin, RemoveWarmupMixin
 from stock_indicators.indicators.common.results import IndicatorResults, ResultBase
 from stock_indicators.indicators.common.quote import Quote
 
 
 def get_hma(quotes: Iterable[Quote], lookback_periods: int):
     """Get HMA calculated.
 
@@ -43,13 +43,13 @@
 
     @hma.setter
     def hma(self, value):
         self._csdata.Hma = value
 
 
 _T = TypeVar("_T", bound=HMAResult)
-class HMAResults(RemoveWarmupMixin, IndicatorResults[_T]):
+class HMAResults(CondenseMixin, RemoveWarmupMixin, IndicatorResults[_T]):
     """
     A wrapper class for the list of Hull Moving Average (HMA) results.
     It is exactly same with built-in `list` except for that it provides
     some useful helper methods written in CSharp implementation.
     """
```

### Comparing `stock-indicators-1.2.1/stock_indicators/indicators/ht_trendline.py` & `stock_indicators-1.3.0/stock_indicators/indicators/ht_trendline.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Iterable, Optional, TypeVar
 
 from stock_indicators._cslib import CsIndicator
 from stock_indicators._cstypes import List as CsList
-from stock_indicators.indicators.common.helpers import RemoveWarmupMixin
+from stock_indicators.indicators.common.helpers import CondenseMixin, RemoveWarmupMixin
 from stock_indicators.indicators.common.results import IndicatorResults, ResultBase
 from stock_indicators.indicators.common.quote import Quote
 
 
 def get_ht_trendline(quotes: Iterable[Quote]):
     """Get HTL calculated.
 
@@ -56,13 +56,13 @@
 
     @smooth_price.setter
     def smooth_price(self, value):
         self._csdata.SmoothPrice = value
 
 
 _T = TypeVar("_T", bound=HTTrendlineResult)
-class HTTrendlineResults(RemoveWarmupMixin, IndicatorResults[_T]):
+class HTTrendlineResults(CondenseMixin, RemoveWarmupMixin, IndicatorResults[_T]):
     """
     A wrapper class for the list of Hilbert Transform Instantaneous Trendline (HTL) results.
     It is exactly same with built-in `list` except for that it provides
     some useful helper methods written in CSharp implementation.
     """
```

### Comparing `stock-indicators-1.2.1/stock_indicators/indicators/hurst.py` & `stock_indicators-1.3.0/stock_indicators/indicators/hurst.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Iterable, Optional, TypeVar
 
 from stock_indicators._cslib import CsIndicator
 from stock_indicators._cstypes import List as CsList
-from stock_indicators.indicators.common.helpers import RemoveWarmupMixin
+from stock_indicators.indicators.common.helpers import CondenseMixin, RemoveWarmupMixin
 from stock_indicators.indicators.common.results import IndicatorResults, ResultBase
 from stock_indicators.indicators.common.quote import Quote
 
 
 def get_hurst(quotes: Iterable[Quote], lookback_periods: int = 100):
     """Get Hurst Exponent calculated.
 
@@ -43,13 +43,13 @@
 
     @hurst_exponent.setter
     def hurst_exponent(self, value):
         self._csdata.HurstExponent = value
 
 
 _T = TypeVar("_T", bound=HurstResult)
-class HurstResults(RemoveWarmupMixin, IndicatorResults[_T]):
+class HurstResults(CondenseMixin, RemoveWarmupMixin, IndicatorResults[_T]):
     """
     A wrapper class for the list of Hurst Exponent results.
     It is exactly same with built-in `list` except for that it provides
     some useful helper methods written in CSharp implementation.
     """
```

### Comparing `stock-indicators-1.2.1/stock_indicators/indicators/ichimoku.py` & `stock_indicators-1.3.0/stock_indicators/indicators/ichimoku.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from decimal import Decimal
 from typing import Iterable, Optional, TypeVar, overload
 
 from stock_indicators._cslib import CsIndicator
 from stock_indicators._cstypes import List as CsList
 from stock_indicators._cstypes import Decimal as CsDecimal
 from stock_indicators._cstypes import to_pydecimal
+from stock_indicators.indicators.common.helpers import CondenseMixin
 from stock_indicators.indicators.common.results import IndicatorResults, ResultBase
 from stock_indicators.indicators.common.quote import Quote
 
 
 @overload
 def get_ichimoku(quotes: Iterable[Quote], tenkan_periods: int = 9,
                  kijun_periods: int = 26, senkou_b_periods: int = 52) -> "IchimokuResults[IchimokuResult]": ...
@@ -116,13 +117,13 @@
 
     @chikou_span.setter
     def chikou_span(self, value):
         self._csdata.ChikouSpan = CsDecimal(value)
 
 
 _T = TypeVar("_T", bound=IchimokuResult)
-class IchimokuResults(IndicatorResults[_T]):
+class IchimokuResults(CondenseMixin, IndicatorResults[_T]):
     """
     A wrapper class for the list of Ichimoku Cloud results.
     It is exactly same with built-in `list` except for that it provides
     some useful helper methods written in C# implementation.
     """
```

### Comparing `stock-indicators-1.2.1/stock_indicators/indicators/kama.py` & `stock_indicators-1.3.0/stock_indicators/indicators/kama.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from decimal import Decimal
 from typing import Iterable, Optional, TypeVar
 
 from stock_indicators._cslib import CsIndicator
 from stock_indicators._cstypes import List as CsList
 from stock_indicators._cstypes import Decimal as CsDecimal
 from stock_indicators._cstypes import to_pydecimal
-from stock_indicators.indicators.common.helpers import RemoveWarmupMixin
+from stock_indicators.indicators.common.helpers import CondenseMixin, RemoveWarmupMixin
 from stock_indicators.indicators.common.results import IndicatorResults, ResultBase
 from stock_indicators.indicators.common.quote import Quote
 
 
 def get_kama(quotes: Iterable[Quote], er_periods: int = 10,
              fast_periods: int = 2, slow_periods: int = 30):
     """Get KAMA calculated.
@@ -62,13 +62,13 @@
 
     @kama.setter
     def kama(self, value):
         self._csdata.Kama = CsDecimal(value)
 
 
 _T = TypeVar("_T", bound=KAMAResult)
-class KAMAResults(RemoveWarmupMixin, IndicatorResults[_T]):
+class KAMAResults(CondenseMixin, RemoveWarmupMixin, IndicatorResults[_T]):
     """
     A wrapper class for the list of Kaufman’s Adaptive Moving Average (KAMA) results.
     It is exactly same with built-in `list` except for that it provides
     some useful helper methods written in CSharp implementation.
     """
```

### Comparing `stock-indicators-1.2.1/stock_indicators/indicators/keltner.py` & `stock_indicators-1.3.0/stock_indicators/indicators/keltner.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Iterable, Optional, TypeVar
 
 from stock_indicators._cslib import CsIndicator
 from stock_indicators._cstypes import List as CsList
-from stock_indicators.indicators.common.helpers import RemoveWarmupMixin
+from stock_indicators.indicators.common.helpers import CondenseMixin, RemoveWarmupMixin
 from stock_indicators.indicators.common.results import IndicatorResults, ResultBase
 from stock_indicators.indicators.common.quote import Quote
 
 
 def get_keltner(quotes: Iterable[Quote], ema_periods: int = 20,
                 multiplier: float = 2, atr_periods: int = 10):
     """Get Keltner Channels calculated.
@@ -75,13 +75,13 @@
 
     @width.setter
     def width(self, value):
         self._csdata.Width = value
 
 
 _T = TypeVar("_T", bound=KeltnerResult)
-class KeltnerResults(RemoveWarmupMixin, IndicatorResults[_T]):
+class KeltnerResults(CondenseMixin, RemoveWarmupMixin, IndicatorResults[_T]):
     """
     A wrapper class for the list of Keltner Channels results.
     It is exactly same with built-in `list` except for that it provides
     some useful helper methods written in CSharp implementation.
     """
```

### Comparing `stock-indicators-1.2.1/stock_indicators/indicators/kvo.py` & `stock_indicators-1.3.0/stock_indicators/indicators/kvo.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Iterable, Optional, TypeVar
 
 from stock_indicators._cslib import CsIndicator
 from stock_indicators._cstypes import List as CsList
-from stock_indicators.indicators.common.helpers import RemoveWarmupMixin
+from stock_indicators.indicators.common.helpers import CondenseMixin, RemoveWarmupMixin
 from stock_indicators.indicators.common.results import IndicatorResults, ResultBase
 from stock_indicators.indicators.common.quote import Quote
 
 
 def get_kvo(quotes: Iterable[Quote], fast_periods: int = 34,
             slow_periods: int = 55, signal_periods: int = 13):
     """Get KVO calculated.
@@ -59,13 +59,13 @@
 
     @signal.setter
     def signal(self, value):
         self._csdata.Signal = value
 
 
 _T = TypeVar("_T", bound=KVOResult)
-class KVOResults(RemoveWarmupMixin, IndicatorResults[_T]):
+class KVOResults(CondenseMixin, RemoveWarmupMixin, IndicatorResults[_T]):
     """
     A wrapper class for the list of Klinger Volume Oscillator (KVO) results.
     It is exactly same with built-in `list` except for that it provides
     some useful helper methods written in CSharp implementation.
     """
```

### Comparing `stock-indicators-1.2.1/stock_indicators/indicators/ma_envelopes.py` & `stock_indicators-1.3.0/stock_indicators/indicators/ma_envelopes.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from typing import Iterable, Optional, TypeVar
 
 from stock_indicators._cslib import CsIndicator
 from stock_indicators._cstypes import List as CsList
 from stock_indicators.indicators.common.enums import MAType
+from stock_indicators.indicators.common.helpers import CondenseMixin
 from stock_indicators.indicators.common.results import IndicatorResults, ResultBase
 from stock_indicators.indicators.common.quote import Quote
 
 
 def get_ma_envelopes(quotes: Iterable[Quote], lookback_periods: int,
                 percent_offset: float = 2.5, ma_type: MAType = MAType.SMA):
     """Get Moving Average Envelopes calculated.
@@ -67,13 +68,13 @@
 
     @lower_envelope.setter
     def lower_envelope(self, value):
         self._csdata.LowerEnvelope = value
 
 
 _T = TypeVar("_T", bound=MAEnvelopeResult)
-class MAEnvelopeResults(IndicatorResults[_T]):
+class MAEnvelopeResults(CondenseMixin, IndicatorResults[_T]):
     """
     A wrapper class for the list of Moving Average Envelopes results.
     It is exactly same with built-in `list` except for that it provides
     some useful helper methods written in CSharp implementation.
     """
```

### Comparing `stock-indicators-1.2.1/stock_indicators/indicators/macd.py` & `stock_indicators-1.3.0/stock_indicators/indicators/macd.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Iterable, Optional, TypeVar
 
 from stock_indicators._cslib import CsIndicator
 from stock_indicators.indicators.common.enums import CandlePart
-from stock_indicators.indicators.common.helpers import RemoveWarmupMixin
+from stock_indicators.indicators.common.helpers import CondenseMixin, RemoveWarmupMixin
 from stock_indicators.indicators.common.results import IndicatorResults, ResultBase
 from stock_indicators.indicators.common.quote import Quote
 
 
 def get_macd(quotes: Iterable[Quote], fast_periods: int = 12,
              slow_periods: int = 26, signal_periods: int = 9,
              candle_part: CandlePart = CandlePart.CLOSE):
@@ -88,13 +88,13 @@
 
     @slow_ema.setter
     def slow_ema(self, value):
         self._csdata.SlowEma = value
 
 
 _T = TypeVar("_T", bound=MACDResult)
-class MACDResults(RemoveWarmupMixin ,IndicatorResults[_T]):
+class MACDResults(CondenseMixin, RemoveWarmupMixin ,IndicatorResults[_T]):
     """
     A wrapper class for the list of MACD(Moving Average Convergence/Divergence) results.
     It is exactly same with built-in `list` except for that it provides
     some useful helper methods written in C# implementation.
     """
```

### Comparing `stock-indicators-1.2.1/stock_indicators/indicators/mama.py` & `stock_indicators-1.3.0/stock_indicators/indicators/mama.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Iterable, Optional, TypeVar
 
 from stock_indicators._cslib import CsIndicator
 from stock_indicators._cstypes import List as CsList
-from stock_indicators.indicators.common.helpers import RemoveWarmupMixin
+from stock_indicators.indicators.common.helpers import CondenseMixin, RemoveWarmupMixin
 from stock_indicators.indicators.common.results import IndicatorResults, ResultBase
 from stock_indicators.indicators.common.quote import Quote
 
 
 def get_mama(quotes: Iterable[Quote], fast_limit: float = 0.5,
              slow_limit: float = 0.05):
     """Get MAMA calculated.
@@ -56,13 +56,13 @@
 
     @fama.setter
     def fama(self, value):
         self._csdata.Fama = value
 
 
 _T = TypeVar("_T", bound=MAMAResult)
-class MAMAResults(RemoveWarmupMixin, IndicatorResults[_T]):
+class MAMAResults(CondenseMixin, RemoveWarmupMixin, IndicatorResults[_T]):
     """
     A wrapper class for the list of MESA Adaptive Moving Average (MAMA) results.
     It is exactly same with built-in `list` except for that it provides
     some useful helper methods written in CSharp implementation.
     """
```

### Comparing `stock-indicators-1.2.1/stock_indicators/indicators/marubozu.py` & `stock_indicators-1.3.0/stock_indicators/indicators/marubozu.py`

 * *Files identical despite different names*

### Comparing `stock-indicators-1.2.1/stock_indicators/indicators/mfi.py` & `stock_indicators-1.3.0/stock_indicators/indicators/mfi.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Iterable, Optional, TypeVar
 
 from stock_indicators._cslib import CsIndicator
 from stock_indicators._cstypes import List as CsList
-from stock_indicators.indicators.common.helpers import RemoveWarmupMixin
+from stock_indicators.indicators.common.helpers import CondenseMixin, RemoveWarmupMixin
 from stock_indicators.indicators.common.results import IndicatorResults, ResultBase
 from stock_indicators.indicators.common.quote import Quote
 
 
 def get_mfi(quotes: Iterable[Quote], lookback_periods: int = 14):
     """Get MFI calculated.
 
@@ -43,13 +43,13 @@
 
     @mfi.setter
     def mfi(self, value):
         self._csdata.Mfi = value
 
 
 _T = TypeVar("_T", bound=MFIResult)
-class MFIResults(RemoveWarmupMixin, IndicatorResults[_T]):
+class MFIResults(CondenseMixin, RemoveWarmupMixin, IndicatorResults[_T]):
     """
     A wrapper class for the list of Money Flow Index (MFI) results.
     It is exactly same with built-in `list` except for that it provides
     some useful helper methods written in CSharp implementation.
     """
```

### Comparing `stock-indicators-1.2.1/stock_indicators/indicators/obv.py` & `stock_indicators-1.3.0/stock_indicators/indicators/obv.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from typing import Iterable, Optional, TypeVar
 
 from stock_indicators._cslib import CsIndicator
 from stock_indicators._cstypes import List as CsList
+from stock_indicators.indicators.common.helpers import CondenseMixin
 from stock_indicators.indicators.common.results import IndicatorResults, ResultBase
 from stock_indicators.indicators.common.quote import Quote
 
 
 def get_obv(quotes: Iterable[Quote], sma_periods: Optional[int] = None):
     """Get OBV calculated.
 
@@ -50,13 +51,13 @@
 
     @obv_sma.setter
     def obv_sma(self, value):
         self._csdata.ObvSma = value
 
 
 _T = TypeVar("_T", bound=OBVResult)
-class OBVResults(IndicatorResults[_T]):
+class OBVResults(CondenseMixin, IndicatorResults[_T]):
     """
     A wrapper class for the list of On-balance Volume (OBV) results.
     It is exactly same with built-in `list` except for that it provides
     some useful helper methods written in CSharp implementation.
     """
```

### Comparing `stock-indicators-1.2.1/stock_indicators/indicators/parabolic_sar.py` & `stock_indicators-1.3.0/stock_indicators/indicators/parabolic_sar.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Iterable, Optional, TypeVar, overload
 
 from stock_indicators._cslib import CsIndicator
 from stock_indicators._cstypes import List as CsList
-from stock_indicators.indicators.common.helpers import RemoveWarmupMixin
+from stock_indicators.indicators.common.helpers import CondenseMixin, RemoveWarmupMixin
 from stock_indicators.indicators.common.results import IndicatorResults, ResultBase
 from stock_indicators.indicators.common.quote import Quote
 
 
 @overload
 def get_parabolic_sar(quotes: Iterable[Quote], acceleration_step: float = 0.02,
                       max_acceleration_factor: float = 0.2) -> "ParabolicSARResults[ParabolicSARResult]": ...
@@ -72,13 +72,13 @@
 
     @is_reversal.setter
     def is_reversal(self, value):
         self._csdata.IsReversal = value
 
 
 _T = TypeVar("_T", bound=ParabolicSARResult)
-class ParabolicSARResults(RemoveWarmupMixin, IndicatorResults[_T]):
+class ParabolicSARResults(CondenseMixin, RemoveWarmupMixin, IndicatorResults[_T]):
     """
     A wrapper class for the list of Parabolic SAR(stop and reverse) results.
     It is exactly same with built-in `list` except for that it provides
     some useful helper methods written in C# implementation.
     """
```

### Comparing `stock-indicators-1.2.1/stock_indicators/indicators/pivot_points.py` & `stock_indicators-1.3.0/stock_indicators/indicators/pivot_points.py`

 * *Files identical despite different names*

### Comparing `stock-indicators-1.2.1/stock_indicators/indicators/pivots.py` & `stock_indicators-1.3.0/stock_indicators/indicators/pivots.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from typing import Iterable, Optional, TypeVar
 
 from stock_indicators._cslib import CsIndicator
 from stock_indicators._cstypes import List as CsList
 from stock_indicators._cstypes import Decimal as CsDecimal
 from stock_indicators._cstypes import to_pydecimal
 from stock_indicators.indicators.common.enums import EndType, PivotTrend
+from stock_indicators.indicators.common.helpers import CondenseMixin
 from stock_indicators.indicators.common.results import IndicatorResults, ResultBase
 from stock_indicators.indicators.common.quote import Quote
 
 
 def get_pivots(quotes: Iterable[Quote], left_span: int = 2,
                right_span: int = 2, max_trend_periods: int = 20,
                end_type: EndType = EndType.HIGH_LOW):
@@ -104,13 +105,13 @@
 
     @low_trend.setter
     def low_trend(self, value):
         self._csdata.LowTrend = value.cs_value
 
 
 _T = TypeVar("_T", bound=PivotsResult)
-class PivotsResults(IndicatorResults[_T]):
+class PivotsResults(CondenseMixin, IndicatorResults[_T]):
     """
     A wrapper class for the list of Pivots results.
     It is exactly same with built-in `list` except for that it provides
     some useful helper methods written in CSharp implementation.
     """
```

### Comparing `stock-indicators-1.2.1/stock_indicators/indicators/pmo.py` & `stock_indicators-1.3.0/stock_indicators/indicators/pmo.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Iterable, Optional, TypeVar
 
 from stock_indicators._cslib import CsIndicator
 from stock_indicators._cstypes import List as CsList
-from stock_indicators.indicators.common.helpers import RemoveWarmupMixin
+from stock_indicators.indicators.common.helpers import CondenseMixin, RemoveWarmupMixin
 from stock_indicators.indicators.common.results import IndicatorResults, ResultBase
 from stock_indicators.indicators.common.quote import Quote
 
 
 def get_pmo(quotes: Iterable[Quote], time_periods: int = 35,
             smooth_periods: int = 20, signal_periods: int = 10):
     """Get PMO calculated.
@@ -59,13 +59,13 @@
 
     @signal.setter
     def signal(self, value):
         self._csdata.Signal = value
 
 
 _T = TypeVar("_T", bound=PMOResult)
-class PMOResults(RemoveWarmupMixin, IndicatorResults[_T]):
+class PMOResults(CondenseMixin, RemoveWarmupMixin, IndicatorResults[_T]):
     """
     A wrapper class for the list of Price Momentum Oscillator (PMO) results.
     It is exactly same with built-in `list` except for that it provides
     some useful helper methods written in CSharp implementation.
     """
```

### Comparing `stock-indicators-1.2.1/stock_indicators/indicators/prs.py` & `stock_indicators-1.3.0/stock_indicators/indicators/prs.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from typing import Iterable, Optional, TypeVar
 
 from stock_indicators._cslib import CsIndicator
 from stock_indicators._cstypes import List as CsList
+from stock_indicators.indicators.common.helpers import CondenseMixin
 from stock_indicators.indicators.common.results import IndicatorResults, ResultBase
 from stock_indicators.indicators.common.quote import Quote
 
 
 def get_prs(eval_quotes: Iterable[Quote], base_quotes: Iterable[Quote],
             lookback_periods: Optional[int] = None, sma_periods: Optional[int] = None):
     """Get PRS calculated.
@@ -73,13 +74,13 @@
     def prs_percent(self, value):
         self._csdata.PrsPercent = value
 
 
 _T = TypeVar("_T", bound=PRSResult)
 
 
-class PRSResults(IndicatorResults[_T]):
+class PRSResults(CondenseMixin, IndicatorResults[_T]):
     """
     A wrapper class for the list of Price Relative Strength (PRS) results.
     It is exactly same with built-in `list` except for that it provides
     some useful helper methods written in CSharp implementation.
     """
```

### Comparing `stock-indicators-1.2.1/stock_indicators/indicators/pvo.py` & `stock_indicators-1.3.0/stock_indicators/indicators/pvo.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Iterable, Optional, TypeVar
 
 from stock_indicators._cslib import CsIndicator
 from stock_indicators._cstypes import List as CsList
-from stock_indicators.indicators.common.helpers import RemoveWarmupMixin
+from stock_indicators.indicators.common.helpers import CondenseMixin, RemoveWarmupMixin
 from stock_indicators.indicators.common.results import IndicatorResults, ResultBase
 from stock_indicators.indicators.common.quote import Quote
 
 
 def get_pvo(quotes: Iterable[Quote], fast_periods: int = 12,
                slow_periods: int = 26, signal_periods: int = 9):
     """Get PVO calculated.
@@ -67,13 +67,13 @@
 
     @histogram.setter
     def histogram(self, value):
         self._csdata.Histogram = value
 
 
 _T = TypeVar("_T", bound=PVOResult)
-class PVOResults(RemoveWarmupMixin, IndicatorResults[_T]):
+class PVOResults(CondenseMixin, RemoveWarmupMixin, IndicatorResults[_T]):
     """
     A wrapper class for the list of Percentage Volume Oscillator (PVO) results.
     It is exactly same with built-in `list` except for that it provides
     some useful helper methods written in CSharp implementation.
     """
```

### Comparing `stock-indicators-1.2.1/stock_indicators/indicators/renko.py` & `stock_indicators-1.3.0/stock_indicators/indicators/renko.py`

 * *Files identical despite different names*

### Comparing `stock-indicators-1.2.1/stock_indicators/indicators/roc.py` & `stock_indicators-1.3.0/stock_indicators/indicators/roc.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Iterable, Optional, TypeVar
 
 from stock_indicators._cslib import CsIndicator
 from stock_indicators._cstypes import List as CsList
-from stock_indicators.indicators.common.helpers import RemoveWarmupMixin
+from stock_indicators.indicators.common.helpers import CondenseMixin, RemoveWarmupMixin
 from stock_indicators.indicators.common.results import IndicatorResults, ResultBase
 from stock_indicators.indicators.common.quote import Quote
 
 
 def get_roc(quotes: Iterable[Quote], lookback_periods: int, sma_periods: int = None):
     """Get ROC calculated.
 
@@ -92,15 +92,15 @@
 
     @roc_sma.setter
     def roc_sma(self, value):
         self._csdata.RocSma = value
 
 
 _T = TypeVar("_T", bound=ROCResult)
-class ROCResults(RemoveWarmupMixin, IndicatorResults[_T]):
+class ROCResults(CondenseMixin, RemoveWarmupMixin, IndicatorResults[_T]):
     """
     A wrapper class for the list of ROC(Rate of Change) results.
     It is exactly same with built-in `list` except for that it provides
     some useful helper methods written in C# implementation.
     """
 
 
@@ -139,13 +139,13 @@
 
     @lower_band.setter
     def lower_band(self, value):
         self._csdata.LowerBand = value
 
 
 _T = TypeVar("_T", bound=ROCWBResult)
-class ROCWBResults(RemoveWarmupMixin, IndicatorResults[_T]):
+class ROCWBResults(CondenseMixin, RemoveWarmupMixin, IndicatorResults[_T]):
     """
     A wrapper class for the list of ROC(Rate of Change) with band results.
     It is exactly same with built-in `list` except for that it provides
     some useful helper methods written in C# implementation.
     """
```

### Comparing `stock-indicators-1.2.1/stock_indicators/indicators/rolling_pivots.py` & `stock_indicators-1.3.0/stock_indicators/indicators/rolling_pivots.py`

 * *Files identical despite different names*

### Comparing `stock-indicators-1.2.1/stock_indicators/indicators/rsi.py` & `stock_indicators-1.3.0/stock_indicators/indicators/rsi.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Iterable, Optional, TypeVar
 
 from stock_indicators._cslib import CsIndicator
 from stock_indicators._cstypes import List as CsList
-from stock_indicators.indicators.common.helpers import RemoveWarmupMixin
+from stock_indicators.indicators.common.helpers import CondenseMixin, RemoveWarmupMixin
 from stock_indicators.indicators.common.results import IndicatorResults, ResultBase
 from stock_indicators.indicators.common.quote import Quote
 
 
 def get_rsi(quotes: Iterable[Quote], lookback_periods: int = 14):
     """Get RSI calculated.
 
@@ -43,13 +43,13 @@
 
     @rsi.setter
     def rsi(self, value):
         self._csdata.Rsi = value
 
 
 _T = TypeVar("_T", bound=RSIResult)
-class RSIResults(RemoveWarmupMixin, IndicatorResults[_T]):
+class RSIResults(CondenseMixin, RemoveWarmupMixin, IndicatorResults[_T]):
     """
     A wrapper class for the list of RSI(Relative Strength Index) results.
     It is exactly same with built-in `list` except for that it provides
     some useful helper methods written in CSharp implementation.
     """
```

### Comparing `stock-indicators-1.2.1/stock_indicators/indicators/slope.py` & `stock_indicators-1.3.0/stock_indicators/indicators/slope.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from decimal import Decimal
 from typing import Iterable, Optional, TypeVar
 
 from stock_indicators._cslib import CsIndicator
 from stock_indicators._cstypes import List as CsList
 from stock_indicators._cstypes import Decimal as CsDecimal
 from stock_indicators._cstypes import to_pydecimal
-from stock_indicators.indicators.common.helpers import RemoveWarmupMixin
+from stock_indicators.indicators.common.helpers import CondenseMixin, RemoveWarmupMixin
 from stock_indicators.indicators.common.results import IndicatorResults, ResultBase
 from stock_indicators.indicators.common.quote import Quote
 
 
 def get_slope(quotes: Iterable[Quote], lookback_periods: int):
     """Get Slope calculated.
 
@@ -77,13 +77,13 @@
         return to_pydecimal(self._csdata.Line)
 
     @line.setter
     def line(self, value):
         self._csdata.Line = CsDecimal(value)
 
 _T = TypeVar("_T", bound=SlopeResult)
-class SlopeResults(RemoveWarmupMixin, IndicatorResults[_T]):
+class SlopeResults(CondenseMixin, RemoveWarmupMixin, IndicatorResults[_T]):
     """
     A wrapper class for the list of Slope results.
     It is exactly same with built-in `list` except for that it provides
     some useful helper methods written in C# implementation.
     """
```

### Comparing `stock-indicators-1.2.1/stock_indicators/indicators/sma.py` & `stock_indicators-1.3.0/stock_indicators/indicators/sma.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import Iterable, Optional, TypeVar
 
 from stock_indicators._cslib import CsIndicator
 from stock_indicators._cstypes import List as CsList
 from stock_indicators.indicators.common.enums import CandlePart
-from stock_indicators.indicators.common.helpers import RemoveWarmupMixin
+from stock_indicators.indicators.common.helpers import CondenseMixin, RemoveWarmupMixin
 from stock_indicators.indicators.common.results import IndicatorResults, ResultBase
 from stock_indicators.indicators.common.quote import Quote
 
 
 def get_sma(quotes: Iterable[Quote], lookback_periods: int,
             candle_part: CandlePart = CandlePart.CLOSE):
     """Get SMA calculated.
@@ -76,17 +76,15 @@
 
     @sma.setter
     def sma(self, value):
         self._csdata.Sma = value
 
 
 _T = TypeVar("_T", bound=SMAResult)
-
-
-class SMAResults(RemoveWarmupMixin, IndicatorResults[_T]):
+class SMAResults(CondenseMixin, RemoveWarmupMixin, IndicatorResults[_T]):
     """
     A wrapper class for the list of SMA(Simple Moving Average) results.
     It is exactly same with built-in `list` except for that it provides
     some useful helper methods written in CSharp implementation.
     """
 
 
@@ -117,15 +115,13 @@
 
     @mape.setter
     def mape(self, value):
         self._csdata.Mape = value
 
 
 _T = TypeVar("_T", bound=SMAAnalysisResult)
-
-
-class SMAAnalysisResults(RemoveWarmupMixin, IndicatorResults[_T]):
+class SMAAnalysisResults(CondenseMixin, RemoveWarmupMixin, IndicatorResults[_T]):
     """
     A wrapper class for the list of SMA Analysis results.
     It is exactly same with built-in `list` except for that it provides
     some useful helper methods written in CSharp implementation.
     """
```

### Comparing `stock-indicators-1.2.1/stock_indicators/indicators/smi.py` & `stock_indicators-1.3.0/stock_indicators/indicators/smi.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Iterable, Optional, TypeVar
 
 from stock_indicators._cslib import CsIndicator
 from stock_indicators._cstypes import List as CsList
-from stock_indicators.indicators.common.helpers import RemoveWarmupMixin
+from stock_indicators.indicators.common.helpers import CondenseMixin, RemoveWarmupMixin
 from stock_indicators.indicators.common.results import IndicatorResults, ResultBase
 from stock_indicators.indicators.common.quote import Quote
 
 
 def get_smi(quotes: Iterable[Quote], lookback_periods: int = 13,
             first_smooth_periods: int = 25, second_smooth_periods: int = 2,
             signal_periods: int = 3):
@@ -64,13 +64,13 @@
 
     @signal.setter
     def signal(self, value):
         self._csdata.Signal = value
 
 
 _T = TypeVar("_T", bound=SMIResult)
-class SMIResults(RemoveWarmupMixin, IndicatorResults[_T]):
+class SMIResults(CondenseMixin, RemoveWarmupMixin, IndicatorResults[_T]):
     """
     A wrapper class for the list of Stochastic Momentum Index (SMI) results.
     It is exactly same with built-in `list` except for that it provides
     some useful helper methods written in CSharp implementation.
     """
```

### Comparing `stock-indicators-1.2.1/stock_indicators/indicators/smma.py` & `stock_indicators-1.3.0/stock_indicators/indicators/smma.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Iterable, Optional, TypeVar
 
 from stock_indicators._cslib import CsIndicator
 from stock_indicators._cstypes import List as CsList
-from stock_indicators.indicators.common.helpers import RemoveWarmupMixin
+from stock_indicators.indicators.common.helpers import CondenseMixin, RemoveWarmupMixin
 from stock_indicators.indicators.common.results import IndicatorResults, ResultBase
 from stock_indicators.indicators.common.quote import Quote
 
 
 def get_smma(quotes: Iterable[Quote], lookback_periods: int):
     """Get SMMA calculated.
 
@@ -43,13 +43,13 @@
 
     @smma.setter
     def smma(self, value):
         self._csdata.Smma = value
 
 
 _T = TypeVar("_T", bound=SMMAResult)
-class SMMAResults(RemoveWarmupMixin, IndicatorResults[_T]):
+class SMMAResults(CondenseMixin, RemoveWarmupMixin, IndicatorResults[_T]):
     """
     A wrapper class for the list of Smoothed Moving Average (SMMA) results.
     It is exactly same with built-in `list` except for that it provides
     some useful helper methods written in CSharp implementation.
     """
```

### Comparing `stock-indicators-1.2.1/stock_indicators/indicators/starc_bands.py` & `stock_indicators-1.3.0/stock_indicators/indicators/starc_bands.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import Iterable, Optional, TypeVar
 from warnings import warn
 
 from stock_indicators._cslib import CsIndicator
 from stock_indicators._cstypes import List as CsList
-from stock_indicators.indicators.common.helpers import RemoveWarmupMixin
+from stock_indicators.indicators.common.helpers import CondenseMixin, RemoveWarmupMixin
 from stock_indicators.indicators.common.results import IndicatorResults, ResultBase
 from stock_indicators.indicators.common.quote import Quote
 
 
 def get_starc_bands(quotes: Iterable[Quote], sma_periods: int = None,
             multiplier: float = 2, atr_periods: int = 10):
     """Get STARC Bands calculated.
@@ -72,13 +72,13 @@
 
     @lower_band.setter
     def lower_band(self, value):
         self._csdata.LowerBand = value
 
 
 _T = TypeVar("_T", bound=STARCBandsResult)
-class STARCBandsResults(RemoveWarmupMixin, IndicatorResults[_T]):
+class STARCBandsResults(CondenseMixin, RemoveWarmupMixin, IndicatorResults[_T]):
     """
     A wrapper class for the list of Stoller Average Range Channel (STARC) Bands results.
     It is exactly same with built-in `list` except for that it provides
     some useful helper methods written in CSharp implementation.
     """
```

### Comparing `stock-indicators-1.2.1/stock_indicators/indicators/stc.py` & `stock_indicators-1.3.0/stock_indicators/indicators/stc.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Iterable, Optional, TypeVar
 
 from stock_indicators._cslib import CsIndicator
 from stock_indicators._cstypes import List as CsList
-from stock_indicators.indicators.common.helpers import RemoveWarmupMixin
+from stock_indicators.indicators.common.helpers import CondenseMixin, RemoveWarmupMixin
 from stock_indicators.indicators.common.results import IndicatorResults, ResultBase
 from stock_indicators.indicators.common.quote import Quote
 
 
 def get_stc(quotes: Iterable[Quote], cycle_periods: int = 10,
             fast_periods: int = 23, slow_periods: int = 50):
     """Get STC calculated.
@@ -51,13 +51,13 @@
 
     @stc.setter
     def stc(self, value):
         self._csdata.Stc = value
 
 
 _T = TypeVar("_T", bound=STCResult)
-class STCResults(RemoveWarmupMixin, IndicatorResults[_T]):
+class STCResults(CondenseMixin, RemoveWarmupMixin, IndicatorResults[_T]):
     """
     A wrapper class for the list of Schaff Trend Cycle (STC) results.
     It is exactly same with built-in `list` except for that it provides
     some useful helper methods written in CSharp implementation.
     """
```

### Comparing `stock-indicators-1.2.1/stock_indicators/indicators/stdev.py` & `stock_indicators-1.3.0/stock_indicators/indicators/stdev.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Iterable, Optional, TypeVar
 
 from stock_indicators._cslib import CsIndicator
 from stock_indicators._cstypes import List as CsList
-from stock_indicators.indicators.common.helpers import RemoveWarmupMixin
+from stock_indicators.indicators.common.helpers import CondenseMixin, RemoveWarmupMixin
 from stock_indicators.indicators.common.results import IndicatorResults, ResultBase
 from stock_indicators.indicators.common.quote import Quote
 
 
 def get_stdev(quotes: Iterable[Quote], lookback_periods: int,
               sma_periods: Optional[int] = None):
     """Get Rolling Standard Deviation calculated.
@@ -70,13 +70,13 @@
 
     @stdev_sma.setter
     def stdev_sma(self, value):
         self._csdata.StdDevSma = value
 
 
 _T = TypeVar("_T", bound=StdevResult)
-class StdevResults(RemoveWarmupMixin, IndicatorResults[_T]):
+class StdevResults(CondenseMixin, RemoveWarmupMixin, IndicatorResults[_T]):
     """
     A wrapper class for the list of Rolling Standard Deviation results.
     It is exactly same with built-in `list` except for that it provides
     some useful helper methods written in C# implementation.
     """
```

### Comparing `stock-indicators-1.2.1/stock_indicators/indicators/stdev_channels.py` & `stock_indicators-1.3.0/stock_indicators/indicators/stdev_channels.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Iterable, Optional, TypeVar
 
 from stock_indicators._cslib import CsIndicator
 from stock_indicators._cstypes import List as CsList
-from stock_indicators.indicators.common.helpers import RemoveWarmupMixin
+from stock_indicators.indicators.common.helpers import CondenseMixin, RemoveWarmupMixin
 from stock_indicators.indicators.common.results import IndicatorResults, ResultBase
 from stock_indicators.indicators.common.quote import Quote
 
 
 def get_stdev_channels(quotes: Iterable[Quote],
                        lookback_periods: Optional[int] = 20,
                        standard_deviations: float = 2):
@@ -72,13 +72,13 @@
 
     @break_point.setter
     def break_point(self, value):
         self._csdata.BreakPoint = value
 
 
 _T = TypeVar("_T", bound=StdevChannelsResult)
-class StdevChannelsResults(RemoveWarmupMixin, IndicatorResults[_T]):
+class StdevChannelsResults(CondenseMixin, RemoveWarmupMixin, IndicatorResults[_T]):
     """
     A wrapper class for the list of Standard Deviation Channels results.
     It is exactly same with built-in `list` except for that it provides
     some useful helper methods written in CSharp implementation.
     """
```

### Comparing `stock-indicators-1.2.1/stock_indicators/indicators/stoch.py` & `stock_indicators-1.3.0/stock_indicators/indicators/stoch.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 from typing import Iterable, Optional, TypeVar
 
 from stock_indicators._cslib import CsIndicator
 from stock_indicators._cstypes import List as CsList
-from stock_indicators.indicators.common.helpers import RemoveWarmupMixin
+from stock_indicators.indicators.common.enums import MAType
+from stock_indicators.indicators.common.helpers import CondenseMixin, RemoveWarmupMixin
 from stock_indicators.indicators.common.results import IndicatorResults, ResultBase
 from stock_indicators.indicators.common.quote import Quote
 
 
-def get_stoch(quotes: Iterable[Quote], lookback_periods: int = 14, signal_periods: int = 3, smooth_periods: int = 3):
+def get_stoch(quotes: Iterable[Quote], lookback_periods: int = 14, signal_periods: int = 3, smooth_periods: int = 3,
+              k_factor: float = 3, d_factor: float = 2, ma_type: MAType = MAType.SMA):
     """Get Stochastic Oscillator calculated, with KDJ indexes.
 
     Stochastic Oscillatoris a momentum indicator that looks back N periods to produce a scale of 0 to 100.
     %J is also included for the KDJ Index extension.
 
     Parameters:
         `quotes` : Iterable[Quote]
@@ -23,23 +25,34 @@
         `signal_periods` : int, defaults 3
             Smoothing period for the %D signal line.
 
         `smooth_periods` : int, defaults 3
             Smoothing period for the %K Oscillator.
             Use 3 for Slow or 1 for Fast.
 
+        `k_factor` : float, defaults 3
+            Weight of %K in the %J calculation.
+
+        `d_factor` : float, defaults 2
+            Weight of %K in the %J calculation.
+
+        `ma_type` : MAType, defaults MAType.SMA
+            Type of moving average to use.
+            See docs for instructions and options.
+
     Returns:
         `StochResults[StochResult]`
             StochResults is list of StochResult with providing useful helper methods.
 
     See more:
          - [Stochastic Oscillator Reference](https://python.stockindicators.dev/indicators/Stoch/#content)
          - [Helper Methods](https://python.stockindicators.dev/utilities/#content)
     """
-    stoch_results = CsIndicator.GetStoch[Quote](CsList(Quote, quotes), lookback_periods, signal_periods, smooth_periods)
+    stoch_results = CsIndicator.GetStoch[Quote](CsList(Quote, quotes), lookback_periods, signal_periods, smooth_periods,
+                                                    k_factor, d_factor, ma_type.cs_value)
     return StochResults(stoch_results, StochResult)
 
 
 class StochResult(ResultBase):
     """
     A wrapper class for a single unit of Stochastic Oscillator(with KDJ Index) results.
     """
@@ -70,13 +83,13 @@
 
     k = oscillator
     d = signal
     j = percent_j
 
 
 _T = TypeVar("_T", bound=StochResult)
-class StochResults(RemoveWarmupMixin, IndicatorResults[_T]):
+class StochResults(CondenseMixin, RemoveWarmupMixin, IndicatorResults[_T]):
     """
     A wrapper class for the list of Stochastic Oscillator(with KDJ Index) results.
     It is exactly same with built-in `list` except for that it provides
     some useful helper methods written in C# implementation.
     """
```

### Comparing `stock-indicators-1.2.1/stock_indicators/indicators/stoch_rsi.py` & `stock_indicators-1.3.0/stock_indicators/indicators/stoch_rsi.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Iterable, Optional, TypeVar
 
 from stock_indicators._cslib import CsIndicator
 from stock_indicators._cstypes import List as CsList
-from stock_indicators.indicators.common.helpers import RemoveWarmupMixin
+from stock_indicators.indicators.common.helpers import CondenseMixin, RemoveWarmupMixin
 from stock_indicators.indicators.common.results import IndicatorResults, ResultBase
 from stock_indicators.indicators.common.quote import Quote
 
 
 def get_stoch_rsi(quotes: Iterable[Quote], rsi_periods: int, stoch_periods: int, signal_periods: int, smooth_periods: int = 1):
     """Get Stochastic RSI calculated.
 
@@ -59,13 +59,13 @@
 
     @signal.setter
     def signal(self, value):
         self._csdata.Signal = value
 
 
 _T = TypeVar("_T", bound=StochRSIResult)
-class StochRSIResults(RemoveWarmupMixin, IndicatorResults[_T]):
+class StochRSIResults(CondenseMixin, RemoveWarmupMixin, IndicatorResults[_T]):
     """
     A wrapper class for the list of Stochastic RSI results.
     It is exactly same with built-in `list` except for that it provides
     some useful helper methods written in C# implementation.
     """
```

### Comparing `stock-indicators-1.2.1/stock_indicators/indicators/super_trend.py` & `stock_indicators-1.3.0/stock_indicators/indicators/super_trend.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from decimal import Decimal
 from typing import Iterable, Optional, TypeVar
 
 from stock_indicators._cslib import CsIndicator
 from stock_indicators._cstypes import List as CsList
 from stock_indicators._cstypes import Decimal as CsDecimal
 from stock_indicators._cstypes import to_pydecimal
-from stock_indicators.indicators.common.helpers import RemoveWarmupMixin
+from stock_indicators.indicators.common.helpers import CondenseMixin, RemoveWarmupMixin
 from stock_indicators.indicators.common.results import IndicatorResults, ResultBase
 from stock_indicators.indicators.common.quote import Quote
 
 
 def get_super_trend(quotes: Iterable[Quote], lookback_periods: int = 10, multiplier: float = 3):
     """Get SuperTrend calculated.
 
@@ -66,13 +66,13 @@
 
     @lower_band.setter
     def lower_band(self, value):
         self._csdata.LowerBand = CsDecimal(value)
 
 
 _T = TypeVar("_T", bound=SuperTrendResult)
-class SuperTrendResults(RemoveWarmupMixin, IndicatorResults[_T]):
+class SuperTrendResults(CondenseMixin, RemoveWarmupMixin, IndicatorResults[_T]):
     """
     A wrapper class for the list of Super Trend results.
     It is exactly same with built-in `list` except for that it provides
     some useful helper methods written in C# implementation.
     """
```

### Comparing `stock-indicators-1.2.1/stock_indicators/indicators/t3.py` & `stock_indicators-1.3.0/stock_indicators/indicators/t3.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from typing import Iterable, Optional, TypeVar
 
 from stock_indicators._cslib import CsIndicator
 from stock_indicators._cstypes import List as CsList
+from stock_indicators.indicators.common.helpers import CondenseMixin
 from stock_indicators.indicators.common.results import IndicatorResults, ResultBase
 from stock_indicators.indicators.common.quote import Quote
 
 
 def get_t3(quotes: Iterable[Quote], lookback_periods: int = 5,
            volume_factor: float = 0.7):
     """Get T3 calculated.
@@ -47,13 +48,13 @@
 
     @t3.setter
     def t3(self, value):
         self._csdata.T3 = value
 
 
 _T = TypeVar("_T", bound=T3Result)
-class T3Results(IndicatorResults[_T]):
+class T3Results(CondenseMixin, IndicatorResults[_T]):
     """
     A wrapper class for the list of Tillson T3 results.
     It is exactly same with built-in `list` except for that it provides
     some useful helper methods written in CSharp implementation.
     """
```

### Comparing `stock-indicators-1.2.1/stock_indicators/indicators/tema.py` & `stock_indicators-1.3.0/stock_indicators/indicators/tema.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Iterable, Optional, TypeVar
 
 from stock_indicators._cslib import CsIndicator
 from stock_indicators._cstypes import List as CsList
-from stock_indicators.indicators.common.helpers import RemoveWarmupMixin
+from stock_indicators.indicators.common.helpers import CondenseMixin, RemoveWarmupMixin
 from stock_indicators.indicators.common.results import IndicatorResults, ResultBase
 from stock_indicators.indicators.common.quote import Quote
 
 
 def get_tema(quotes: Iterable[Quote], lookback_periods: int):
     """Get TEMA calculated.
 
@@ -43,13 +43,13 @@
 
     @tema.setter
     def tema(self, value):
         self._csdata.Tema = value
 
 
 _T = TypeVar("_T", bound=TEMAResult)
-class TEMAResults(RemoveWarmupMixin, IndicatorResults[_T]):
+class TEMAResults(CondenseMixin, RemoveWarmupMixin, IndicatorResults[_T]):
     """
     A wrapper class for the list of Triple Exponential Moving Average (TEMA) results.
     It is exactly same with built-in `list` except for that it provides
     some useful helper methods written in C# implementation.
     """
```

### Comparing `stock-indicators-1.2.1/stock_indicators/indicators/tr.py` & `stock_indicators-1.3.0/stock_indicators/indicators/tr.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from typing import Iterable, Optional, TypeVar
 
 from stock_indicators._cslib import CsIndicator
 from stock_indicators._cstypes import List as CsList
+from stock_indicators.indicators.common.helpers import CondenseMixin
 from stock_indicators.indicators.common.results import IndicatorResults, ResultBase
 from stock_indicators.indicators.common.quote import Quote
 
 
 def get_tr(quotes: Iterable[Quote]):
     """Get TR calculated.
 
@@ -38,13 +39,13 @@
 
     @tr.setter
     def tr(self, value):
         self._csdata.Tr = value
 
 
 _T = TypeVar("_T", bound=TrResult)
-class TrResults(IndicatorResults[_T]):
+class TrResults(CondenseMixin, IndicatorResults[_T]):
     """
     A wrapper class for the list of True Range (TR) results.
     It is exactly same with built-in `list` except for that it provides
     some useful helper methods written in C# implementation.
     """
```

### Comparing `stock-indicators-1.2.1/stock_indicators/indicators/trix.py` & `stock_indicators-1.3.0/stock_indicators/indicators/trix.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Iterable, Optional, TypeVar
 
 from stock_indicators._cslib import CsIndicator
 from stock_indicators._cstypes import List as CsList
-from stock_indicators.indicators.common.helpers import RemoveWarmupMixin
+from stock_indicators.indicators.common.helpers import CondenseMixin, RemoveWarmupMixin
 from stock_indicators.indicators.common.results import IndicatorResults, ResultBase
 from stock_indicators.indicators.common.quote import Quote
 
 
 def get_trix(quotes: Iterable[Quote], lookback_periods: int, signal_periods: Optional[int] = None):
     """Get TRIX calculated.
 
@@ -62,13 +62,13 @@
 
     @signal.setter
     def signal(self, value):
         self._csdata.Signal = value
 
 
 _T = TypeVar("_T", bound=TRIXResult)
-class TRIXResults(RemoveWarmupMixin, IndicatorResults[_T]):
+class TRIXResults(CondenseMixin, RemoveWarmupMixin, IndicatorResults[_T]):
     """
     A wrapper class for the list of Triple EMA Oscillator (TRIX) results.
     It is exactly same with built-in `list` except for that it provides
     some useful helper methods written in C# implementation.
     """
```

### Comparing `stock-indicators-1.2.1/stock_indicators/indicators/tsi.py` & `stock_indicators-1.3.0/stock_indicators/indicators/tsi.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Iterable, Optional, TypeVar
 
 from stock_indicators._cslib import CsIndicator
 from stock_indicators._cstypes import List as CsList
-from stock_indicators.indicators.common.helpers import RemoveWarmupMixin
+from stock_indicators.indicators.common.helpers import CondenseMixin, RemoveWarmupMixin
 from stock_indicators.indicators.common.results import IndicatorResults, ResultBase
 from stock_indicators.indicators.common.quote import Quote
 
 
 def get_tsi(quotes: Iterable[Quote], lookback_periods: int = 25,
            smooth_periods: int = 13, signal_periods: int = 7):
     """Get TSI calculated.
@@ -59,13 +59,13 @@
 
     @signal.setter
     def signal(self, value):
         self._csdata.Signal = value
 
 
 _T = TypeVar("_T", bound=TSIResult)
-class TSIResults(RemoveWarmupMixin, IndicatorResults[_T]):
+class TSIResults(CondenseMixin, RemoveWarmupMixin, IndicatorResults[_T]):
     """
     A wrapper class for the list of True Strength Index (TSI) results.
     It is exactly same with built-in `list` except for that it provides
     some useful helper methods written in CSharp implementation.
     """
```

### Comparing `stock-indicators-1.2.1/stock_indicators/indicators/ulcer_index.py` & `stock_indicators-1.3.0/stock_indicators/indicators/ulcer_index.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Iterable, Optional, TypeVar
 
 from stock_indicators._cslib import CsIndicator
 from stock_indicators._cstypes import List as CsList
-from stock_indicators.indicators.common.helpers import RemoveWarmupMixin
+from stock_indicators.indicators.common.helpers import CondenseMixin, RemoveWarmupMixin
 from stock_indicators.indicators.common.results import IndicatorResults, ResultBase
 from stock_indicators.indicators.common.quote import Quote
 
 
 def get_ulcer_index(quotes: Iterable[Quote], lookback_periods: int = 14):
     """Get Ulcer Index calculated.
 
@@ -43,13 +43,13 @@
 
     @ui.setter
     def ui(self, value):
         self._csdata.UI = value
 
 
 _T = TypeVar("_T", bound=UlcerIndexResult)
-class UlcerIndexResults(RemoveWarmupMixin, IndicatorResults[_T]):
+class UlcerIndexResults(CondenseMixin, RemoveWarmupMixin, IndicatorResults[_T]):
     """
     A wrapper class for the list of Ulcer Index (UI) results.
     It is exactly same with built-in `list` except for that it provides
     some useful helper methods written in CSharp implementation.
     """
```

### Comparing `stock-indicators-1.2.1/stock_indicators/indicators/ultimate.py` & `stock_indicators-1.3.0/stock_indicators/indicators/ultimate.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Iterable, Optional, TypeVar
 
 from stock_indicators._cslib import CsIndicator
 from stock_indicators._cstypes import List as CsList
-from stock_indicators.indicators.common.helpers import RemoveWarmupMixin
+from stock_indicators.indicators.common.helpers import CondenseMixin, RemoveWarmupMixin
 from stock_indicators.indicators.common.results import IndicatorResults, ResultBase
 from stock_indicators.indicators.common.quote import Quote
 
 
 def get_ultimate(quotes: Iterable[Quote], short_periods: int = 7,
                  middle_periods: int = 14, long_periods: int = 28):
     """Get Ultimate Oscillator calculated.
@@ -51,13 +51,13 @@
 
     @ultimate.setter
     def ultimate(self, value):
         self._csdata.Ultimate = value
 
 
 _T = TypeVar("_T", bound=UltimateResult)
-class UltimateResults(RemoveWarmupMixin, IndicatorResults[_T]):
+class UltimateResults(CondenseMixin, RemoveWarmupMixin, IndicatorResults[_T]):
     """
     A wrapper class for the list of Ultimate Oscillator results.
     It is exactly same with built-in `list` except for that it provides
     some useful helper methods written in CSharp implementation.
     """
```

### Comparing `stock-indicators-1.2.1/stock_indicators/indicators/volatility_stop.py` & `stock_indicators-1.3.0/stock_indicators/indicators/volatility_stop.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Iterable, Optional, TypeVar
 
 from stock_indicators._cslib import CsIndicator
 from stock_indicators._cstypes import List as CsList
-from stock_indicators.indicators.common.helpers import RemoveWarmupMixin
+from stock_indicators.indicators.common.helpers import CondenseMixin, RemoveWarmupMixin
 from stock_indicators.indicators.common.results import IndicatorResults, ResultBase
 from stock_indicators.indicators.common.quote import Quote
 
 
 def get_volatility_stop(quotes: Iterable[Quote], lookback_periods: int = 7,
                         multiplier: float = 3):
     """Get Volatility Stop calculated.
@@ -72,13 +72,13 @@
 
     @is_stop.setter
     def is_stop(self, value):
         self._csdata.IsStop = value
 
 
 _T = TypeVar("_T", bound=VolatilityStopResult)
-class VolatilityStopResults(RemoveWarmupMixin, IndicatorResults[_T]):
+class VolatilityStopResults(CondenseMixin, RemoveWarmupMixin, IndicatorResults[_T]):
     """
     A wrapper class for the list of Volatility Stop results.
     It is exactly same with built-in `list` except for that it provides
     some useful helper methods written in CSharp implementation.
     """
```

### Comparing `stock-indicators-1.2.1/stock_indicators/indicators/vortex.py` & `stock_indicators-1.3.0/stock_indicators/indicators/vortex.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Iterable, Optional, TypeVar
 
 from stock_indicators._cslib import CsIndicator
 from stock_indicators._cstypes import List as CsList
-from stock_indicators.indicators.common.helpers import RemoveWarmupMixin
+from stock_indicators.indicators.common.helpers import CondenseMixin, RemoveWarmupMixin
 from stock_indicators.indicators.common.results import IndicatorResults, ResultBase
 from stock_indicators.indicators.common.quote import Quote
 
 
 def get_vortex(quotes: Iterable[Quote], lookback_periods: int):
     """Get VI calculated.
 
@@ -52,13 +52,13 @@
 
     @nvi.setter
     def nvi(self, value):
         self._csdata.Nvi = value
 
 
 _T = TypeVar("_T", bound=VortexResult)
-class VortexResults(RemoveWarmupMixin, IndicatorResults[_T]):
+class VortexResults(CondenseMixin, RemoveWarmupMixin, IndicatorResults[_T]):
     """
     A wrapper class for the list of Vortex Indicator (VI) results.
     It is exactly same with built-in `list` except for that it provides
     some useful helper methods written in CSharp implementation.
     """
```

### Comparing `stock-indicators-1.2.1/stock_indicators/indicators/vwap.py` & `stock_indicators-1.3.0/stock_indicators/indicators/vwap.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from datetime import datetime
 from typing import Iterable, Optional, TypeVar, overload
 
 from stock_indicators._cslib import CsIndicator
 from stock_indicators._cstypes import List as CsList
 from stock_indicators._cstypes import DateTime as CsDateTime
-from stock_indicators.indicators.common.helpers import RemoveWarmupMixin
+from stock_indicators.indicators.common.helpers import CondenseMixin, RemoveWarmupMixin
 from stock_indicators.indicators.common.results import IndicatorResults, ResultBase
 from stock_indicators.indicators.common.quote import Quote
 
 
 @overload
 def get_vwap(quotes: Iterable[Quote], start: Optional[datetime] = None) -> "VWAPResults[VWAPResult]": ...
 @overload
@@ -57,13 +57,13 @@
 
     @vwap.setter
     def vwap(self, value):
         self._csdata.Vwap = value
 
 
 _T = TypeVar("_T", bound=VWAPResult)
-class VWAPResults(RemoveWarmupMixin, IndicatorResults[_T]):
+class VWAPResults(CondenseMixin, RemoveWarmupMixin, IndicatorResults[_T]):
     """
     A wrapper class for the list of Volume Weighted Average Price (VWAP) results.
     It is exactly same with built-in `list` except for that it provides
     some useful helper methods written in C# implementation.
     """
```

### Comparing `stock-indicators-1.2.1/stock_indicators/indicators/vwma.py` & `stock_indicators-1.3.0/stock_indicators/indicators/vwma.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Iterable, Optional, TypeVar
 
 from stock_indicators._cslib import CsIndicator
 from stock_indicators._cstypes import List as CsList
-from stock_indicators.indicators.common.helpers import RemoveWarmupMixin
+from stock_indicators.indicators.common.helpers import CondenseMixin, RemoveWarmupMixin
 from stock_indicators.indicators.common.results import IndicatorResults, ResultBase
 from stock_indicators.indicators.common.quote import Quote
 
 
 def get_vwma(quotes: Iterable[Quote], lookback_periods: int):
     """Get VWMA calculated.
 
@@ -43,13 +43,13 @@
 
     @vwma.setter
     def vwma(self, value):
         self._csdata.Vwma = value
 
 
 _T = TypeVar("_T", bound=VWMAResult)
-class VWMAResults(RemoveWarmupMixin, IndicatorResults[_T]):
+class VWMAResults(CondenseMixin, RemoveWarmupMixin, IndicatorResults[_T]):
     """
     A wrapper class for the list of Volume Weighted Moving Average (VWMA) results.
     It is exactly same with built-in `list` except for that it provides
     some useful helper methods written in CSharp implementation.
     """
```

### Comparing `stock-indicators-1.2.1/stock_indicators/indicators/williams_r.py` & `stock_indicators-1.3.0/stock_indicators/indicators/williams_r.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Iterable, Optional, TypeVar
 
 from stock_indicators._cslib import CsIndicator
 from stock_indicators._cstypes import List as CsList
-from stock_indicators.indicators.common.helpers import RemoveWarmupMixin
+from stock_indicators.indicators.common.helpers import CondenseMixin, RemoveWarmupMixin
 from stock_indicators.indicators.common.results import IndicatorResults, ResultBase
 from stock_indicators.indicators.common.quote import Quote
 
 
 def get_williams_r(quotes: Iterable[Quote], lookback_periods: int = 14):
     """Get Williams %R calculated.
 
@@ -44,13 +44,13 @@
 
     @williams_r.setter
     def williams_r(self, value):
         self._csdata.WilliamsR = value
 
 
 _T = TypeVar("_T", bound=WilliamsResult)
-class WilliamsResults(RemoveWarmupMixin, IndicatorResults[_T]):
+class WilliamsResults(CondenseMixin, RemoveWarmupMixin, IndicatorResults[_T]):
     """
     A wrapper class for the list of Williams %R results.
     It is exactly same with built-in `list` except for that it provides
     some useful helper methods written in CSharp implementation.
     """
```

### Comparing `stock-indicators-1.2.1/stock_indicators/indicators/wma.py` & `stock_indicators-1.3.0/stock_indicators/indicators/wma.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Iterable, Optional, TypeVar
 
 from stock_indicators._cslib import CsIndicator
 from stock_indicators.indicators.common.enums import CandlePart
-from stock_indicators.indicators.common.helpers import RemoveWarmupMixin
+from stock_indicators.indicators.common.helpers import CondenseMixin, RemoveWarmupMixin
 from stock_indicators.indicators.common.results import IndicatorResults, ResultBase
 from stock_indicators.indicators.common.quote import Quote
 
 
 def get_wma(quotes: Iterable[Quote], lookback_periods: int,
             candle_part: CandlePart = CandlePart.CLOSE):
     """Get WMA calculated.
@@ -49,13 +49,13 @@
 
     @wma.setter
     def wma(self, value):
         self._csdata.Wma = value
 
 
 _T = TypeVar("_T", bound=WMAResult)
-class WMAResults(RemoveWarmupMixin, IndicatorResults[_T]):
+class WMAResults(CondenseMixin, RemoveWarmupMixin, IndicatorResults[_T]):
     """
     A wrapper class for the list of Weighted Moving Average (WMA) results.
     It is exactly same with built-in `list` except for that it provides
     some useful helper methods written in CSharp implementation.
     """
```

### Comparing `stock-indicators-1.2.1/stock_indicators/indicators/zig_zag.py` & `stock_indicators-1.3.0/stock_indicators/indicators/zig_zag.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from typing import Iterable, Optional, TypeVar
 
 from stock_indicators._cslib import CsIndicator
 from stock_indicators._cstypes import List as CsList
 from stock_indicators._cstypes import Decimal as CsDecimal
 from stock_indicators._cstypes import to_pydecimal
 from stock_indicators.indicators.common.enums import EndType
+from stock_indicators.indicators.common.helpers import CondenseMixin
 from stock_indicators.indicators.common.results import IndicatorResults, ResultBase
 from stock_indicators.indicators.common.quote import Quote
 
 
 def get_zig_zag(quotes: Iterable[Quote], end_type: EndType = EndType.CLOSE,
                 percent_change: float = 5):
     """Get Zig Zag calculated.
@@ -75,13 +76,13 @@
 
     @retrace_low.setter
     def retrace_low(self, value):
         self._csdata.RetraceLow = CsDecimal(value)
 
 
 _T = TypeVar("_T", bound=ZigZagResult)
-class ZigZagResults(IndicatorResults[_T]):
+class ZigZagResults(CondenseMixin, IndicatorResults[_T]):
     """
     A wrapper class for the list of Zig Zag results.
     It is exactly same with built-in `list` except for that it provides
     some useful helper methods written in CSharp implementation.
     """
```

### Comparing `stock-indicators-1.2.1/stock_indicators.egg-info/SOURCES.txt` & `stock_indicators-1.3.0/stock_indicators.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,43 +1,44 @@
 .editorconfig
+.gitattributes
 .gitignore
 .pylintrc
 LICENSE
 README.md
 pyproject.toml
 requirements-test.txt
 requirements.txt
 .github/CODE_OF_CONDUCT.md
 .github/PULL_REQUEST_TEMPLATE.md
 .github/SECURITY.md
 .github/dependabot.yml
 .github/ISSUE_TEMPLATE/bug_report.md
 .github/ISSUE_TEMPLATE/feature_request.md
-.github/workflows/deploy.yml
-.github/workflows/docs-deploy.yml
-.github/workflows/docs-test-a11y.yml
-.github/workflows/docs-test-links.yml
-.github/workflows/lock.yml
-.github/workflows/semantic-pr-linter.yml
-.github/workflows/test-all-env.yml
-.github/workflows/test-coverage.yml
-.github/workflows/test.yml
+.github/workflows/deploy-package.yml
+.github/workflows/deploy-website.yml
+.github/workflows/lint-pull-request.yml
+.github/workflows/lock-issue-pr.yml
+.github/workflows/test-docs-a11y.yml
+.github/workflows/test-docs-links.yml
+.github/workflows/test-indicators-all-env.yml
+.github/workflows/test-indicators-coverage.yml
+.github/workflows/test-indicators.yml
 benchmarks/__init__.py
 benchmarks/conftest.py
 benchmarks/test_benchmark_indicators.py
 docs/.pa11yci
 docs/404.html
 docs/GemFile
 docs/GemFile.lock
 docs/README.md
 docs/_config.yml
 docs/contributing.md
 docs/favicon.ico
-docs/.offline/banner.png
-docs/.offline/banner.xcf
+docs/.offline/social-banner.pptx
+docs/.offline/social-banner.svg
 docs/_data/aliases.yml
 docs/_data/categories.yml
 docs/_includes/candle-result.md
 docs/_includes/candlepart-options.md
 docs/_includes/cyclotron.html
 docs/_includes/footer.html
 docs/_includes/head-style.html
@@ -183,30 +184,33 @@
 stock_indicators/indicators/__init__.py
 stock_indicators/indicators/adl.py
 stock_indicators/indicators/adx.py
 stock_indicators/indicators/alligator.py
 stock_indicators/indicators/alma.py
 stock_indicators/indicators/aroon.py
 stock_indicators/indicators/atr.py
+stock_indicators/indicators/atr_stop.py
 stock_indicators/indicators/awesome.py
 stock_indicators/indicators/basic_quotes.py
 stock_indicators/indicators/beta.py
 stock_indicators/indicators/bollinger_bands.py
 stock_indicators/indicators/bop.py
 stock_indicators/indicators/cci.py
 stock_indicators/indicators/chaikin_oscillator.py
 stock_indicators/indicators/chandelier.py
 stock_indicators/indicators/chop.py
 stock_indicators/indicators/cmf.py
+stock_indicators/indicators/cmo.py
 stock_indicators/indicators/connors_rsi.py
 stock_indicators/indicators/correlation.py
 stock_indicators/indicators/dema.py
 stock_indicators/indicators/doji.py
 stock_indicators/indicators/donchian.py
 stock_indicators/indicators/dpo.py
+stock_indicators/indicators/dynamic.py
 stock_indicators/indicators/elder_ray.py
 stock_indicators/indicators/ema.py
 stock_indicators/indicators/epma.py
 stock_indicators/indicators/fcb.py
 stock_indicators/indicators/fisher_transform.py
 stock_indicators/indicators/force_index.py
 stock_indicators/indicators/fractal.py
@@ -273,30 +277,33 @@
 tests/conftest.py
 tests/test_adl.py
 tests/test_adx.py
 tests/test_alligator.py
 tests/test_alma.py
 tests/test_aroon.py
 tests/test_atr.py
+tests/test_atr_stop.py
 tests/test_awesome.py
 tests/test_basic_quote.py
 tests/test_beta.py
 tests/test_bollinger_bands.py
 tests/test_bop.py
 tests/test_cci.py
 tests/test_chaikin_oscillator.py
 tests/test_chandelier.py
 tests/test_chop.py
 tests/test_cmf.py
+tests/test_cmo.py
 tests/test_connors_rsi.py
 tests/test_correlation.py
 tests/test_dema.py
 tests/test_doji.py
 tests/test_donchian.py
 tests/test_dpo.py
+tests/test_dynamic.py
 tests/test_elder_ray.py
 tests/test_ema.py
 tests/test_epma.py
 tests/test_fcb.py
 tests/test_fisher_transform.py
 tests/test_force_index.py
 tests/test_fractal.py
@@ -323,15 +330,15 @@
 tests/test_pvo.py
 tests/test_renko.py
 tests/test_roc.py
 tests/test_rolling_pivots.py
 tests/test_rsi.py
 tests/test_slope.py
 tests/test_sma.py
-tests/test_sma_extended.py
+tests/test_sma_analysis.py
 tests/test_smi.py
 tests/test_smma.py
 tests/test_starc_bands.py
 tests/test_stc.py
 tests/test_stdev.py
 tests/test_stdev_channels.py
 tests/test_stoch.py
```

### Comparing `stock-indicators-1.2.1/tests/common/test_candle.py` & `stock_indicators-1.3.0/tests/common/test_candle.py`

 * *Files identical despite different names*

### Comparing `stock-indicators-1.2.1/tests/common/test_common.py` & `stock_indicators-1.3.0/tests/common/test_common.py`

 * *Files identical despite different names*

### Comparing `stock-indicators-1.2.1/tests/common/test_cstypes.py` & `stock_indicators-1.3.0/tests/common/test_cstypes.py`

 * *Files identical despite different names*

### Comparing `stock-indicators-1.2.1/tests/common/test_indicator_results.py` & `stock_indicators-1.3.0/tests/common/test_indicator_results.py`

 * *Files 7% similar despite different names*

```diff
@@ -45,17 +45,24 @@
         r2 = results * 2
         
         assert len(r2) == len(results) * 2
         
     def test_find(self, quotes):
         results = indicators.get_sma(quotes, 20)
         
-        # r[18]
-        r = results.find(datetime(2017, 1, 30))
-        assert r.sma is None
+        # r[19]
+        r = results.find(datetime(2017, 1, 31))
+        assert 214.5250 == round(float(r.sma), 4)
+
+    def test_not_found(self, quotes):
+        results = indicators.get_sma(quotes, 20)
+        
+        # returns None
+        r = results.find(datetime(1996, 10, 12))
+        assert r is None
 
     def test_remove_with_period(self, quotes):
         results = indicators.get_sma(quotes, 20)
         length = len(results)
         
         results = results.remove_warmup_periods(50)
         assert len(results) == length - 50
```

### Comparing `stock-indicators-1.2.1/tests/common/test_type_compatibility.py` & `stock_indicators-1.3.0/tests/common/test_type_compatibility.py`

 * *Files identical despite different names*

### Comparing `stock-indicators-1.2.1/tests/conftest.py` & `stock_indicators-1.3.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `stock-indicators-1.2.1/tests/test_adl.py` & `stock_indicators-1.3.0/tests/test_adl.py`

 * *Files 13% similar despite different names*

```diff
@@ -48,12 +48,22 @@
 
         r = results[501]
         assert 0.8052        == round(float(r.money_flow_multiplier), 4)
         assert 118396116.25  == round(float(r.money_flow_volume),     2)
         assert 3439986548.42 == round(float(r.adl),                   2)
         assert 3595352721.16 == round(float(r.adl_sma),               2)
 
+    def test_condense(self, quotes):
+        results = indicators.get_adl(quotes).condense()
+
+        assert 502 == len(results)
+
+        r = results[-1]
+        assert 0.8052        == round(float(r.money_flow_multiplier), 4)
+        assert 118396116.25  == round(float(r.money_flow_volume),     2)
+        assert 3439986548.42 == round(float(r.adl),                   2)
+        assert r.adl_sma is None
 
     def test_exceptions(self, quotes):
         from System import ArgumentOutOfRangeException
         with pytest.raises(ArgumentOutOfRangeException):
             indicators.get_adl(quotes, 0)
```

### Comparing `stock-indicators-1.2.1/tests/test_adx.py` & `stock_indicators-1.3.0/tests/test_adx.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,11 +50,21 @@
         assert 502 - (2 * 14 + 100) == len(results)
 
         r = results[len(results)-1]
         assert 17.7565 == round(float(r.pdi), 4)
         assert 31.1510 == round(float(r.mdi), 4)
         assert 34.2987 == round(float(r.adx), 4)
 
+    def test_condense(self, quotes):
+        results = indicators.get_adx(quotes, 14).condense()
+
+        assert 475 == len(results)
+
+        r = results[-1]
+        assert 17.7565 == round(float(r.pdi), 4)
+        assert 31.1510 == round(float(r.mdi), 4)
+        assert 34.2987 == round(float(r.adx), 4)
+
     def test_exceptions(self, quotes):
         from System import ArgumentOutOfRangeException
         with pytest.raises(ArgumentOutOfRangeException):
             indicators.get_adx(quotes, 1)
```

### Comparing `stock-indicators-1.2.1/tests/test_alligator.py` & `stock_indicators-1.3.0/tests/test_alligator.py`

 * *Files 3% similar despite different names*

```diff
@@ -55,15 +55,25 @@
 
         assert 502 - 21 - 250 == len(results)
 
         r = results[len(results)-1]
         assert 260.98953 == round(float(r.jaw), 5)
         assert 253.53576 == round(float(r.teeth), 5)
         assert 244.29591 == round(float(r.lips), 5)
-    
+
+    def test_condense(self, quotes):
+        results = indicators.get_alligator(quotes).condense()
+
+        assert 495 == len(results)
+
+        r = results[-1]
+        assert 260.98953 == round(float(r.jaw), 5)
+        assert  253.53576 == round(float(r.teeth), 5)
+        assert 244.29591 == round(float(r.lips), 5)
+
     def test_exceptions(self, quotes):
         from System import ArgumentOutOfRangeException
         with pytest.raises(ArgumentOutOfRangeException):
             indicators.get_alligator(quotes, 13, 8, 13, 5, 5, 3)
             
         with pytest.raises(ArgumentOutOfRangeException):
             indicators.get_alligator(quotes, 13, 8, 8, 5, 8, 3)
```

### Comparing `stock-indicators-1.2.1/tests/test_alma.py` & `stock_indicators-1.3.0/tests/test_alma.py`

 * *Files 6% similar despite different names*

```diff
@@ -36,14 +36,22 @@
         results = indicators.get_alma(quotes, 10, .85, 6).remove_warmup_periods()
 
         assert 502 - 9 == len(results)
         
         last = results.pop()
         assert 242.1871 == round(float(last.alma), 4)
 
+    def test_condense(self, quotes):
+        results = indicators.get_alma(quotes, 10, .85, 6).condense()
+
+        assert 493 == len(results)
+
+        r = results[-1]
+        assert 242.1871 == round(float(r.alma), 4)
+
     def test_exceptions(self, quotes):
         from System import ArgumentOutOfRangeException
         with pytest.raises(ArgumentOutOfRangeException):
             indicators.get_alma(quotes, 0, 1, 5)
         
         with pytest.raises(ArgumentOutOfRangeException):
             indicators.get_alma(quotes, 15, 1.1, 3)
```

### Comparing `stock-indicators-1.2.1/tests/test_aroon.py` & `stock_indicators-1.3.0/tests/test_aroon.py`

 * *Files 6% similar despite different names*

```diff
@@ -46,11 +46,21 @@
         assert 502 - 25 == len(results)
 
         last = results.pop()
         assert +28 == float(last.aroon_up)
         assert +88 == float(last.aroon_down)
         assert -60 == float(last.oscillator)
 
+    def test_condense(self, quotes):
+        results = indicators.get_aroon(quotes, 25).condense()
+
+        assert 477 == len(results)
+
+        r = results[-1]
+        assert  28 == float(r.aroon_up)
+        assert  88 == float(r.aroon_down)
+        assert -60 == float(r.oscillator)
+
     def test_exceptions(self, quotes):
         from System import ArgumentOutOfRangeException
         with pytest.raises(ArgumentOutOfRangeException):
             indicators.get_aroon(quotes, 0)
```

### Comparing `stock-indicators-1.2.1/tests/test_atr.py` & `stock_indicators-1.3.0/tests/test_atr.py`

 * *Files 16% similar despite different names*

```diff
@@ -44,11 +44,21 @@
         assert 488 == len(results)
 
         last = results.pop()
         assert 2.6700 == round(float(last.tr), 4)
         assert 6.1497 == round(float(last.atr), 4)
         assert 2.5072 == round(float(last.atrp), 4)
 
+    def test_condense(self, quotes):
+        results = indicators.get_atr(quotes, 14).condense()
+
+        assert 488 == len(results)
+
+        last = results.pop()
+        assert 2.6700 == round(float(last.tr), 4)
+        assert 6.1497 == round(float(last.atr), 4)
+        assert 2.5072 == round(float(last.atrp), 4)
+
     def test_exceptions(self, quotes):
         from System import ArgumentOutOfRangeException
         with pytest.raises(ArgumentOutOfRangeException):
             indicators.get_atr(quotes, 1)
```

### Comparing `stock-indicators-1.2.1/tests/test_awesome.py` & `stock_indicators-1.3.0/tests/test_awesome.py`

 * *Files 9% similar despite different names*

```diff
@@ -34,14 +34,23 @@
 
         assert 502 - 33 == len(results)
 
         last = results.pop()
         assert -17.7692 == round(float(last.oscillator), 4)
         assert -7.2763  == round(float(last.normalized), 4)
 
+    def test_condense(self, quotes):
+        results = indicators.get_awesome(quotes, 5, 34).condense()
+
+        assert 469 == len(results)
+
+        last = results.pop()
+        assert -17.7692 == round(float(last.oscillator), 4)
+        assert -7.2763  == round(float(last.normalized), 4)
+
     def test_exceptions(self, quotes):
         from System import ArgumentOutOfRangeException
         with pytest.raises(ArgumentOutOfRangeException):
             indicators.get_awesome(quotes, 0, 34)
 
         with pytest.raises(ArgumentOutOfRangeException):
             indicators.get_awesome(quotes, 25, 25)
```

### Comparing `stock-indicators-1.2.1/tests/test_basic_quote.py` & `stock_indicators-1.3.0/tests/test_basic_quote.py`

 * *Files identical despite different names*

### Comparing `stock-indicators-1.2.1/tests/test_beta.py` & `stock_indicators-1.3.0/tests/test_beta.py`

 * *Files 9% similar despite different names*

```diff
@@ -30,15 +30,15 @@
         r = results[249]
         assert  1.9200 == round(float(r.beta), 4)
         assert -1.2289 == round(float(r.beta_up), 4)
         assert -0.3956 == round(float(r.beta_down), 4)
         assert  3.1066 == round(float(r.ratio), 4)
         assert  0.6944 == round(float(r.convexity), 4)
         
-        r= results[501]
+        r = results[501]
         assert 1.5123 == round(float(r.beta), 4)
         assert 2.0721 == round(float(r.beta_up), 4)
         assert 1.5908 == round(float(r.beta_down), 4)
         assert 1.3026 == round(float(r.ratio), 4)
         assert 0.2316 == round(float(r.convexity), 4)
         
     def test_standard(self, quotes, other_quotes):
@@ -110,14 +110,26 @@
     def test_no_quotes(self, quotes):
         r = indicators.get_beta([], [], 5)
         assert 0 == len(r)
         
         r = indicators.get_beta(quotes[:1], quotes[:1], 5)
         assert 1 == len(r)
 
+    def test_condense(self, quotes, other_quotes):
+        results = indicators.get_beta(other_quotes, quotes, 20, BetaType.ALL).condense()
+
+        assert 482 == len(results)
+
+        r = results[-1]
+        assert 1.5123 == round(float(r.beta), 4)
+        assert 2.0721 == round(float(r.beta_up), 4)
+        assert 1.5908 == round(float(r.beta_down), 4)
+        assert 1.3026 == round(float(r.ratio), 4)
+        assert 0.2316 == round(float(r.convexity), 4)
+
     def test_exceptions(self, quotes, other_quotes):
         from System import ArgumentOutOfRangeException
         with pytest.raises(ArgumentOutOfRangeException):
             indicators.get_beta(quotes, other_quotes, 0)
 
         from Skender.Stock.Indicators import InvalidQuotesException
         with pytest.raises(InvalidQuotesException):
```

### Comparing `stock-indicators-1.2.1/tests/test_bollinger_bands.py` & `stock_indicators-1.3.0/tests/test_bollinger_bands.py`

 * *Files 9% similar despite different names*

```diff
@@ -25,15 +25,14 @@
         assert 251.8600  == round(float(r.sma), 4)
         assert 273.7004  == round(float(r.upper_band), 4)
         assert 230.0196  == round(float(r.lower_band), 4)
         assert 0.349362  == round(float(r.percent_b), 6)
         assert -0.602552 == round(float(r.z_score), 6)
         assert 0.173433  == round(float(r.width), 6)
 
-
     def test_bad_data(self, bad_quotes):
         r = indicators.get_bollinger_bands(bad_quotes, 15, 3)
 
         assert 502 == len(r)
 
     def test_removed(self, quotes):
         results = indicators.get_bollinger_bands(quotes, 20, 2).remove_warmup_periods()
@@ -44,14 +43,28 @@
         assert 251.8600  == round(float(last.sma), 4)
         assert 273.7004  == round(float(last.upper_band), 4)
         assert 230.0196  == round(float(last.lower_band), 4)
         assert 0.349362  == round(float(last.percent_b), 6)
         assert -0.602552 == round(float(last.z_score), 6)
         assert 0.173433  == round(float(last.width), 6)
 
+    def test_condense(self, quotes):
+        results = indicators.get_bollinger_bands(quotes, 20, 2).condense()
+
+        assert 483 == len(results)
+
+        last = results.pop()
+        assert 251.8600  == round(float(last.sma), 4)
+        assert 273.7004  == round(float(last.upper_band), 4)
+        assert 230.0196  == round(float(last.lower_band), 4)
+        assert 0.349362  == round(float(last.percent_b), 6)
+        assert -0.602552 == round(float(last.z_score), 6)
+        assert 0.173433  == round(float(last.width), 6)
+
+
     def test_exceptions(self, quotes):
         from System import ArgumentOutOfRangeException
         with pytest.raises(ArgumentOutOfRangeException):
             indicators.get_bollinger_bands(quotes, 1)
         
         with pytest.raises(ArgumentOutOfRangeException):
             indicators.get_bollinger_bands(quotes, 2, 0)
```

### Comparing `stock-indicators-1.2.1/tests/test_bop.py` & `stock_indicators-1.3.0/tests/test_bop.py`

 * *Files 8% similar despite different names*

```diff
@@ -30,12 +30,20 @@
     def test_removed(self, quotes):
         results = indicators.get_bop(quotes).remove_warmup_periods()
         
         assert 502 - 13 == len(results)
         
         last = results.pop()
         assert -0.292788 == round(float(last.bop), 6)
-        
+
+    def test_condense(self, quotes):
+        results = indicators.get_bop(quotes).condense()
+
+        assert 489 == len(results)
+
+        last = results.pop()
+        assert -0.292788 == round(float(last.bop), 6)
+
     def test_exceptions(self, quotes):
         from System import ArgumentOutOfRangeException
         with pytest.raises(ArgumentOutOfRangeException):
             indicators.get_bop(quotes, 0)
```

### Comparing `stock-indicators-1.2.1/tests/test_cci.py` & `stock_indicators-1.3.0/tests/test_cci.py`

 * *Files 11% similar despite different names*

```diff
@@ -18,12 +18,20 @@
     def test_removed(self, quotes):
         results = indicators.get_cci(quotes, 20).remove_warmup_periods()
         
         assert 502 - 19 == len(results)
         
         last = results.pop()
         assert -52.9946 == round(float(last.cci), 4)
-        
+
+    def test_condense(self, quotes):
+        results = indicators.get_cci(quotes, 20).condense()
+
+        assert 483 == len(results)
+
+        last = results.pop()
+        assert -52.9946 == round(float(last.cci), 4)
+
     def test_exceptions(self, quotes):
         from System import ArgumentOutOfRangeException
         with pytest.raises(ArgumentOutOfRangeException):
             indicators.get_cci(quotes, 0)
```

### Comparing `stock-indicators-1.2.1/tests/test_chaikin_oscillator.py` & `stock_indicators-1.3.0/tests/test_chaikin_oscillator.py`

 * *Files 18% similar despite different names*

```diff
@@ -30,15 +30,26 @@
         assert 502 - (slow_periods + 100) == len(results)
         
         last = results.pop()
         assert 3439986548.42 == round(float(last.adl), 2)
         assert        0.8052 == round(float(last.money_flow_multiplier), 4)
         assert  118396116.25 == round(float(last.money_flow_volume), 2)
         assert  -19135200.72 == round(float(last.oscillator), 2)
-        
+
+    def test_condense(self, quotes):
+        results = indicators.get_chaikin_osc(quotes, 3, 10).condense()
+
+        assert 493 == len(results)
+
+        last = results.pop()
+        assert 3439986548.42 == round(float(last.adl), 2)
+        assert        0.8052 == round(float(last.money_flow_multiplier), 4)
+        assert  118396116.25 == round(float(last.money_flow_volume), 2)
+        assert  -19135200.72 == round(float(last.oscillator), 2)
+
     def test_exceptions(self, quotes):
         from System import ArgumentOutOfRangeException
         with pytest.raises(ArgumentOutOfRangeException):
             indicators.get_chaikin_osc(quotes, 0)
         
         with pytest.raises(ArgumentOutOfRangeException):
             indicators.get_chaikin_osc(quotes, 10, 5)
```

### Comparing `stock-indicators-1.2.1/tests/test_chandelier.py` & `stock_indicators-1.3.0/tests/test_chandelier.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,14 +35,22 @@
         long_results = indicators.get_chandelier(quotes, 22, 3).remove_warmup_periods()
 
         assert 480 == len(long_results)
 
         last = long_results.pop()
         assert 256.5860 == round(float(last.chandelier_exit), 4)
 
+    def test_condense(self, quotes):
+        long_results = indicators.get_chandelier(quotes, 22, 3).condense()
+
+        assert 480 == len(long_results)
+
+        last = long_results.pop()
+        assert 256.5860 == round(float(last.chandelier_exit), 4)
+
     def test_exceptions(self, quotes):
         from System import ArgumentOutOfRangeException
         with pytest.raises(ArgumentOutOfRangeException):
             indicators.get_chandelier(quotes, 0)
 
         with pytest.raises(ArgumentOutOfRangeException):
             indicators.get_chandelier(quotes, 25, 0)
```

### Comparing `stock-indicators-1.2.1/tests/test_chop.py` & `stock_indicators-1.3.0/tests/test_cmo.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,44 +1,54 @@
 import pytest
 from stock_indicators import indicators
 
-class TestChop:
+class TestCMO:
     def test_standard(self, quotes):
-        results = indicators.get_chop(quotes, 14)
+        results = indicators.get_cmo(quotes, 14)
         
         assert 502 == len(results)
-        assert 488 == len(list(filter(lambda x: x.chop is not None, results)))
+        assert 488 == len(list(filter(lambda x: x.cmo is not None, results)))
         
         r = results[13]
-        assert r.chop is None
-        
+        assert r.cmo is None
+
         r = results[14]
-        assert 69.9967 == round(float(r.chop), 4)
-        
+        assert 24.1081 == round(float(r.cmo), 4)
+
         r = results[249]
-        assert 41.8499 == round(float(r.chop), 4)
-        
+        assert 48.9614 == round(float(r.cmo), 4)
+
         r = results[501]
-        assert 38.6526 == round(float(r.chop), 4)
-        
-    def test_small_lookback(self, quotes):
-        results = indicators.get_chop(quotes, 2)
-        
-        assert 502 == len(results)
-        assert 500 == len(list(filter(lambda x: x.chop is not None, results)))
-        
+        assert -26.7502 == round(float(r.cmo), 4)
+
     def test_bad_data(self, bad_quotes):
-        r = indicators.get_chop(bad_quotes, 20)
+        r = indicators.get_cmo(bad_quotes, 15)
+        
         assert 502 == len(r)
-    
+
+    def test_no_quotes(self, quotes):
+        r = indicators.get_cmo([], 5)
+        assert 0 == len(r)
+
+        r = indicators.get_cmo(quotes[:1], 5)
+        assert 1 == len(r)
+   
     def test_removed(self, quotes):
-        results = indicators.get_chop(quotes, 14).remove_warmup_periods()
+        results = indicators.get_cmo(quotes, 14).remove_warmup_periods()
         
-        assert 502 - 14 == len(results)
+        assert 488 == len(results)
         
         last = results.pop()
-        assert 38.6526 == round(float(last.chop), 4)
-        
+        assert -26.7502 == round(float(last.cmo), 4)
+
+    def test_condense(self, quotes):
+        results = indicators.get_cmo(quotes, 14).condense()
+
+        assert 488 == len(results)
+
+        last = results.pop()
+        assert -26.7502 == round(float(last.cmo), 4)
+
     def test_exceptions(self, quotes):
         from System import ArgumentOutOfRangeException
         with pytest.raises(ArgumentOutOfRangeException):
-            indicators.get_chop(quotes, 1)
+            indicators.get_cmo(quotes, 0)
```

### Comparing `stock-indicators-1.2.1/tests/test_cmf.py` & `stock_indicators-1.3.0/tests/test_cmf.py`

 * *Files 11% similar despite different names*

```diff
@@ -36,12 +36,22 @@
         
         assert 502 - 19 == len(results)
         
         last = results.pop()
         assert       0.8052 == round(float(last.money_flow_multiplier), 4)
         assert 118396116.25 == round(float(last.money_flow_volume), 2)
         assert    -0.123754 == round(float(last.cmf), 6)
-   
+
+    def test_condense(self, quotes):
+        results = indicators.get_cmf(quotes, 20).condense()
+
+        assert 483 == len(results)
+
+        last = results.pop()
+        assert       0.8052 == round(float(last.money_flow_multiplier), 4)
+        assert 118396116.25 == round(float(last.money_flow_volume), 2)
+        assert    -0.123754 == round(float(last.cmf), 6)
+
     def test_exceptions(self, quotes):
         from System import ArgumentOutOfRangeException
         with pytest.raises(ArgumentOutOfRangeException):
             indicators.get_cmf(quotes, 0)
```

### Comparing `stock-indicators-1.2.1/tests/test_connors_rsi.py` & `stock_indicators-1.3.0/tests/test_connors_rsi.py`

 * *Files 5% similar despite different names*

```diff
@@ -42,15 +42,27 @@
         results = results.remove_warmup_periods()
         
         last = results.pop()
         assert 68.8087 == round(float(last.rsi_close), 4)
         assert 67.4899 == round(float(last.rsi_streak), 4)
         assert 88.0000 == round(float(last.percent_rank), 4)
         assert 74.7662 == round(float(last.connors_rsi), 4)
+
+    def test_condense(self, quotes):
+        results = indicators.get_connors_rsi(quotes, 3, 2, 100)
+        results = results.condense()
         
+        assert 401 == len(results)
+
+        last = results.pop()
+        assert 68.8087 == round(float(last.rsi_close), 4)
+        assert 67.4899 == round(float(last.rsi_streak), 4)
+        assert 88.0000 == round(float(last.percent_rank), 4)
+        assert 74.7662 == round(float(last.connors_rsi), 4)
+
     def test_exceptions(self, quotes):
         from System import ArgumentOutOfRangeException
         with pytest.raises(ArgumentOutOfRangeException):
             indicators.get_connors_rsi(quotes, 1, 2, 100)
         
         with pytest.raises(ArgumentOutOfRangeException):
             indicators.get_connors_rsi(quotes, 3, 1, 100)
```

### Comparing `stock-indicators-1.2.1/tests/test_correlation.py` & `stock_indicators-1.3.0/tests/test_correlation.py`

 * *Files 10% similar despite different names*

```diff
@@ -37,12 +37,21 @@
         results = results.remove_warmup_periods()
         
         assert 502 - 19 == len(results)
         
         last = results.pop()
         assert 0.8460 == round(float(last.correlation), 4)
         assert 0.7157 == round(float(last.r_squared), 4)
-        
+
+    def test_condense(self, quotes, other_quotes):
+        results = indicators.get_correlation(quotes, other_quotes, 20).condense()
+
+        assert 483 == len(results)
+
+        last = results.pop()
+        assert 0.8460 == round(float(last.correlation), 4)
+        assert 0.7157 == round(float(last.r_squared), 4)
+
     def test_exceptions(self, quotes, other_quotes):
         from System import ArgumentOutOfRangeException
         with pytest.raises(ArgumentOutOfRangeException):
             indicators.get_correlation(quotes, other_quotes, 0)
```

### Comparing `stock-indicators-1.2.1/tests/test_dema.py` & `stock_indicators-1.3.0/tests/test_smma.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,35 +1,62 @@
 import pytest
 from stock_indicators import indicators
 
-class TestDoubleEMA:
+class TestSMMA:
     def test_standard(self, quotes):
-        results = indicators.get_dema(quotes, 20)
+        results = indicators.get_smma(quotes, 20)
         
         assert 502 == len(results)
-        assert 483 == len(list(filter(lambda x: x.dema is not None, results)))
+        assert 483 == len(list(filter(lambda x: x.smma is not None, results)))
         
-        r = results[51]
-        assert 225.8259 == round(float(r.dema), 4)
+        r = results[18]
+        assert r.smma is None
         
-        r = results[249]
-        assert 258.4452 == round(float(r.dema), 4)
+        r = results[19]
+        assert r.smma is not None
         
-        r = results[501]
-        assert 241.1677 == round(float(r.dema), 4)
+        r = results[19]
+        assert 214.52500 == round(float(r.smma), 5)
+        
+        r = results[20]
+        assert 214.55125 == round(float(r.smma), 5)
+        
+        r = results[21]
+        assert 214.58319 == round(float(r.smma), 5)
+        
+        r = results[100]
+        assert 225.78071 == round(float(r.smma), 5)
         
+        r = results[501]
+        assert 255.67462 == round(float(r.smma), 5)
+       
     def test_bad_data(self, bad_quotes):
-        r = indicators.get_dema(bad_quotes, 15)
+        r = indicators.get_smma(bad_quotes, 15)
         assert 502 == len(r)
         
+    def test_no_quotes(self, quotes):
+        r = indicators.get_smma([], 5)
+        assert 0 == len(r)
+        
+        r = indicators.get_smma(quotes[:1], 5)
+        assert 1 == len(r)
+        
     def test_removed(self, quotes):
-        results = indicators.get_dema(quotes, 20).remove_warmup_periods()
+        results = indicators.get_smma(quotes, 20).remove_warmup_periods()
         
-        assert 502 - (2 * 20 + 100) == len(results)
+        assert 502 - (20 + 100) == len(results)
         
         last = results.pop()
-        assert 241.1677 == round(float(last.dema), 4)
-        
-    def test_exceptions(self, quotes):
+        assert 255.67462 == round(float(last.smma), 5)
+
+    def test_condense(self, quotes):
+        results = indicators.get_smma(quotes, 20).condense()
+
+        assert 483 == len(results)
+
+        last = results.pop()
+        assert 255.67462 == round(float(last.smma), 5)
+
+    def test_exceptions(self, quotes, other_quotes, mismatch_quotes):
         from System import ArgumentOutOfRangeException
         with pytest.raises(ArgumentOutOfRangeException):
-            indicators.get_dema(quotes, 0)
+            indicators.get_smma(quotes, 0)
```

### Comparing `stock-indicators-1.2.1/tests/test_doji.py` & `stock_indicators-1.3.0/tests/test_doji.py`

 * *Files identical despite different names*

### Comparing `stock-indicators-1.2.1/tests/test_donchian.py` & `stock_indicators-1.3.0/tests/test_donchian.py`

 * *Files 6% similar despite different names*

```diff
@@ -51,12 +51,23 @@
         assert 502 - 20 == len(results)
         
         last = results.pop()
         assert 251.5050 == round(float(last.center_line), 4)
         assert 273.5900 == round(float(last.upper_band), 4)
         assert 229.4200 == round(float(last.lower_band), 4)
         assert 0.175623 == round(float(last.width), 6)
-        
+
+    def test_condense(self, quotes):
+        results = indicators.get_donchian(quotes, 20).condense()
+
+        assert 482 == len(results)
+
+        last = results.pop()
+        assert 251.5050 == round(float(last.center_line), 4)
+        assert 273.5900 == round(float(last.upper_band), 4)
+        assert 229.4200 == round(float(last.lower_band), 4)
+        assert 0.175623 == round(float(last.width), 6)
+
     def test_exceptions(self, quotes):
         from System import ArgumentOutOfRangeException
         with pytest.raises(ArgumentOutOfRangeException):
             indicators.get_donchian(quotes, 0)
```

### Comparing `stock-indicators-1.2.1/tests/test_dpo.py` & `stock_indicators-1.3.0/tests/test_dpo.py`

 * *Files 17% similar despite different names*

```diff
@@ -28,12 +28,21 @@
     #     q = new_quotes.pop()
     #     assert 2.18214 == round(float(q.close), 5)
         
     def test_bad_data(self, bad_quotes):
         r = indicators.get_dpo(bad_quotes, 5)
         
         assert 502 == len(r)
-        
+
+    def test_condense(self, quotes):
+        results = indicators.get_dpo(quotes, 14).condense()
+
+        assert 489 == len(results)
+
+        last = results.pop()
+        assert   2.1821 == round(float(last.dpo), 4)
+        assert 246.7079 == round(float(last.sma), 4)
+
     def test_exceptions(self, quotes):
         from System import ArgumentOutOfRangeException
         with pytest.raises(ArgumentOutOfRangeException):
             indicators.get_dpo(quotes, 0)
```

### Comparing `stock-indicators-1.2.1/tests/test_elder_ray.py` & `stock_indicators-1.3.0/tests/test_elder_ray.py`

 * *Files 13% similar despite different names*

```diff
@@ -48,12 +48,22 @@
         
         assert 502 - (100 + 13) == len(results)
         
         last = results.pop()
         assert 246.0129 == round(float(last.ema), 4)
         assert -00.4729 == round(float(last.bull_power), 4)
         assert  -3.1429 == round(float(last.bear_power), 4)
-        
+
+    def test_condense(self, quotes):
+        results = indicators.get_elder_ray(quotes, 13).condense()
+
+        assert 490 == len(results)
+
+        last = results.pop()
+        assert 246.0129 == round(float(last.ema), 4)
+        assert -00.4729 == round(float(last.bull_power), 4)
+        assert  -3.1429 == round(float(last.bear_power), 4)
+
     def test_exceptions(self, quotes):
         from System import ArgumentOutOfRangeException
         with pytest.raises(ArgumentOutOfRangeException):
             indicators.get_elder_ray(quotes, 0)
```

### Comparing `stock-indicators-1.2.1/tests/test_ema.py` & `stock_indicators-1.3.0/tests/test_ema.py`

 * *Files 13% similar despite different names*

```diff
@@ -49,11 +49,19 @@
         results = indicators.get_ema(quotes, 20).remove_warmup_periods()
 
         assert 502 - (20 + 100) == len(results)
 
         last = results.pop()
         assert 249.3519 == round(float(last.ema), 4)
 
+    def test_condense(self, quotes):
+        results = indicators.get_ema(quotes, 20).condense()
+
+        assert 483 == len(results)
+
+        last = results.pop()
+        assert 249.3519 == round(float(last.ema), 4)
+
     def test_exceptions(self, quotes):
         from System import ArgumentOutOfRangeException
         with pytest.raises(ArgumentOutOfRangeException):
             indicators.get_ema(quotes, 0)
```

### Comparing `stock-indicators-1.2.1/tests/test_epma.py` & `stock_indicators-1.3.0/tests/test_epma.py`

 * *Files 10% similar despite different names*

```diff
@@ -31,13 +31,20 @@
     def test_removed(self, quotes):
         results = indicators.get_epma(quotes, 20).remove_warmup_periods()
         
         assert 502 - 19 == len(results)
         
         last = results.pop()
         assert 235.8131 == round(float(last.epma), 4)
-        
+
+    def test_condense(self, quotes):
+        results = indicators.get_epma(quotes, 20).condense()
+
+        assert 483 == len(results)
+
+        last = results.pop()
+        assert 235.8131 == round(float(last.epma), 4)
 
     def test_exceptions(self, quotes):
         from System import ArgumentOutOfRangeException
         with pytest.raises(ArgumentOutOfRangeException):
             indicators.get_epma(quotes, 0)
```

### Comparing `stock-indicators-1.2.1/tests/test_fcb.py` & `stock_indicators-1.3.0/tests/test_fcb.py`

 * *Files 10% similar despite different names*

```diff
@@ -42,12 +42,21 @@
         results = indicators.get_fcb(quotes, 2).remove_warmup_periods()
         
         assert 502 - 5 == len(results)
         
         last = results.pop()
         assert 262.47 == round(float(last.upper_band), 2)
         assert 229.42 == round(float(last.lower_band), 2)
-        
+
+    def test_condense(self, quotes):
+        results = indicators.get_fcb(quotes, 2).condense()
+
+        assert 497 == len(results)
+
+        last = results.pop()
+        assert 262.47 == round(float(last.upper_band), 2)
+        assert 229.42 == round(float(last.lower_band), 2)
+
     def test_exceptions(self, quotes):
         from System import ArgumentOutOfRangeException
         with pytest.raises(ArgumentOutOfRangeException):
             indicators.get_fcb(quotes, 1)
```

### Comparing `stock-indicators-1.2.1/tests/test_fisher_transform.py` & `stock_indicators-1.3.0/tests/test_fisher_transform.py`

 * *Files 6% similar despite different names*

```diff
@@ -54,12 +54,21 @@
         
     def test_no_quotes(self, quotes):
         r = indicators.get_fisher_transform([])
         assert 0 == len(r)
         
         r = indicators.get_fisher_transform(quotes[:1])
         assert 1 == len(r)
-        
+
+    def test_condense(self, quotes):
+        results = indicators.get_fisher_transform(quotes, 10).condense()
+
+        assert 502 == len(results)
+
+        last = results.pop()
+        assert -1.2876 == round(float(last.fisher), 4)
+        assert -2.0071 == round(float(last.trigger), 4)
+
     def test_exceptions(self, quotes):
         from System import ArgumentOutOfRangeException
         with pytest.raises(ArgumentOutOfRangeException):
             indicators.get_fisher_transform(quotes, 0)
```

### Comparing `stock-indicators-1.2.1/tests/test_force_index.py` & `stock_indicators-1.3.0/tests/test_force_index.py`

 * *Files 5% similar despite different names*

```diff
@@ -30,12 +30,20 @@
     def test_removed(self, quotes):
         results = indicators.get_force_index(quotes, 13).remove_warmup_periods()
         
         assert 502 - (13 + 100) == len(results)
         
         last = results.pop()
         assert -16824018.428 == round(float(last.force_index), 3)
-        
+
+    def test_condense(self, quotes):
+        results = indicators.get_force_index(quotes, 13).condense()
+
+        assert 489 == len(results)
+
+        last = results.pop()
+        assert -16824018.428 == round(float(last.force_index), 3)
+
     def test_exceptions(self, quotes):
         from System import ArgumentOutOfRangeException
         with pytest.raises(ArgumentOutOfRangeException):
             indicators.get_force_index(quotes, 0)
```

### Comparing `stock-indicators-1.2.1/tests/test_fractal.py` & `stock_indicators-1.3.0/tests/test_fractal.py`

 * *Files 8% similar despite different names*

```diff
@@ -74,11 +74,20 @@
         assert 1 == len(r)
 
     def test_bad_data(self, bad_quotes):
         r = indicators.get_fractal(bad_quotes)
 
         assert 502 == len(r)
 
+    def test_condense(self, quotes):
+        results = indicators.get_fractal(quotes).condense()
+
+        assert 129 == len(results)
+
+        last = results.pop()
+        assert 229.42 == round(float(last.fractal_bull), 2)
+        assert last.fractal_bear is None
+
     def test_exceptions(self, quotes):
         from System import ArgumentOutOfRangeException
         with pytest.raises(ArgumentOutOfRangeException):
             indicators.get_fractal(quotes, 1)
```

### Comparing `stock-indicators-1.2.1/tests/test_gator.py` & `stock_indicators-1.3.0/tests/test_gator.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,7 +88,18 @@
         assert 502 - 150 == len(results)
         
         last = results.pop()
         assert  7.4538 == round(float(last.upper), 4)
         assert -9.2399 == round(float(last.lower), 4)
         assert last.is_upper_expanding == True
         assert last.is_lower_expanding == True
+
+    def test_condense(self, quotes):
+        results = indicators.get_gator(quotes).condense()
+
+        assert 490 == len(results)
+
+        last = results.pop()
+        assert  7.4538 == round(float(last.upper), 4)
+        assert -9.2399 == round(float(last.lower), 4)
+        assert last.is_upper_expanding == True
+        assert last.is_lower_expanding == True
```

### Comparing `stock-indicators-1.2.1/tests/test_heikin_ashi.py` & `stock_indicators-1.3.0/tests/test_heikin_ashi.py`

 * *Files identical despite different names*

### Comparing `stock-indicators-1.2.1/tests/test_hma.py` & `stock_indicators-1.3.0/tests/test_hma.py`

 * *Files 14% similar despite different names*

```diff
@@ -28,12 +28,20 @@
     def test_removed(self, quotes):
         results = indicators.get_hma(quotes, 20).remove_warmup_periods()
         
         assert 480 == len(results)
         
         last = results.pop()
         assert 235.6972 == round(float(last.hma), 4)
-        
+
+    def test_condense(self, quotes):
+        results = indicators.get_hma(quotes, 20).condense()
+
+        assert 480 == len(results)
+
+        last = results.pop()
+        assert 235.6972 == round(float(last.hma), 4)
+
     def test_exceptions(self, quotes):
         from System import ArgumentOutOfRangeException
         with pytest.raises(ArgumentOutOfRangeException):
             indicators.get_hma(quotes, 1)
```

### Comparing `stock-indicators-1.2.1/tests/test_ht_trendline.py` & `stock_indicators-1.3.0/tests/test_ht_trendline.py`

 * *Files 7% similar despite different names*

```diff
@@ -55,15 +55,24 @@
         results = indicators.get_ht_trendline(quotes).remove_warmup_periods()
         
         assert 502 - 100 == len(results)
         
         last = results.pop()
         assert 252.2172 == round(float(last.trendline), 4)
         assert 242.3435 == round(float(last.smooth_price), 4)
-        
+
+    def test_condense(self, quotes):
+        results = indicators.get_ht_trendline(quotes).condense()
+
+        assert 502 == len(results)
+
+        last = results.pop()
+        assert 252.2172 == round(float(last.trendline), 4)
+        assert 242.3435 == round(float(last.smooth_price), 4)
+
     def test_penny_data(self, penny_quotes):
         results = indicators.get_ht_trendline(penny_quotes)
         assert 533 == len(results)
         
     def test_no_quotes(self, quotes):
         r = indicators.get_ht_trendline([])
         assert 0 == len(r)
```

### Comparing `stock-indicators-1.2.1/tests/test_hurst.py` & `stock_indicators-1.3.0/tests/test_hurst.py`

 * *Files 9% similar despite different names*

```diff
@@ -38,11 +38,19 @@
         results = results.remove_warmup_periods()
 
         assert 1 == len(results)
 
         last  = results.pop()
         assert 0.483563 == round(float(last.hurst_exponent), 6)
 
+    def test_condense(self, longest_quotes):
+        results = indicators.get_hurst(longest_quotes, len(longest_quotes) - 1).condense()
+
+        assert 1 == len(results)
+
+        last  = results.pop()
+        assert 0.483563 == round(float(last.hurst_exponent), 6)
+
     def test_exceptions(self, quotes):
         from System import ArgumentOutOfRangeException
         with pytest.raises(ArgumentOutOfRangeException):
             indicators.get_hurst(quotes, 19)
```

### Comparing `stock-indicators-1.2.1/tests/test_ichimoku.py` & `stock_indicators-1.3.0/tests/test_ichimoku.py`

 * *Files 13% similar despite different names*

```diff
@@ -51,14 +51,26 @@
     def test_no_quotes(self, quotes):
         r = indicators.get_ichimoku([])
         assert 0 == len(r)
         
         r = indicators.get_ichimoku(quotes[:1])
         assert 1 == len(r)
 
+    def test_condense(self, quotes):
+        results = indicators.get_ichimoku(quotes, 9, 26, 52).condense()
+
+        assert 502 == len(results)
+
+        last = results.pop()
+        assert 241.2600 == round(float(last.tenkan_sen), 4)
+        assert 251.5050 == round(float(last.kijun_sen), 4)
+        assert 264.7700 == round(float(last.senkou_span_a), 4)
+        assert 269.8200 == round(float(last.senkou_span_b), 4)
+        assert last.chikou_span is None
+
     def test_exceptions(self, quotes):
         from System import ArgumentOutOfRangeException
         with pytest.raises(ArgumentOutOfRangeException):
             indicators.get_ichimoku(quotes, 0)
 
         with pytest.raises(ArgumentOutOfRangeException):
             indicators.get_ichimoku(quotes, 9, 0, 52)
```

### Comparing `stock-indicators-1.2.1/tests/test_kama.py` & `stock_indicators-1.3.0/tests/test_kama.py`

 * *Files 5% similar despite different names*

```diff
@@ -55,15 +55,23 @@
         
         results = indicators.get_kama(quotes, er_periods, fast_periods, slow_periods)
         results = results.remove_warmup_periods()
         
         assert 502 - max(er_periods + 100, er_periods * 10) == len(results)
         
         last = results.pop()
-        
+        assert   0.2214 == round(float(last.efficiency_ratio), 4)
+        assert 240.1138 == round(float(last.kama), 4)
+
+    def test_condense(self, quotes):
+        results = indicators.get_kama(quotes, 10, 2, 30).condense()
+
+        assert 493 == len(results)
+
+        last = results.pop()
         assert   0.2214 == round(float(last.efficiency_ratio), 4)
         assert 240.1138 == round(float(last.kama), 4)
 
     def test_exceptions(self, quotes):
         from System import ArgumentOutOfRangeException
         with pytest.raises(ArgumentOutOfRangeException):
             indicators.get_kama(quotes, 0, 2, 30)
```

### Comparing `stock-indicators-1.2.1/tests/test_keltner.py` & `stock_indicators-1.3.0/tests/test_keltner.py`

 * *Files 4% similar despite different names*

```diff
@@ -54,15 +54,26 @@
         assert 502 - max(2 * n, n + 100) == len(results)
         
         last = results.pop()
         assert 262.1873 == round(float(last.upper_band), 4)
         assert 249.3519 == round(float(last.center_line), 4)
         assert 236.5165 == round(float(last.lower_band), 4)
         assert 0.102950 == round(float(last.width), 6)
-        
+
+    def test_condense(self, quotes):
+        results = indicators.get_keltner(quotes, 20, 2, 10).condense()
+
+        assert 483 == len(results)
+
+        last = results.pop()
+        assert 262.1873 == round(float(last.upper_band), 4)
+        assert 249.3519 == round(float(last.center_line), 4)
+        assert 236.5165 == round(float(last.lower_band), 4)
+        assert 0.102950 == round(float(last.width), 6)
+
     def test_exceptions(self, quotes):
         from System import ArgumentOutOfRangeException
         with pytest.raises(ArgumentOutOfRangeException):
             indicators.get_keltner(quotes, 1, 2, 10)
             
         with pytest.raises(ArgumentOutOfRangeException):
             indicators.get_keltner(quotes, 20, 2, 1)
```

### Comparing `stock-indicators-1.2.1/tests/test_kvo.py` & `stock_indicators-1.3.0/tests/test_kvo.py`

 * *Files 4% similar despite different names*

```diff
@@ -53,15 +53,24 @@
         results = indicators.get_kvo(quotes, 34, 55, 13).remove_warmup_periods()
         
         assert 502 - (55 + 150) == len(results)
         
         last = results.pop()
         assert  -539224047 == round(float(last.oscillator), 0)
         assert -1548306127 == round(float(last.signal), 0)
-        
+
+    def test_condense(self, quotes):
+        results = indicators.get_kvo(quotes, 34, 55, 13).condense()
+
+        assert 446 == len(results)
+
+        last = results.pop()
+        assert  -539224047 == round(float(last.oscillator), 0)
+        assert -1548306127 == round(float(last.signal), 0)
+
     def test_exceptions(self, quotes):
         from System import ArgumentOutOfRangeException
         with pytest.raises(ArgumentOutOfRangeException):
             indicators.get_kvo(quotes, 2)
         
         with pytest.raises(ArgumentOutOfRangeException):
             indicators.get_kvo(quotes, 20, 20)
```

### Comparing `stock-indicators-1.2.1/tests/test_ma_envelopes.py` & `stock_indicators-1.3.0/tests/test_ma_envelopes.py`

 * *Files 2% similar despite different names*

```diff
@@ -203,14 +203,24 @@
 
         r = indicators.get_ma_envelopes(bad_quotes, 5, 2.5, MAType.TEMA)
         assert 502 == len(r)
 
         r = indicators.get_ma_envelopes(bad_quotes, 5, 2.5, MAType.WMA)
         assert 502 == len(r)
 
+    def test_condense(self, quotes):
+        results = indicators.get_ma_envelopes(quotes, 10, 2.5, MAType.ALMA).condense()
+
+        assert 493 == len(results)
+
+        last = results.pop()
+        assert 242.1871 == round(float(last.center_line), 4)
+        assert 248.2418 == round(float(last.upper_envelope), 4)
+        assert 236.1324 == round(float(last.lower_envelope), 4)
+
     def test_exceptions(self, quotes):
         from System import ArgumentOutOfRangeException
         with pytest.raises(ArgumentOutOfRangeException):
             indicators.get_ma_envelopes(quotes, 14, 0)
 
         with pytest.raises(ArgumentOutOfRangeException):
             indicators.get_ma_envelopes(quotes, 14, 5, MAType.KAMA)
```

### Comparing `stock-indicators-1.2.1/tests/test_macd.py` & `stock_indicators-1.3.0/tests/test_macd.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,14 +41,24 @@
         assert 502 - (26 + 9 + 250) == len(results)
 
         last = results.pop()
         assert -6.2198 == round(float(last.macd), 4)
         assert -5.8569 == round(float(last.signal), 4)
         assert -0.3629 == round(float(last.histogram), 4)
 
+    def test_condense(self, quotes):
+        results = indicators.get_macd(quotes, 12, 26, 9).condense()
+
+        assert 477 == len(results)
+
+        last = results.pop()
+        assert -6.2198 == round(float(last.macd), 4)
+        assert -5.8569 == round(float(last.signal), 4)
+        assert -0.3629 == round(float(last.histogram), 4)
+
     def test_exceptions(self, quotes):
         from System import ArgumentOutOfRangeException
         with pytest.raises(ArgumentOutOfRangeException):
             indicators.get_macd(quotes, 0, 26, 9)
 
         with pytest.raises(ArgumentOutOfRangeException):
             indicators.get_macd(quotes, 12, 12, 9)
```

### Comparing `stock-indicators-1.2.1/tests/test_mama.py` & `stock_indicators-1.3.0/tests/test_mama.py`

 * *Files 12% similar despite different names*

```diff
@@ -44,23 +44,31 @@
         r = indicators.get_mama([])
         assert 0 == len(r)
         
         r = indicators.get_mama(quotes[:1])
         assert 1 == len(r)
         
     def test_removed(self, quotes):
-        results = indicators.get_mama(quotes, 0.5, 0.05)
-        results = results.remove_warmup_periods()
+        results = indicators.get_mama(quotes, 0.5, 0.05).remove_warmup_periods()
         
         assert 502 - 50 == len(results)
         
         last = results.pop()        
         assert 244.1092 == round(float(last.mama), 4)
         assert 252.6139 == round(float(last.fama), 4)
-        
+
+    def test_condense(self, quotes):
+        results = indicators.get_mama(quotes, 0.5, 0.05).condense()
+
+        assert 497 == len(results)
+
+        last = results.pop()        
+        assert 244.1092 == round(float(last.mama), 4)
+        assert 252.6139 == round(float(last.fama), 4)
+
     def test_exceptions(self, quotes):
         from System import ArgumentOutOfRangeException
         with pytest.raises(ArgumentOutOfRangeException):
             indicators.get_mama(quotes, 0.5, 0.5)
         
         with pytest.raises(ArgumentOutOfRangeException):
             indicators.get_mama(quotes, 1, 0.5)
```

### Comparing `stock-indicators-1.2.1/tests/test_marubozu.py` & `stock_indicators-1.3.0/tests/test_marubozu.py`

 * *Files identical despite different names*

### Comparing `stock-indicators-1.2.1/tests/test_mfi.py` & `stock_indicators-1.3.0/tests/test_mfi.py`

 * *Files 3% similar despite different names*

```diff
@@ -40,12 +40,20 @@
     def test_removed(self, quotes):
         results = indicators.get_mfi(quotes, 14).remove_warmup_periods()
         
         assert 502 - 14 == len(results)
         
         last = results.pop()
         assert 39.9494 == round(float(last.mfi), 4)
-        
+
+    def test_condense(self, quotes):
+        results = indicators.get_mfi(quotes, 14).condense()
+
+        assert 488 == len(results)
+
+        last = results.pop()
+        assert 39.9494 == round(float(last.mfi), 4)
+
     def test_exceptions(self, quotes):
         from System import ArgumentOutOfRangeException
         with pytest.raises(ArgumentOutOfRangeException):
             indicators.get_mfi(quotes, 1)
```

### Comparing `stock-indicators-1.2.1/tests/test_obv.py` & `stock_indicators-1.3.0/tests/test_obv.py`

 * *Files 13% similar despite different names*

```diff
@@ -47,12 +47,21 @@
         
     def test_no_quotes(self, quotes):
         r = indicators.get_obv([])
         assert 0 == len(r)
         
         r = indicators.get_obv(quotes[:1])
         assert 1 == len(r)
-        
+
+    def test_condense(self, quotes):
+        results = indicators.get_obv(quotes).condense()
+
+        assert 502 == len(results)
+
+        last = results.pop()
+        assert 539843504 == last.obv
+        assert last.obv_sma is None
+
     def test_exceptions(self, quotes):
         from System import ArgumentOutOfRangeException
         with pytest.raises(ArgumentOutOfRangeException):
             indicators.get_obv(quotes, 0)
```

### Comparing `stock-indicators-1.2.1/tests/test_parabolic_sar.py` & `stock_indicators-1.3.0/tests/test_parabolic_sar.py`

 * *Files 3% similar despite different names*

```diff
@@ -63,15 +63,24 @@
         results = indicators.get_parabolic_sar(quotes, 0.02, 0.2).remove_warmup_periods()
         
         assert 488 == len(results)
         
         last = results.pop()
         assert 229.7662 == round(float(last.sar), 4)
         assert False == last.is_reversal
-        
+
+    def test_condense(self, quotes):
+        results = indicators.get_parabolic_sar(quotes, 0.02, 0.2).condense()
+
+        assert 488 == len(results)
+
+        last = results.pop()
+        assert 229.7662 == round(float(last.sar), 4)
+        assert False == last.is_reversal
+
     def test_exceptions(self, quotes):
         from System import ArgumentOutOfRangeException
         with pytest.raises(ArgumentOutOfRangeException):
             indicators.get_parabolic_sar(quotes, 0, 1)
 
         with pytest.raises(ArgumentOutOfRangeException):
             indicators.get_parabolic_sar(quotes, 0.02, 0)
```

### Comparing `stock-indicators-1.2.1/tests/test_pivot_points.py` & `stock_indicators-1.3.0/tests/test_pivot_points.py`

 * *Files identical despite different names*

### Comparing `stock-indicators-1.2.1/tests/test_pivots.py` & `stock_indicators-1.3.0/tests/test_pivots.py`

 * *Files 10% similar despite different names*

```diff
@@ -84,15 +84,28 @@
         
     def test_no_quotes(self, quotes):
         r = indicators.get_pivots([])
         assert 0 == len(r)
         
         r = indicators.get_pivots(quotes[:1])
         assert 1 == len(r)
-    
+
+    def test_condense(self, quotes):
+        results = indicators.get_pivots(quotes, 4, 4, 20, EndType.HIGH_LOW).condense()
+
+        assert 67 == len(results)
+
+        r = results.pop()
+        assert r.high_point is None
+        assert r.high_trend is None
+        assert r.high_line is None
+        assert 252.34 == float(round(r.low_point, 2))
+        assert r.low_trend == PivotTrend.LL
+        assert 252.34 == float(round(r.low_line, 2))
+
     def test_exceptions(self, quotes):
         from System import ArgumentOutOfRangeException
         with pytest.raises(ArgumentOutOfRangeException):
             indicators.get_pivots(quotes, 1)
             
         with pytest.raises(ArgumentOutOfRangeException):
             indicators.get_pivots(quotes, 2, 1)
```

### Comparing `stock-indicators-1.2.1/tests/test_pmo.py` & `stock_indicators-1.3.0/tests/test_pmo.py`

 * *Files 11% similar despite different names*

```diff
@@ -32,15 +32,24 @@
         results = indicators.get_pmo(quotes, 35, 20, 10).remove_warmup_periods()
         
         assert 502 - (35 + 20 + 250) == len(results)   
         
         last = results.pop()
         assert -2.7016 == round(float(last.pmo), 4)
         assert -2.3117 == round(float(last.signal), 4)
-           
+
+    def test_condense(self, quotes):
+        results = indicators.get_pmo(quotes, 35, 20, 10).condense()
+
+        assert 448 == len(results)
+
+        last = results.pop()
+        assert -2.7016 == round(float(last.pmo), 4)
+        assert -2.3117 == round(float(last.signal), 4)
+
     def test_exceptions(self, quotes):
         from System import ArgumentOutOfRangeException
         with pytest.raises(ArgumentOutOfRangeException):
             indicators.get_pmo(quotes, 1)
             
         with pytest.raises(ArgumentOutOfRangeException):
             indicators.get_pmo(quotes, 5, 0)
```

### Comparing `stock-indicators-1.2.1/tests/test_prs.py` & `stock_indicators-1.3.0/tests/test_prs.py`

 * *Files 7% similar despite different names*

```diff
@@ -30,15 +30,25 @@
         
     def test_no_quotes(self, quotes):
         r = indicators.get_prs([], [])
         assert 0 == len(r)
         
         r = indicators.get_prs(quotes[:1], quotes[:1])
         assert 1 == len(r)
-        
+
+    def test_condense(self, quotes, other_quotes):
+        results = indicators.get_prs(other_quotes, quotes, 30, 10).condense()
+
+        assert 502 == len(results)
+
+        last = results.pop()
+        assert 1.356817 == round(float(last.prs), 6)
+        assert 1.343445 == round(float(last.prs_sma), 6)
+        assert 0.037082 == round(float(last.prs_percent), 6) 
+
     def test_exceptions(self, quotes, other_quotes, mismatch_quotes):
         from System import ArgumentOutOfRangeException
         with pytest.raises(ArgumentOutOfRangeException):
             indicators.get_prs(quotes, other_quotes, 0)
             
         with pytest.raises(ArgumentOutOfRangeException):
             indicators.get_prs(quotes, other_quotes, 14, 0)
```

### Comparing `stock-indicators-1.2.1/tests/test_pvo.py` & `stock_indicators-1.3.0/tests/test_pvo.py`

 * *Files 9% similar despite different names*

```diff
@@ -56,15 +56,25 @@
         
         assert 502 - (slow_periods + signal_periods + 250) == len(results)
         
         last = results.pop()
         assert 10.4395 == float(round(last.pvo, 4))
         assert 12.2681 == float(round(last.signal, 4))
         assert -1.8286 == float(round(last.histogram, 4))
-                
+
+    def test_condense(self, quotes):
+        results = indicators.get_pvo(quotes, 12, 26, 9).condense()
+
+        assert 477 == len(results)
+
+        last = results.pop()
+        assert 10.4395 == float(round(last.pvo, 4))
+        assert 12.2681 == float(round(last.signal, 4))
+        assert -1.8286 == float(round(last.histogram, 4))
+
     def test_exceptions(self, quotes):
         from System import ArgumentOutOfRangeException
         with pytest.raises(ArgumentOutOfRangeException):
             indicators.get_pvo(quotes, 0, 26, 9)
             
         with pytest.raises(ArgumentOutOfRangeException):
             indicators.get_pvo(quotes, 12, 12, 9)
```

### Comparing `stock-indicators-1.2.1/tests/test_renko.py` & `stock_indicators-1.3.0/tests/test_renko.py`

 * *Files identical despite different names*

### Comparing `stock-indicators-1.2.1/tests/test_roc.py` & `stock_indicators-1.3.0/tests/test_roc.py`

 * *Files 4% similar despite different names*

```diff
@@ -49,14 +49,23 @@
         
         assert 502 - 20 == len(results)
         
         last = results.pop()
         assert -8.2482 == round(float(last.roc), 4)
         assert last.roc_sma is None
 
+    def test_condense(self, quotes):
+        results = indicators.get_roc(quotes, 20).condense()
+
+        assert 482 == len(results)
+
+        last = results.pop()
+        assert -8.2482 == round(float(last.roc), 4)
+        assert last.roc_sma is None
+
     def test_exceptions(self, quotes):
         from System import ArgumentOutOfRangeException
         with pytest.raises(ArgumentOutOfRangeException):
             indicators.get_roc(quotes, 0)
             
         with pytest.raises(ArgumentOutOfRangeException):
             indicators.get_roc(quotes, 14, 0)
```

### Comparing `stock-indicators-1.2.1/tests/test_rolling_pivots.py` & `stock_indicators-1.3.0/tests/test_rolling_pivots.py`

 * *Files identical despite different names*

### Comparing `stock-indicators-1.2.1/tests/test_rsi.py` & `stock_indicators-1.3.0/tests/test_rsi.py`

 * *Files 12% similar despite different names*

```diff
@@ -52,11 +52,19 @@
         results = indicators.get_rsi(quotes, 14).remove_warmup_periods()
 
         assert 502 - (10 * 14) == len(results)
 
         last = results.pop()
         assert 42.0773 == round(float(last.rsi), 4)
 
+    def test_condense(self, quotes):
+        results = indicators.get_rsi(quotes, 14).condense()
+
+        assert 488 == len(results)
+
+        last = results.pop()
+        assert 42.0773 == round(float(last.rsi), 4)
+
     def test_exceptions(self, quotes):
         from System import ArgumentOutOfRangeException
         with pytest.raises(ArgumentOutOfRangeException):
             indicators.get_rsi(quotes, 0)
```

### Comparing `stock-indicators-1.2.1/tests/test_slope.py` & `stock_indicators-1.3.0/tests/test_slope.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,12 +41,24 @@
         
         last = results.pop()
         assert -1.689143 == round(float(last.slope), 6)
         assert 1083.7629 == round(float(last.intercept), 4)
         assert 0000.7955 == round(float(last.r_squared), 4)
         assert   10.9202 == round(float(last.stdev), 4)
         assert  235.8131 == round(float(last.line), 4)
-        
+
+    def test_condense(self, quotes):
+        results = indicators.get_slope(quotes, 20).condense()
+
+        assert 483 == len(results)
+
+        last = results.pop()
+        assert -1.689143 == round(float(last.slope), 6)
+        assert 1083.7629 == round(float(last.intercept), 4)
+        assert 0000.7955 == round(float(last.r_squared), 4)
+        assert   10.9202 == round(float(last.stdev), 4)
+        assert  235.8131 == round(float(last.line), 4)
+
     def test_exceptions(self, quotes):
         from System import ArgumentOutOfRangeException
         with pytest.raises(ArgumentOutOfRangeException):
             indicators.get_slope(quotes, 0)
```

### Comparing `stock-indicators-1.2.1/tests/test_sma.py` & `stock_indicators-1.3.0/tests/test_sma.py`

 * *Files 4% similar despite different names*

```diff
@@ -64,11 +64,17 @@
 
     def test_removed(self, quotes):
         results = indicators.get_sma(quotes, 20).remove_warmup_periods()
 
         assert 502 - 19 == len(results)
         assert 251.8600 == round(float(results[len(results)-1].sma), 4)
 
+    def test_condense(self, quotes):
+        results = indicators.get_sma(quotes, 20).condense()
+
+        assert 483 == len(results)
+        assert 251.8600 == round(float(results[len(results)-1].sma), 4)
+
     def test_exceptions(self, quotes):
         from System import ArgumentOutOfRangeException
         with pytest.raises(ArgumentOutOfRangeException):
             indicators.get_sma(quotes, 0)
```

### Comparing `stock-indicators-1.2.1/tests/test_sma_extended.py` & `stock_indicators-1.3.0/tests/test_dema.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,47 +1,43 @@
 import pytest
 from stock_indicators import indicators
-from stock_indicators._cslib import CsDecimal
 
-class TestSMAExtended:
-    def test_result_types(self, quotes):
-        results = indicators.get_sma_analysis(quotes, 20)
+class TestDoubleEMA:
+    def test_standard(self, quotes):
+        results = indicators.get_dema(quotes, 20)
         
-        # Sample value.
-        r = results[501]
-        assert     float == type(r._csdata.Sma)
-        assert     float == type(r._csdata.Mad)
-        assert     float == type(r._csdata.Mse)
-        assert     float == type(r._csdata.Mape)
-
-    def test_extended(self, quotes):
-        results = indicators.get_sma_analysis(quotes, 20)
-
-        # proper quantities.
-        # should always be the same number of results as there is quotes.
         assert 502 == len(results)
-        assert 483 == len(list(filter(lambda x: x.sma is not None, results)))
-
-        # Sample value.
+        assert 483 == len(list(filter(lambda x: x.dema is not None, results)))
+        
+        r = results[51]
+        assert 225.8259 == round(float(r.dema), 4)
+        
+        r = results[249]
+        assert 258.4452 == round(float(r.dema), 4)
+        
         r = results[501]
-        assert 251.8600 == round(float(r.sma), 4)
-        assert 9.4500   == round(float(r.mad), 4)
-        assert 119.2510 == round(float(r.mse), 4)
-        assert 0.037637 == round(float(r.mape), 6)
-
+        assert 241.1677 == round(float(r.dema), 4)
+        
     def test_bad_data(self, bad_quotes):
-        results = indicators.get_sma_analysis(bad_quotes, 15)
+        r = indicators.get_dema(bad_quotes, 15)
+        assert 502 == len(r)
+        
+    def test_removed(self, quotes):
+        results = indicators.get_dema(quotes, 20).remove_warmup_periods()
+        
+        assert 502 - (2 * 20 + 100) == len(results)
+        
+        last = results.pop()
+        assert 241.1677 == round(float(last.dema), 4)
 
-        # Assertions 
-        assert 502 == len(results)
+    def test_condense(self, quotes):
+        results = indicators.get_dema(quotes, 20).condense()
 
-    def test_removed(self, quotes):
-        results = indicators.get_sma_analysis(quotes, 20).remove_warmup_periods()
+        assert 483 == len(results)
 
-        # Assertions
-        assert 502 - 19 == len(results)
-        assert 251.8600 == round(float(results[len(results)-1].sma), 4)
+        last = results.pop()
+        assert 241.1677 == round(float(last.dema), 4)
 
     def test_exceptions(self, quotes):
         from System import ArgumentOutOfRangeException
         with pytest.raises(ArgumentOutOfRangeException):
-            indicators.get_sma_analysis(quotes, 0)
+            indicators.get_dema(quotes, 0)
```

### Comparing `stock-indicators-1.2.1/tests/test_smi.py` & `stock_indicators-1.3.0/tests/test_smi.py`

 * *Files 5% similar despite different names*

```diff
@@ -76,15 +76,24 @@
         results = indicators.get_smi(quotes, 14, 20, 5, 3).remove_warmup_periods()
         
         assert 501 - (14 + 100) == len(results)   
         
         last = results.pop()
         assert -52.6560 == round(float(last.smi), 4)
         assert -54.1903 == round(float(last.signal), 4)
-           
+
+    def test_condense(self, quotes):
+        results = indicators.get_smi(quotes, 14, 20, 5, 3).condense()
+
+        assert 489 == len(results)
+
+        last = results.pop()
+        assert -52.6560 == round(float(last.smi), 4)
+        assert -54.1903 == round(float(last.signal), 4)
+
     def test_exceptions(self, quotes):
         from System import ArgumentOutOfRangeException
         with pytest.raises(ArgumentOutOfRangeException):
             indicators.get_smi(quotes, 0, 5, 5, 5)
             
         with pytest.raises(ArgumentOutOfRangeException):
             indicators.get_smi(quotes, 14, 0, 5, 5)
```

### Comparing `stock-indicators-1.2.1/tests/test_smma.py` & `stock_indicators-1.3.0/tests/test_tema.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,54 +1,43 @@
 import pytest
 from stock_indicators import indicators
 
-class TestSMMA:
+class TestTripleEMA:
     def test_standard(self, quotes):
-        results = indicators.get_smma(quotes, 20)
-        
+        results = indicators.get_tema(quotes, 20)
+
         assert 502 == len(results)
-        assert 483 == len(list(filter(lambda x: x.smma is not None, results)))
-        
-        r = results[18]
-        assert r.smma is None
-        
-        r = results[19]
-        assert r.smma is not None
-        
-        r = results[19]
-        assert 214.52500 == round(float(r.smma), 5)
-        
-        r = results[20]
-        assert 214.55125 == round(float(r.smma), 5)
-        
-        r = results[21]
-        assert 214.58319 == round(float(r.smma), 5)
-        
-        r = results[100]
-        assert 225.78071 == round(float(r.smma), 5)
-        
+        assert 483 == len(list(filter(lambda x: x.tema is not None, results)))
+
+        r = results[67]
+        assert 222.9562 == round(float(r.tema), 4)
+
+        r = results[249]
+        assert 258.6208 == round(float(r.tema), 4)
+
         r = results[501]
-        assert 255.67462 == round(float(r.smma), 5)
-       
+        assert 238.7690 == round(float(r.tema), 4)
+
     def test_bad_data(self, bad_quotes):
-        r = indicators.get_smma(bad_quotes, 15)
+        r = indicators.get_tema(bad_quotes, 15)
         assert 502 == len(r)
-        
-    def test_no_quotes(self, quotes):
-        r = indicators.get_smma([], 5)
-        assert 0 == len(r)
-        
-        r = indicators.get_smma(quotes[:1], 5)
-        assert 1 == len(r)
-        
+
     def test_removed(self, quotes):
-        results = indicators.get_smma(quotes, 20).remove_warmup_periods()
-        
-        assert 502 - (20 + 100) == len(results)
-        
+        results = indicators.get_tema(quotes, 20).remove_warmup_periods()
+
+        assert 502 - (3 * 20 + 100) == len(results)
+
+        last = results.pop()
+        assert 238.7690 == round(float(last.tema), 4)
+
+    def test_condense(self, quotes):
+        results = indicators.get_tema(quotes, 20).condense()
+
+        assert 483 == len(results)
+
         last = results.pop()
-        assert 255.67462 == round(float(last.smma), 5)
-        
-    def test_exceptions(self, quotes, other_quotes, mismatch_quotes):
+        assert 238.7690 == round(float(last.tema), 4)
+
+    def test_exceptions(self, quotes):
         from System import ArgumentOutOfRangeException
         with pytest.raises(ArgumentOutOfRangeException):
-            indicators.get_smma(quotes, 0)
+            indicators.get_tema(quotes, 0)
```

### Comparing `stock-indicators-1.2.1/tests/test_starc_bands.py` & `stock_indicators-1.3.0/tests/test_starc_bands.py`

 * *Files 8% similar despite different names*

```diff
@@ -65,14 +65,24 @@
         assert 502 - (lookback_periods + 150) == len(results)
 
         last = results.pop()
         assert 251.8600 == round(float(last.center_line), 4)
         assert 264.1595 == round(float(last.upper_band), 4)
         assert 239.5605 == round(float(last.lower_band), 4)
 
+    def test_condense(self, quotes):
+        results = indicators.get_starc_bands(quotes, 20, 2, 14).condense()
+
+        assert 483 == len(results)
+
+        last = results.pop()
+        assert 251.8600 == round(float(last.center_line), 4)
+        assert 264.1595 == round(float(last.upper_band), 4)
+        assert 239.5605 == round(float(last.lower_band), 4)
+
     def test_exceptions(self, quotes):
         from System import ArgumentOutOfRangeException
         with pytest.raises(ArgumentOutOfRangeException):
             indicators.get_starc_bands(quotes, 1, 2, 10)
 
         with pytest.raises(ArgumentOutOfRangeException):
             indicators.get_starc_bands(quotes, 20, 2, 1)
```

### Comparing `stock-indicators-1.2.1/tests/test_stc.py` & `stock_indicators-1.3.0/tests/test_stc.py`

 * *Files 8% similar despite different names*

```diff
@@ -41,15 +41,23 @@
         slow_periods = 26
         
         results = indicators.get_stc(quotes, cycle_periods, fast_periods, slow_periods)
         results = results.remove_warmup_periods()
         
         last = results.pop()
         assert 19.2544 == round(float(last.stc), 4)
-    
+
+    def test_condense(self, quotes):
+        results = indicators.get_stc(quotes, 9, 12, 26).condense()
+
+        assert 467 == len(results)
+
+        last = results.pop()
+        assert 19.2544 == round(float(last.stc), 4)
+
     def test_exceptions(self, quotes, other_quotes, mismatch_quotes):
         from System import ArgumentOutOfRangeException
         with pytest.raises(ArgumentOutOfRangeException):
             indicators.get_stc(quotes, 9, 0, 26)
             
         with pytest.raises(ArgumentOutOfRangeException):
             indicators.get_stc(quotes, 9, 12, 12)
```

### Comparing `stock-indicators-1.2.1/tests/test_stdev.py` & `stock_indicators-1.3.0/tests/test_stdev.py`

 * *Files 15% similar despite different names*

```diff
@@ -73,15 +73,26 @@
         assert 502 - 9 == len(results)
         
         last = results.pop()
         assert   5.4738 == round(float(last.stdev), 4)
         assert 242.4100 == round(float(last.mean), 4)
         assert 0.524312 == round(float(last.z_score), 6)
         assert last.stdev_sma is None
-        
+
+    def test_condense(self, quotes):
+        results = indicators.get_stdev(quotes, 10).condense()
+
+        assert 493 == len(results)
+
+        last = results.pop()
+        assert   5.4738 == round(float(last.stdev), 4)
+        assert 242.4100 == round(float(last.mean), 4)
+        assert 0.524312 == round(float(last.z_score), 6)
+        assert last.stdev_sma is None
+
     def test_exceptions(self, quotes):
         from System import ArgumentOutOfRangeException
         with pytest.raises(ArgumentOutOfRangeException):
             indicators.get_stdev(quotes, 1)
 
         with pytest.raises(ArgumentOutOfRangeException):
             indicators.get_stdev(quotes, 14,0)
```

### Comparing `stock-indicators-1.2.1/tests/test_stdev_channels.py` & `stock_indicators-1.3.0/tests/test_stdev_channels.py`

 * *Files 4% similar despite different names*

```diff
@@ -87,15 +87,26 @@
         assert 500 == len(results)
         
         last = results.pop()
         assert 235.8131 == round(float(last.center_line), 4)
         assert 257.6536 == round(float(last.upper_channel), 4)
         assert 213.9727 == round(float(last.lower_channel), 4)
         assert last.break_point is False
-    
+
+    def test_condense(self, quotes):
+        results = indicators.get_stdev_channels(quotes, 20, 2).condense()
+
+        assert 500 == len(results)
+
+        last = results.pop()
+        assert 235.8131 == round(float(last.center_line), 4)
+        assert 257.6536 == round(float(last.upper_channel), 4)
+        assert 213.9727 == round(float(last.lower_channel), 4)
+        assert last.break_point is False
+
     def test_exceptions(self, quotes):
         from System import ArgumentOutOfRangeException
         with pytest.raises(ArgumentOutOfRangeException):
             indicators.get_stdev_channels(quotes, 0)
 
         with pytest.raises(ArgumentOutOfRangeException):
             indicators.get_stdev_channels(quotes, 20,0)
```

### Comparing `stock-indicators-1.2.1/tests/test_stoch.py` & `stock_indicators-1.3.0/tests/test_trix.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,92 +1,55 @@
 import pytest
 from stock_indicators import indicators
 
-class TestStoch:
+class TestTRIX:
     def test_standard(self, quotes):
-        results = indicators.get_stoch(quotes, 14, 3, 3)
-        
-        assert 502 == len(results)
-        assert 487 == len(list(filter(lambda x: x.oscillator is not None, results)))
-        assert 485 == len(list(filter(lambda x: x.signal is not None, results)))
+        results = indicators.get_trix(quotes, 20, 5)
 
-        r = results[15]
-        assert 81.1253 == round(float(r.oscillator), 4)
-        assert r.signal is None
-        assert r.percent_j is None
-
-        r = results[17]
-        assert 92.1307 == round(float(r.oscillator), 4)
-        assert 88.4995 == round(float(r.signal), 4)
-        assert 99.3929 == round(float(r.percent_j), 4)
-
-        r = results[149]
-        assert 81.6870 == round(float(r.oscillator), 4)
-        assert 79.7935 == round(float(r.signal), 4)
-        assert 85.4741 == round(float(r.percent_j), 4)
+        assert 502 == len(results)
+        assert 482 == len(list(filter(lambda x: x.ema3 is not None, results)))
+        assert 482 == len(list(filter(lambda x: x.trix is not None, results)))
+        assert 478 == len(list(filter(lambda x: x.signal is not None, results)))
+
+        r = results[67]
+        assert 221.7837 == round(float(r.ema3), 4)
+        assert 0.050030 == round(float(r.trix), 6)
+        assert 0.057064 == round(float(r.signal), 6)
 
         r = results[249]
-        assert 83.2020 == round(float(r.oscillator), 4)
-        assert 83.0813 == round(float(r.signal), 4)
-        assert 83.4435 == round(float(r.percent_j), 4)
-
-        r = results[501]
-        assert 43.1353 == round(float(r.oscillator), 4)
-        assert 35.5674 == round(float(r.signal), 4)
-        assert 58.2712 == round(float(r.percent_j), 4)
-
-    def test_no_signal(self, quotes):
-        results = indicators.get_stoch(quotes, 5, 1, 3)
-
-        r = results[487]
-        assert r.oscillator == r.signal
-        assert r.k == r.d
-
-        r = results[501]
-        assert r.oscillator == r.signal
-        assert r.k == r.d
-
-    def test_fast(self, quotes):
-        results = indicators.get_stoch(quotes, 5, 10, 1)
-
-        r = results[487]
-        assert 25.0353 == round(float(r.oscillator), 4)
-        assert 60.5706 == round(float(r.signal), 4)
+        assert 249.4469 == round(float(r.ema3), 4)
+        assert 0.121781 == round(float(r.trix), 6)
+        assert 0.119769 == round(float(r.signal), 6)
 
         r = results[501]
-        assert 91.6233 == round(float(r.oscillator), 4)
-        assert 36.0608 == round(float(r.signal), 4)
-
-
-    def test_fast_small(self, quotes):
-        results = indicators.get_stoch(quotes, 1, 10, 1)
-
-        r = results[70]
-        assert 0 == round(float(r.oscillator), 4)
-
-        r = results[71]
-        assert 100 == round(float(r.oscillator), 4)
+        assert  263.3216 == round(float(r.ema3), 4)
+        assert -0.230742 == round(float(r.trix), 6)
+        assert -0.204536 == round(float(r.signal), 6)
 
     def test_bad_data(self, bad_quotes):
-        r = indicators.get_stoch(bad_quotes, 15)
+        r = indicators.get_trix(bad_quotes, 15, 2)
         assert 502 == len(r)
 
     def test_removed(self, quotes):
-        results = indicators.get_stoch(quotes, 14, 3, 3).remove_warmup_periods()
+        results = indicators.get_trix(quotes, 20, 5).remove_warmup_periods()
 
-        assert 502 - (14 + 3 - 2) == len(results)
+        assert 502 - ((3 * 20) + 100) == len(results)
 
         last = results.pop()
-        assert 43.1353 == round(float(last.oscillator), 4)
-        assert 35.5674 == round(float(last.signal), 4)
-        assert 58.2712 == round(float(last.percent_j), 4)
+        assert  263.3216 == round(float(last.ema3), 4)
+        assert -0.230742 == round(float(last.trix), 6)
+        assert -0.204536 == round(float(last.signal), 6)
 
-    def test_exceptions(self, quotes):
-        from System import ArgumentOutOfRangeException
-        with pytest.raises(ArgumentOutOfRangeException):
-            indicators.get_stoch(quotes, 0)
+    def test_condense(self, quotes):
+        results = indicators.get_trix(quotes, 20, 5).condense()
 
-        with pytest.raises(ArgumentOutOfRangeException):
-            indicators.get_stoch(quotes, 14, 0)
+        assert 482 == len(results)
+
+        last = results.pop()
+        assert  263.3216 == round(float(last.ema3), 4)
+        assert -0.230742 == round(float(last.trix), 6)
+        assert -0.204536 == round(float(last.signal), 6)
 
+    def test_exceptions(self, quotes):
+        from System import ArgumentOutOfRangeException
         with pytest.raises(ArgumentOutOfRangeException):
-            indicators.get_stoch(quotes, 14, 3, 0)
+            indicators.get_trix(quotes, 0)
```

### Comparing `stock-indicators-1.2.1/tests/test_stoch_rsi.py` & `stock_indicators-1.3.0/tests/test_stoch_rsi.py`

 * *Files 10% similar despite different names*

```diff
@@ -75,14 +75,23 @@
         removed_qty = rsi_periods + stoch_periods + smooth_periods + 100
         assert 502 - removed_qty == len(results)
 
         last = results.pop()
         assert 89.8385 == round(float(last.stoch_rsi), 4)
         assert 73.4176 == round(float(last.signal), 4)
 
+    def test_condense(self, quotes):
+        results = indicators.get_stoch_rsi(quotes, 14, 14, 3, 3).condense()
+
+        assert 473 == len(results)
+
+        last = results.pop()
+        assert 89.8385 == round(float(last.stoch_rsi), 4)
+        assert 73.4176 == round(float(last.signal), 4)
+
     def test_exceptions(self, quotes):
         from System import ArgumentOutOfRangeException
         with pytest.raises(ArgumentOutOfRangeException):
             indicators.get_stoch_rsi(quotes, 0, 14, 3, 1)
 
         with pytest.raises(ArgumentOutOfRangeException):
             indicators.get_stoch_rsi(quotes, 14, 0, 3, 3)
```

### Comparing `stock-indicators-1.2.1/tests/test_super_trend.py` & `stock_indicators-1.3.0/tests/test_super_trend.py`

 * *Files 18% similar despite different names*

```diff
@@ -57,14 +57,24 @@
         assert 488 == len(results)
 
         last = results.pop()
         assert 250.7954 == round(float(last.super_trend), 4)
         assert last.super_trend == last.upper_band
         assert last.lower_band is None
 
+    def test_condense(self, quotes):
+        results = indicators.get_super_trend(quotes, 14, 3).condense()
+
+        assert 488 == len(results)
+
+        last = results.pop()
+        assert 250.7954 == round(float(last.super_trend), 4)
+        assert last.super_trend == last.upper_band
+        assert last.lower_band is None
+
     def test_exceptions(self, quotes):
         from System import ArgumentOutOfRangeException
         with pytest.raises(ArgumentOutOfRangeException):
             indicators.get_super_trend(quotes, 1)
 
         with pytest.raises(ArgumentOutOfRangeException):
             indicators.get_super_trend(quotes, 7, 0)
```

### Comparing `stock-indicators-1.2.1/tests/test_t3.py` & `stock_indicators-1.3.0/tests/test_t3.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,15 +32,23 @@
         
     def test_no_quotes(self, quotes):
         r = indicators.get_t3([])
         assert 0 == len(r)
         
         r = indicators.get_t3(quotes[:1])
         assert 1 == len(r)
-        
+
+    def test_condense(self, quotes):
+        results = indicators.get_t3(quotes, 5, 0.7).condense()
+
+        assert 502 == len(results)
+
+        last = results.pop()
+        assert 238.9308 == round(float(last.t3), 4)
+
     def test_exceptions(self, quotes):
         from System import ArgumentOutOfRangeException
         with pytest.raises(ArgumentOutOfRangeException):
             indicators.get_t3(quotes, 0)
 
         with pytest.raises(ArgumentOutOfRangeException):
             indicators.get_t3(quotes, 25, 0)
```

### Comparing `stock-indicators-1.2.1/tests/test_tr.py` & `stock_indicators-1.3.0/tests/test_tr.py`

 * *Files 5% similar despite different names*

```diff
@@ -34,7 +34,15 @@
     
     def test_no_quotes(self, quotes):
         r = indicators.get_tr([])
         assert 0 == len(r)
         
         r = indicators.get_tr(quotes[:1])
         assert 1 == len(r)
+
+    def test_condense(self, quotes):
+        results = indicators.get_tr(quotes).condense()
+
+        assert 501 == len(results)
+
+        last = results.pop()
+        assert 2.67 == round(float(last.tr), 2)
```

### Comparing `stock-indicators-1.2.1/tests/test_trix.py` & `stock_indicators-1.3.0/tests/test_williams_r.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,45 +1,48 @@
 import pytest
 from stock_indicators import indicators
 
-class TestTRIX:
-    def test_standard(self, quotes):
-        results = indicators.get_trix(quotes, 20, 5)
 
+class TestWilliamsR:
+    def test_standard(self, quotes):
+        results = indicators.get_williams_r(quotes, 14)
+        
         assert 502 == len(results)
-        assert 482 == len(list(filter(lambda x: x.ema3 is not None, results)))
-        assert 482 == len(list(filter(lambda x: x.trix is not None, results)))
-        assert 478 == len(list(filter(lambda x: x.signal is not None, results)))
-
-        r = results[67]
-        assert 221.7837 == round(float(r.ema3), 4)
-        assert 0.050030 == round(float(r.trix), 6)
-        assert 0.057064 == round(float(r.signal), 6)
-
-        r = results[249]
-        assert 249.4469 == round(float(r.ema3), 4)
-        assert 0.121781 == round(float(r.trix), 6)
-        assert 0.119769 == round(float(r.signal), 6)
-
+        assert 489 == len(list(filter(lambda x: x.williams_r is not None, results)))
+        
+        r = results[343]
+        assert -19.8211 == round(float(r.williams_r), 4)
+        
         r = results[501]
-        assert  263.3216 == round(float(r.ema3), 4)
-        assert -0.230742 == round(float(r.trix), 6)
-        assert -0.204536 == round(float(r.signal), 6)
-
+        assert -52.0121 == round(float(r.williams_r), 4)
+        
     def test_bad_data(self, bad_quotes):
-        r = indicators.get_trix(bad_quotes, 15, 2)
+        r = indicators.get_williams_r(bad_quotes)
         assert 502 == len(r)
-
+        
+    def test_no_quotes(self, quotes):
+        r = indicators.get_williams_r([])
+        assert 0 == len(r)
+        
+        r = indicators.get_williams_r(quotes[:1])
+        assert 1 == len(r)
+        
     def test_removed(self, quotes):
-        results = indicators.get_trix(quotes, 20, 5).remove_warmup_periods()
+        results = indicators.get_williams_r(quotes, 14).remove_warmup_periods()
+
+        assert 502 - 13 == len(results)
+        
+        last = results.pop()
+        assert -52.0121 == round(float(last.williams_r), 4)
+
+    def test_condense(self, quotes):
+        results = indicators.get_williams_r(quotes, 14).condense()
 
-        assert 502 - ((3 * 20) + 100) == len(results)
+        assert 489 == len(results)
 
         last = results.pop()
-        assert  263.3216 == round(float(last.ema3), 4)
-        assert -0.230742 == round(float(last.trix), 6)
-        assert -0.204536 == round(float(last.signal), 6)
+        assert -52.0121 == round(float(last.williams_r), 4)
 
     def test_exceptions(self, quotes):
         from System import ArgumentOutOfRangeException
         with pytest.raises(ArgumentOutOfRangeException):
-            indicators.get_trix(quotes, 0)
+            indicators.get_williams_r(quotes, 0)
```

### Comparing `stock-indicators-1.2.1/tests/test_tsi.py` & `stock_indicators-1.3.0/tests/test_tsi.py`

 * *Files 5% similar despite different names*

```diff
@@ -45,23 +45,31 @@
         r = indicators.get_tsi([])
         assert 0 == len(r)
         
         r = indicators.get_tsi(quotes[:1])
         assert 1 == len(r)
         
     def test_removed(self, quotes):
-        results = indicators.get_tsi(quotes, 25, 13, 7)
-        results = results.remove_warmup_periods()
+        results = indicators.get_tsi(quotes, 25, 13, 7).remove_warmup_periods()
         
         assert 502 - (25 + 13 + 250) == len(results)
         
         last = results.pop()
         assert -28.3513 == round(float(last.tsi), 4)
         assert -29.3597 == round(float(last.signal), 4)
-        
+
+    def test_condense(self, quotes):
+        results = indicators.get_tsi(quotes, 25, 13, 7).condense()
+
+        assert 465 == len(results)
+
+        last = results.pop()
+        assert -28.3513 == round(float(last.tsi), 4)
+        assert -29.3597 == round(float(last.signal), 4)
+
     def test_exceptions(self, quotes):
         from System import ArgumentOutOfRangeException
         with pytest.raises(ArgumentOutOfRangeException):
             indicators.get_tsi(quotes, 0)
 
         with pytest.raises(ArgumentOutOfRangeException):
             indicators.get_tsi(quotes, 25, 0)
```

### Comparing `stock-indicators-1.2.1/tests/test_ulcer_index.py` & `stock_indicators-1.3.0/tests/test_ulcer_index.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,19 +19,26 @@
         r = indicators.get_ulcer_index([])
         assert 0 == len(r)
         
         r = indicators.get_ulcer_index(quotes[:1])
         assert 1 == len(r)
         
     def test_removed(self, quotes):
-        results = indicators.get_ulcer_index(quotes, 14)
-        results = results.remove_warmup_periods()
+        results = indicators.get_ulcer_index(quotes, 14).remove_warmup_periods()
         
         assert 502 - 13 == len(results)
         
         last = results.pop()
         assert 5.7255 == round(float(last.ui), 4)
-        
+
+    def test_condense(self, quotes):
+        results = indicators.get_ulcer_index(quotes, 14).condense()
+
+        assert 489 == len(results)
+
+        last = results.pop()
+        assert 5.7255 == round(float(last.ui), 4)
+
     def test_exceptions(self, quotes):
         from System import ArgumentOutOfRangeException
         with pytest.raises(ArgumentOutOfRangeException):
             indicators.get_ulcer_index(quotes, 0)
```

### Comparing `stock-indicators-1.2.1/tests/test_ultimate.py` & `stock_indicators-1.3.0/tests/test_ultimate.py`

 * *Files 10% similar despite different names*

```diff
@@ -25,22 +25,29 @@
         r = indicators.get_ultimate([])
         assert 0 == len(r)
         
         r = indicators.get_ultimate(quotes[:1])
         assert 1 == len(r)
         
     def test_removed(self, quotes):
-        results = indicators.get_ultimate(quotes, 7, 14, 28)
-        results = results.remove_warmup_periods()
+        results = indicators.get_ultimate(quotes, 7, 14, 28).remove_warmup_periods()
         
         assert 502 - 28 == len(results)
         
         last = results.pop()
         assert 49.5257 == round(float(last.ultimate), 4)
-        
+
+    def test_condense(self, quotes):
+        results = indicators.get_ultimate(quotes, 7, 14, 28).condense()
+
+        assert 474 == len(results)
+
+        last = results.pop()
+        assert 49.5257 == round(float(last.ultimate), 4)
+
     def test_exceptions(self, quotes):
         from System import ArgumentOutOfRangeException
         with pytest.raises(ArgumentOutOfRangeException):
             indicators.get_ultimate(quotes, 0)
             
         with pytest.raises(ArgumentOutOfRangeException):
             indicators.get_ultimate(quotes, 7, 6)
```

### Comparing `stock-indicators-1.2.1/tests/test_volatility_stop.py` & `stock_indicators-1.3.0/tests/test_volatility_stop.py`

 * *Files 5% similar despite different names*

```diff
@@ -61,23 +61,31 @@
         r = indicators.get_volatility_stop([])
         assert 0 == len(r)
 
         r = indicators.get_volatility_stop(quotes[:1])
         assert 1 == len(r)
 
     def test_removed(self, quotes):
-        results = indicators.get_volatility_stop(quotes, 14, 3)
-        results = results.remove_warmup_periods()
+        results = indicators.get_volatility_stop(quotes, 14, 3).remove_warmup_periods()
 
         assert 402 == len(results)
 
         last = results.pop()
         assert 249.2423 == round(float(last.sar), 4)
         assert last.is_stop is False
 
+    def test_condense(self, quotes):
+        results = indicators.get_volatility_stop(quotes, 14, 3).condense()
+
+        assert 448 == len(results)
+
+        last = results.pop()
+        assert 249.2423 == round(float(last.sar), 4)
+        assert last.is_stop is False
+
     def test_exceptions(self, quotes):
         from System import ArgumentOutOfRangeException
         with pytest.raises(ArgumentOutOfRangeException):
             indicators.get_volatility_stop(quotes, 1)
 
         with pytest.raises(ArgumentOutOfRangeException):
             indicators.get_volatility_stop(quotes, 20, 0)
```

### Comparing `stock-indicators-1.2.1/tests/test_vortex.py` & `stock_indicators-1.3.0/tests/test_vortex.py`

 * *Files 15% similar despite different names*

```diff
@@ -36,20 +36,28 @@
         r = indicators.get_vortex([], 5)
         assert 0 == len(r)
         
         r = indicators.get_vortex(quotes[:1], 5)
         assert 1 == len(r)
         
     def test_removed(self, quotes):
-        results = indicators.get_vortex(quotes, 14)
-        results = results.remove_warmup_periods()
+        results = indicators.get_vortex(quotes, 14).remove_warmup_periods()
         
         assert 502 - 14 == len(results)
         
         last = results.pop()
         assert 0.8712 == round(float(last.pvi), 4)
         assert 1.1163 == round(float(last.nvi), 4)
-        
+
+    def test_condense(self, quotes):
+        results = indicators.get_vortex(quotes, 14).condense()
+
+        assert 488 == len(results)
+
+        last = results.pop()
+        assert 0.8712 == round(float(last.pvi), 4)
+        assert 1.1163 == round(float(last.nvi), 4)
+
     def test_exceptions(self, quotes):
         from System import ArgumentOutOfRangeException
         with pytest.raises(ArgumentOutOfRangeException):
             indicators.get_vortex(quotes, 1)
```

### Comparing `stock-indicators-1.2.1/tests/test_vwap.py` & `stock_indicators-1.3.0/tests/test_vwap.py`

 * *Files 6% similar despite different names*

```diff
@@ -93,14 +93,25 @@
         assert 361 == len(results_int) == len(results_date)
         
         last_d = results_date.pop()
         last_i = results_int.pop()
         
         assert 368.2908 == round(float(last_d.vwap), 4)
         assert 368.2908 == round(float(last_i.vwap), 4)
+
+    def test_condense(self, intraday_quotes):
+        intraday_quotes.sort(key=lambda x: x.date)
         
+        results_int = indicators.get_vwap(intraday_quotes[:391], 2020, 12, 15, 10)
+        results_int = results_int.condense()
+        
+        assert 361 == len(results_int)
+        
+        last_i = results_int.pop()
+        assert 368.2908 == round(float(last_i.vwap), 4)
+
     def test_exceptions(self, quotes):
         start_date = datetime(2000, 12, 15)
         
         from System import ArgumentOutOfRangeException
         with pytest.raises(ArgumentOutOfRangeException):
             indicators.get_vwap(quotes, start_date)
```

### Comparing `stock-indicators-1.2.1/tests/test_vwma.py` & `stock_indicators-1.3.0/tests/test_vwma.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,12 +41,20 @@
     def test_removed(self, quotes):
         results = indicators.get_vwma(quotes, 10).remove_warmup_periods()
         
         assert 502 - 9 == len(results)
         
         last = results.pop()
         assert 242.101548 == round(float(last.vwma), 6)
-        
+
+    def test_condense(self, quotes):
+        results = indicators.get_vwma(quotes, 10).condense()
+
+        assert 493 == len(results)
+
+        last = results.pop()
+        assert 242.101548 == round(float(last.vwma), 6)
+
     def test_exceptions(self, quotes):
         from System import ArgumentOutOfRangeException
         with pytest.raises(ArgumentOutOfRangeException):
             indicators.get_vwma(quotes, 0)
```

### Comparing `stock-indicators-1.2.1/tests/test_williams_r.py` & `stock_indicators-1.3.0/tests/test_sma_analysis.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,40 +1,53 @@
 import pytest
 from stock_indicators import indicators
+from stock_indicators._cslib import CsDecimal
 
-
-class TestWilliamsR:
-    def test_standard(self, quotes):
-        results = indicators.get_williams_r(quotes, 14)
+class TestSMAExtended:
+    def test_result_types(self, quotes):
+        results = indicators.get_sma_analysis(quotes, 20)
         
+        # Sample value.
+        r = results[501]
+        assert     float == type(r._csdata.Sma)
+        assert     float == type(r._csdata.Mad)
+        assert     float == type(r._csdata.Mse)
+        assert     float == type(r._csdata.Mape)
+
+    def test_extended(self, quotes):
+        results = indicators.get_sma_analysis(quotes, 20)
+
+        # proper quantities.
+        # should always be the same number of results as there is quotes.
         assert 502 == len(results)
-        assert 489 == len(list(filter(lambda x: x.williams_r is not None, results)))
-        
-        r = results[343]
-        assert -19.8211 == round(float(r.williams_r), 4)
-        
+        assert 483 == len(list(filter(lambda x: x.sma is not None, results)))
+
+        # Sample value.
         r = results[501]
-        assert -52.0121 == round(float(r.williams_r), 4)
-        
+        assert 251.8600 == round(float(r.sma), 4)
+        assert 9.4500   == round(float(r.mad), 4)
+        assert 119.2510 == round(float(r.mse), 4)
+        assert 0.037637 == round(float(r.mape), 6)
+
     def test_bad_data(self, bad_quotes):
-        r = indicators.get_williams_r(bad_quotes)
-        assert 502 == len(r)
-        
-    def test_no_quotes(self, quotes):
-        r = indicators.get_williams_r([])
-        assert 0 == len(r)
-        
-        r = indicators.get_williams_r(quotes[:1])
-        assert 1 == len(r)
-        
+        results = indicators.get_sma_analysis(bad_quotes, 15)
+
+        # Assertions 
+        assert 502 == len(results)
+
     def test_removed(self, quotes):
-        results = indicators.get_williams_r(quotes, 14).remove_warmup_periods()
+        results = indicators.get_sma_analysis(quotes, 20).remove_warmup_periods()
+
+        # Assertions
+        assert 502 - 19 == len(results)
+        assert 251.8600 == round(float(results[len(results)-1].sma), 4)
+
+    def test_condense(self, quotes):
+        results = indicators.get_sma_analysis(quotes, 20).condense()
+
+        assert 483 == len(results)
+        assert 251.8600 == round(float(results[len(results)-1].sma), 4)
 
-        assert 502 - 13 == len(results)
-        
-        last = results.pop()
-        assert -52.0121 == round(float(last.williams_r), 4)
-                
     def test_exceptions(self, quotes):
         from System import ArgumentOutOfRangeException
         with pytest.raises(ArgumentOutOfRangeException):
-            indicators.get_williams_r(quotes, 0)
+            indicators.get_sma_analysis(quotes, 0)
```

### Comparing `stock-indicators-1.2.1/tests/test_wma.py` & `stock_indicators-1.3.0/tests/test_wma.py`

 * *Files 14% similar despite different names*

```diff
@@ -29,12 +29,20 @@
     def test_removed(self, quotes):
         results = indicators.get_wma(quotes, 20).remove_warmup_periods()
 
         assert 502 - 19 == len(results)
         
         last = results.pop()
         assert 246.5110 == round(float(last.wma), 4)
-                
+
+    def test_condense(self, quotes):
+        results = indicators.get_wma(quotes, 20).condense()
+
+        assert 483 == len(results)
+
+        last = results.pop()
+        assert 246.5110 == round(float(last.wma), 4)
+
     def test_exceptions(self, quotes):
         from System import ArgumentOutOfRangeException
         with pytest.raises(ArgumentOutOfRangeException):
             indicators.get_wma(quotes, 0)
```

### Comparing `stock-indicators-1.2.1/tests/test_zig_zag.py` & `stock_indicators-1.3.0/tests/test_zig_zag.py`

 * *Files 3% similar despite different names*

```diff
@@ -126,11 +126,22 @@
     def test_bad_quotes(self, bad_quotes):
         r = indicators.get_zig_zag(bad_quotes, EndType.CLOSE)
         assert 502 == len(r)
         
         r = indicators.get_zig_zag(bad_quotes, EndType.HIGH_LOW)
         assert 502 == len(r)
 
+    def test_condense(self, quotes):
+        results = indicators.get_zig_zag(quotes, EndType.CLOSE, 3).condense()
+
+        assert 14 == len(results)
+
+        last = results.pop()
+        assert  229.99 == float(round(last.zig_zag, 2))
+        assert  251.33 == float(round(last.retrace_high, 2))
+        assert  229.99 == float(round(last.retrace_low, 2))
+        assert     "L" == last.point_type
+
     def test_exceptions(self, quotes):
         from System import ArgumentOutOfRangeException
         with pytest.raises(ArgumentOutOfRangeException):
             indicators.get_zig_zag(quotes, EndType.CLOSE, 0)
```

### Comparing `stock-indicators-1.2.1/tests/utiltest.py` & `stock_indicators-1.3.0/tests/utiltest.py`

 * *Files identical despite different names*

