# Comparing `tmp/inspect_ai-0.3.5.tar.gz` & `tmp/inspect_ai-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inspect_ai-0.3.5.tar", last modified: Sat May  4 21:23:47 2024, max compression
+gzip compressed data, was "inspect_ai-0.3.6.tar", last modified: Mon May  6 20:23:28 2024, max compression
```

## Comparing `inspect_ai-0.3.5.tar` & `inspect_ai-0.3.6.tar`

### file list

```diff
@@ -1,369 +1,369 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 21:23:47.407093 inspect_ai-0.3.5/
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 21:23:47.343093 inspect_ai-0.3.5/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 21:23:47.343093 inspect_ai-0.3.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (127)      544 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/.github/workflows/pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3194 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 21:23:47.343093 inspect_ai-0.3.5/.vscode/
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/.vscode/extensions.json
--rw-r--r--   0 runner    (1001) docker     (127)      465 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (127)     3321 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4148 2024-05-04 21:23:47.407093 inspect_ai-0.3.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 21:23:47.347093 inspect_ai-0.3.5/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/benchmarks/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/benchmarks/arc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 21:23:47.347093 inspect_ai-0.3.5/benchmarks/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/benchmarks/datasets/math_test.csv
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/benchmarks/datasets/mmlu.csv
--rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/benchmarks/gpqa.py
--rw-r--r--   0 runner    (1001) docker     (127)     2453 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/benchmarks/gsm8k.py
--rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/benchmarks/hellaswag.py
--rw-r--r--   0 runner    (1001) docker     (127)     3555 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/benchmarks/mathematics.py
--rw-r--r--   0 runner    (1001) docker     (127)     6930 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/benchmarks/mmlu.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 21:23:47.351093 inspect_ai-0.3.5/docs/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/docs/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 21:23:47.351093 inspect_ai-0.3.5/docs/_examples/
--rw-r--r--   0 runner    (1001) docker     (127)     4560 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/docs/_examples/arc.qmd
--rw-r--r--   0 runner    (1001) docker     (127)     3010 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/docs/_examples/biology_qa.qmd
--rw-r--r--   0 runner    (1001) docker     (127)      998 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/docs/_examples/footer.qmd
--rw-r--r--   0 runner    (1001) docker     (127)     5579 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/docs/_examples/gsm8k.qmd
--rw-r--r--   0 runner    (1001) docker     (127)     3234 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/docs/_examples/hellaswag.qmd
--rw-r--r--   0 runner    (1001) docker     (127)     2624 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/docs/_examples/index.qmd
--rw-r--r--   0 runner    (1001) docker     (127)     6808 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/docs/_examples/mathematics.qmd
--rw-r--r--   0 runner    (1001) docker     (127)     2992 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/docs/_examples/popularity.qmd
--rw-r--r--   0 runner    (1001) docker     (127)     2153 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/docs/_examples/security_guide.qmd
--rw-r--r--   0 runner    (1001) docker     (127)     2158 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/docs/_examples/theory_of_mind.qmd
--rw-r--r--   0 runner    (1001) docker     (127)     4655 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/docs/_examples/tool_use.qmd
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 21:23:47.351093 inspect_ai-0.3.5/docs/_format/
--rwxr-xr-x   0 runner    (1001) docker     (127)      364 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/docs/_format/pre-render.sh
--rw-r--r--   0 runner    (1001) docker     (127)     2504 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/docs/_quarto.yml
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/docs/_variables.yml
--rw-r--r--   0 runner    (1001) docker     (127)    11333 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/docs/datasets.qmd
--rw-r--r--   0 runner    (1001) docker     (127)     9905 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/docs/eval-logs.qmd
--rw-r--r--   0 runner    (1001) docker     (127)     8386 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/docs/eval-suites.qmd
--rw-r--r--   0 runner    (1001) docker     (127)    10373 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/docs/eval-tuning.qmd
--rw-r--r--   0 runner    (1001) docker     (127)    35808 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/docs/examples.qmd
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 21:23:47.359093 inspect_ai-0.3.5/docs/images/
--rw-r--r--   0 runner    (1001) docker     (127)   170128 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/docs/images/aisi-logo.png
--rw-r--r--   0 runner    (1001) docker     (127)    68030 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/docs/images/eval-log.png
--rw-r--r--   0 runner    (1001) docker     (127)   314093 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/docs/images/inspect-view-answers.png
--rw-r--r--   0 runner    (1001) docker     (127)   280184 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/docs/images/inspect-view-filter.png
--rw-r--r--   0 runner    (1001) docker     (127)   284131 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/docs/images/inspect-view-history.png
--rw-r--r--   0 runner    (1001) docker     (127)   413188 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/docs/images/inspect-view-home.png
--rw-r--r--   0 runner    (1001) docker     (127)   241738 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/docs/images/inspect-view-info.png
--rw-r--r--   0 runner    (1001) docker     (127)   143202 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/docs/images/inspect-view-logging-console.png
--rw-r--r--   0 runner    (1001) docker     (127)   155304 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/docs/images/inspect-view-logging.png
--rw-r--r--   0 runner    (1001) docker     (127)   373146 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/docs/images/inspect-view-main.png
--rw-r--r--   0 runner    (1001) docker     (127)   321793 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/docs/images/inspect-view-messages.png
--rw-r--r--   0 runner    (1001) docker     (127)   165394 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/docs/images/inspect-view-metadata.png
--rw-r--r--   0 runner    (1001) docker     (127)   272733 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/docs/images/inspect-view-scoring.png
--rw-r--r--   0 runner    (1001) docker     (127)   274383 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/docs/images/inspect-view-sort.png
--rw-r--r--   0 runner    (1001) docker     (127)    90624 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/docs/images/inspect-view-splash.png
--rw-r--r--   0 runner    (1001) docker     (127)    68787 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/docs/images/popularity.png
--rw-r--r--   0 runner    (1001) docker     (127)    54252 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/docs/images/rate-limit.png
--rw-r--r--   0 runner    (1001) docker     (127)    48461 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/docs/images/running-theory.png
--rw-r--r--   0 runner    (1001) docker     (127)    10437 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/docs/index.qmd
--rw-r--r--   0 runner    (1001) docker     (127)     9421 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/docs/log-viewer.qmd
--rw-r--r--   0 runner    (1001) docker     (127)    18564 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/docs/models.qmd
--rw-r--r--   0 runner    (1001) docker     (127)    15801 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/docs/scorers.qmd
--rw-r--r--   0 runner    (1001) docker     (127)    14283 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/docs/solvers.qmd
--rw-r--r--   0 runner    (1001) docker     (127)      825 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/docs/theme.scss
--rw-r--r--   0 runner    (1001) docker     (127)    15937 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/docs/tools.qmd
--rw-r--r--   0 runner    (1001) docker     (127)    12752 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/docs/workflow.qmd
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 21:23:47.359093 inspect_ai-0.3.5/examples/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 21:23:47.335093 inspect_ai-0.3.5/examples/agents/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 21:23:47.363093 inspect_ai-0.3.5/examples/agents/langchain/
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/examples/agents/langchain/.env.example
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/examples/agents/langchain/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     2029 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/examples/agents/langchain/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     8266 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/examples/agents/langchain/inspect_langchain.py
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/examples/agents/langchain/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/examples/agents/langchain/wikipedia.jsonl
--rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/examples/agents/langchain/wikipedia.py
--rw-r--r--   0 runner    (1001) docker     (127)      537 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/examples/biology_qa.py
--rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/examples/popularity.py
--rw-r--r--   0 runner    (1001) docker     (127)      639 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/examples/security_guide.py
--rw-r--r--   0 runner    (1001) docker     (127)      514 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/examples/theory_of_mind.py
--rw-r--r--   0 runner    (1001) docker     (127)     1980 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/examples/tool_use.py
--rw-r--r--   0 runner    (1001) docker     (127)     2988 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-04 21:23:47.407093 inspect_ai-0.3.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 21:23:47.335093 inspect_ai-0.3.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 21:23:47.363093 inspect_ai-0.3.5/src/inspect_ai/
--rw-r--r--   0 runner    (1001) docker     (127)      671 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 21:23:47.367093 inspect_ai-0.3.5/src/inspect_ai/_cli/
--rw-r--r--   0 runner    (1001) docker     (127)     1705 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_cli/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     7639 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_cli/eval.py
--rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_cli/info.py
--rw-r--r--   0 runner    (1001) docker     (127)     3716 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_cli/list.py
--rw-r--r--   0 runner    (1001) docker     (127)      849 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_cli/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     2807 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_cli/score.py
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_cli/util.py
--rw-r--r--   0 runner    (1001) docker     (127)      942 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_cli/view.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 21:23:47.367093 inspect_ai-0.3.5/src/inspect_ai/_display/
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_display/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_display/_display.py
--rw-r--r--   0 runner    (1001) docker     (127)     2720 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_display/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)    11708 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_display/rich.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 21:23:47.367093 inspect_ai-0.3.5/src/inspect_ai/_eval/
--rw-r--r--   0 runner    (1001) docker     (127)    16214 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_eval/eval.py
--rw-r--r--   0 runner    (1001) docker     (127)     1767 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_eval/images.py
--rw-r--r--   0 runner    (1001) docker     (127)    11631 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_eval/list.py
--rw-r--r--   0 runner    (1001) docker     (127)     2347 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_eval/loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     3653 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_eval/log.py
--rw-r--r--   0 runner    (1001) docker     (127)     3998 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_eval/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     5586 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_eval/score.py
--rw-r--r--   0 runner    (1001) docker     (127)    22961 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_eval/task.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 21:23:47.371093 inspect_ai-0.3.5/src/inspect_ai/_util/
--rw-r--r--   0 runner    (1001) docker     (127)      355 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_util/appdirs.py
--rw-r--r--   0 runner    (1001) docker     (127)      459 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_util/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)      256 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_util/datetime.py
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_util/dev.py
--rw-r--r--   0 runner    (1001) docker     (127)      352 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_util/docstring.py
--rw-r--r--   0 runner    (1001) docker     (127)     3040 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_util/dotenv.py
--rw-r--r--   0 runner    (1001) docker     (127)      737 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_util/error.py
--rw-r--r--   0 runner    (1001) docker     (127)     5969 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_util/file.py
--rw-r--r--   0 runner    (1001) docker     (127)      886 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_util/git.py
--rw-r--r--   0 runner    (1001) docker     (127)     3628 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_util/http.py
--rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_util/images.py
--rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_util/json.py
--rw-r--r--   0 runner    (1001) docker     (127)     2998 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_util/notebook.py
--rw-r--r--   0 runner    (1001) docker     (127)     2160 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_util/path.py
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_util/pattern.py
--rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_util/platform.py
--rw-r--r--   0 runner    (1001) docker     (127)     8512 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_util/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     2038 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_util/retry.py
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_util/samples.py
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_util/text.py
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_util/url.py
--rw-r--r--   0 runner    (1001) docker     (127)      491 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_util/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 21:23:47.371093 inspect_ai-0.3.5/src/inspect_ai/_view/
--rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_view/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     8607 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_view/view.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 21:23:47.375093 inspect_ai-0.3.5/src/inspect_ai/_view/www/
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_view/www/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)    10186 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_view/www/App.mjs
--rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_view/www/api.mjs
--rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_view/www/favicon.svg
--rw-r--r--   0 runner    (1001) docker     (127)     2231 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_view/www/index.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 21:23:47.375093 inspect_ai-0.3.5/src/inspect_ai/_view/www/libs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 21:23:47.339093 inspect_ai-0.3.5/src/inspect_ai/_view/www/libs/bootstrap/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 21:23:47.375093 inspect_ai-0.3.5/src/inspect_ai/_view/www/libs/bootstrap/css/
--rw-r--r--   0 runner    (1001) docker     (127)    85877 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_view/www/libs/bootstrap/css/bootstrap-icons.min.css
--rw-r--r--   0 runner    (1001) docker     (127)   232903 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_view/www/libs/bootstrap/css/bootstrap.min.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 21:23:47.375093 inspect_ai-0.3.5/src/inspect_ai/_view/www/libs/bootstrap/css/fonts/
--rw-r--r--   0 runner    (1001) docker     (127)   176196 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_view/www/libs/bootstrap/css/fonts/bootstrap-icons.woff
--rw-r--r--   0 runner    (1001) docker     (127)   130764 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_view/www/libs/bootstrap/css/fonts/bootstrap-icons.woff2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 21:23:47.375093 inspect_ai-0.3.5/src/inspect_ai/_view/www/libs/bootstrap/js/
--rw-r--r--   0 runner    (1001) docker     (127)    80615 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_view/www/libs/bootstrap/js/bootstrap.bundle.min.js
--rw-r--r--   0 runner    (1001) docker     (127)     9160 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_view/www/libs/clipboard.min.js
--rw-r--r--   0 runner    (1001) docker     (127)    31629 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_view/www/libs/json5.min.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 21:23:47.375093 inspect_ai-0.3.5/src/inspect_ai/_view/www/libs/prism/
--rw-r--r--   0 runner    (1001) docker     (127)     3481 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_view/www/libs/prism/prism-dark.css
--rw-r--r--   0 runner    (1001) docker     (127)     1896 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_view/www/libs/prism/prism.min.css
--rw-r--r--   0 runner    (1001) docker     (127)    16934 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_view/www/libs/prism/prism.min.js
--rw-r--r--   0 runner    (1001) docker     (127)    21104 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_view/www/libs/purify.min.js
--rw-r--r--   0 runner    (1001) docker     (127)    75207 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_view/www/libs/showdown.min.js
--rw-r--r--   0 runner    (1001) docker     (127)    34863 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_view/www/log-schema.json
--rw-r--r--   0 runner    (1001) docker     (127)     8721 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_view/www/log.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 21:23:47.379094 inspect_ai-0.3.5/src/inspect_ai/_view/www/preact/
--rw-r--r--   0 runner    (1001) docker     (127)     3669 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_view/www/preact/hooks.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 21:23:47.379094 inspect_ai-0.3.5/src/inspect_ai/_view/www/preact/htm/
--rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_view/www/preact/htm/htm.mjs
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_view/www/preact/htm/preact.js
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_view/www/preact/htm/preact.mjs
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_view/www/preact/preact-hooks.mjs
--rw-r--r--   0 runner    (1001) docker     (127)    11268 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_view/www/preact/preact.mjs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 21:23:47.379094 inspect_ai-0.3.5/src/inspect_ai/_view/www/src/
--rw-r--r--   0 runner    (1001) docker     (127)     7233 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_view/www/src/App.css
--rw-r--r--   0 runner    (1001) docker     (127)     2701 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_view/www/src/Constants.mjs
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_view/www/src/Register.mjs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 21:23:47.383093 inspect_ai-0.3.5/src/inspect_ai/_view/www/src/components/
--rw-r--r--   0 runner    (1001) docker     (127)      994 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_view/www/src/components/AnsiDisplay.css
--rw-r--r--   0 runner    (1001) docker     (127)     4058 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_view/www/src/components/AnsiDisplay.mjs
--rw-r--r--   0 runner    (1001) docker     (127)      869 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_view/www/src/components/AppErrorBoundary.mjs
--rw-r--r--   0 runner    (1001) docker     (127)     2248 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_view/www/src/components/Card.mjs
--rw-r--r--   0 runner    (1001) docker     (127)     5498 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_view/www/src/components/ChatView.mjs
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_view/www/src/components/CopyButton.mjs
--rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_view/www/src/components/Dialog.mjs
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_view/www/src/components/EmptyPanel.mjs
--rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_view/www/src/components/ErrorPanel.mjs
--rw-r--r--   0 runner    (1001) docker     (127)      612 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_view/www/src/components/LabeledValue.mjs
--rw-r--r--   0 runner    (1001) docker     (127)      833 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_view/www/src/components/LoadingScreen.mjs
--rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_view/www/src/components/MarkdownDiv.mjs
--rw-r--r--   0 runner    (1001) docker     (127)     1595 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_view/www/src/components/MessageContent.mjs
--rw-r--r--   0 runner    (1001) docker     (127)     2101 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_view/www/src/components/MetaDataView.mjs
--rw-r--r--   0 runner    (1001) docker     (127)     6941 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_view/www/src/components/RenderedContent.mjs
--rw-r--r--   0 runner    (1001) docker     (127)     2745 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_view/www/src/components/TabSet.mjs
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_view/www/src/components/ToolButton.mjs
--rw-r--r--   0 runner    (1001) docker     (127)    20289 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_view/www/src/components/ansi-output.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 21:23:47.383093 inspect_ai-0.3.5/src/inspect_ai/_view/www/src/log-reader/
--rw-r--r--   0 runner    (1001) docker     (127)      551 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_view/www/src/log-reader/Log-Reader.mjs
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_view/www/src/log-reader/Native-Log-Reader.mjs
--rw-r--r--   0 runner    (1001) docker     (127)     8046 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_view/www/src/log-reader/Open-AI-Log-Reader.mjs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 21:23:47.383093 inspect_ai-0.3.5/src/inspect_ai/_view/www/src/logging/
--rw-r--r--   0 runner    (1001) docker     (127)     2946 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_view/www/src/logging/LoggingPanel.mjs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 21:23:47.383093 inspect_ai-0.3.5/src/inspect_ai/_view/www/src/plan/
--rw-r--r--   0 runner    (1001) docker     (127)     8260 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_view/www/src/plan/PlanCard.mjs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 21:23:47.383093 inspect_ai-0.3.5/src/inspect_ai/_view/www/src/samples/
--rw-r--r--   0 runner    (1001) docker     (127)      448 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_view/www/src/samples/SampleGroupSeparator.mjs
--rw-r--r--   0 runner    (1001) docker     (127)     3249 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_view/www/src/samples/SampleScoreView.mjs
--rw-r--r--   0 runner    (1001) docker     (127)     8207 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_view/www/src/samples/SampleView.mjs
--rw-r--r--   0 runner    (1001) docker     (127)     4467 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_view/www/src/samples/SamplesCard.mjs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 21:23:47.383093 inspect_ai-0.3.5/src/inspect_ai/_view/www/src/title/
--rw-r--r--   0 runner    (1001) docker     (127)     5378 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_view/www/src/title/TitleBlock.mjs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 21:23:47.383093 inspect_ai-0.3.5/src/inspect_ai/_view/www/src/usage/
--rw-r--r--   0 runner    (1001) docker     (127)     1281 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_view/www/src/usage/ModelTokenTable.mjs
--rw-r--r--   0 runner    (1001) docker     (127)     1890 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_view/www/src/usage/UsageCard.mjs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 21:23:47.383093 inspect_ai-0.3.5/src/inspect_ai/_view/www/src/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     3072 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_view/www/src/utils/Format.mjs
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_view/www/src/utils/Git.mjs
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_view/www/src/utils/Path.mjs
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_view/www/src/utils/Type.mjs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 21:23:47.387093 inspect_ai-0.3.5/src/inspect_ai/_view/www/src/workspace/
--rw-r--r--   0 runner    (1001) docker     (127)      822 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_view/www/src/workspace/EpochFilter.mjs
--rw-r--r--   0 runner    (1001) docker     (127)     4853 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_view/www/src/workspace/SampleFilter.mjs
--rw-r--r--   0 runner    (1001) docker     (127)     7027 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_view/www/src/workspace/SamplesDescriptor.mjs
--rw-r--r--   0 runner    (1001) docker     (127)     2684 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_view/www/src/workspace/SortFilter.mjs
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_view/www/src/workspace/TaskErrorPanel.mjs
--rw-r--r--   0 runner    (1001) docker     (127)    15380 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_view/www/src/workspace/WorkSpace.mjs
--rw-r--r--   0 runner    (1001) docker     (127)     8721 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/_view/www/tools.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 21:23:47.387093 inspect_ai-0.3.5/src/inspect_ai/dataset/
--rw-r--r--   0 runner    (1001) docker     (127)      534 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7465 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/dataset/_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 21:23:47.387093 inspect_ai-0.3.5/src/inspect_ai/dataset/_examples/
--rw-r--r--   0 runner    (1001) docker     (127)    20756 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/dataset/_examples/bias_detection.jsonl
--rw-r--r--   0 runner    (1001) docker     (127)     2009 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/dataset/_examples/biology_qa.jsonl
--rw-r--r--   0 runner    (1001) docker     (127)    32773 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/dataset/_examples/popularity.jsonl
--rw-r--r--   0 runner    (1001) docker     (127)     2659 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/dataset/_examples/security_guide.jsonl
--rw-r--r--   0 runner    (1001) docker     (127)    31831 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/dataset/_examples/theory_of_mind.jsonl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 21:23:47.387093 inspect_ai-0.3.5/src/inspect_ai/dataset/_sources/
--rw-r--r--   0 runner    (1001) docker     (127)     3035 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/dataset/_sources/csv.py
--rw-r--r--   0 runner    (1001) docker     (127)     1702 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/dataset/_sources/example.py
--rw-r--r--   0 runner    (1001) docker     (127)     2557 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/dataset/_sources/file.py
--rw-r--r--   0 runner    (1001) docker     (127)     3559 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/dataset/_sources/hf.py
--rw-r--r--   0 runner    (1001) docker     (127)     3335 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/dataset/_sources/json.py
--rw-r--r--   0 runner    (1001) docker     (127)     3766 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/dataset/_util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 21:23:47.387093 inspect_ai-0.3.5/src/inspect_ai/log/
--rw-r--r--   0 runner    (1001) docker     (127)      776 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/log/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10183 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/log/_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     9174 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/log/_log.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 21:23:47.391093 inspect_ai-0.3.5/src/inspect_ai/model/
--rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    31683 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/model/_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 21:23:47.391093 inspect_ai-0.3.5/src/inspect_ai/model/_providers/
--rw-r--r--   0 runner    (1001) docker     (127)    29724 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/model/_providers/anthropic.py
--rw-r--r--   0 runner    (1001) docker     (127)     7885 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/model/_providers/azureai.py
--rw-r--r--   0 runner    (1001) docker     (127)    10818 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/model/_providers/bedrock.py
--rw-r--r--   0 runner    (1001) docker     (127)     3043 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/model/_providers/cloudflare.py
--rw-r--r--   0 runner    (1001) docker     (127)    10170 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/model/_providers/google.py
--rw-r--r--   0 runner    (1001) docker     (127)    10061 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/model/_providers/hf.py
--rw-r--r--   0 runner    (1001) docker     (127)     7859 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/model/_providers/mistral.py
--rw-r--r--   0 runner    (1001) docker     (127)    13476 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/model/_providers/openai.py
--rw-r--r--   0 runner    (1001) docker     (127)     3298 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/model/_providers/providers.py
--rw-r--r--   0 runner    (1001) docker     (127)      990 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/model/_providers/together.py
--rw-r--r--   0 runner    (1001) docker     (127)      857 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/model/_providers/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     2426 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/model/_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/model/_tool.py
--rw-r--r--   0 runner    (1001) docker     (127)     4749 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/model/_util.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 21:23:47.391093 inspect_ai-0.3.5/src/inspect_ai/scorer/
--rw-r--r--   0 runner    (1001) docker     (127)      893 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/scorer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2054 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/scorer/_answer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2717 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/scorer/_common.py
--rw-r--r--   0 runner    (1001) docker     (127)     1686 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/scorer/_match.py
--rw-r--r--   0 runner    (1001) docker     (127)     7209 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/scorer/_metric.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 21:23:47.395093 inspect_ai-0.3.5/src/inspect_ai/scorer/_metrics/
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/scorer/_metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      943 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/scorer/_metrics/accuracy.py
--rw-r--r--   0 runner    (1001) docker     (127)      555 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/scorer/_metrics/mean.py
--rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/scorer/_metrics/std.py
--rw-r--r--   0 runner    (1001) docker     (127)     7089 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/scorer/_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1802 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/scorer/_pattern.py
--rw-r--r--   0 runner    (1001) docker     (127)     4362 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/scorer/_scorer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 21:23:47.395093 inspect_ai-0.3.5/src/inspect_ai/solver/
--rw-r--r--   0 runner    (1001) docker     (127)      671 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/solver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3100 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/solver/_critique.py
--rw-r--r--   0 runner    (1001) docker     (127)     6146 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/solver/_multiple_choice.py
--rw-r--r--   0 runner    (1001) docker     (127)     5189 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/solver/_plan.py
--rw-r--r--   0 runner    (1001) docker     (127)     2292 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/solver/_prompt.py
--rw-r--r--   0 runner    (1001) docker     (127)     8101 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/solver/_solver.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 21:23:47.395093 inspect_ai-0.3.5/src/inspect_ai/solver/_tool/
--rw-r--r--   0 runner    (1001) docker     (127)     3810 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/solver/_tool/tool.py
--rw-r--r--   0 runner    (1001) docker     (127)     2434 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/solver/_tool/tool_def.py
--rw-r--r--   0 runner    (1001) docker     (127)     1680 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/solver/_tool/use_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     7376 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/solver/_tool/web_search.py
--rw-r--r--   0 runner    (1001) docker     (127)      446 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/solver/_util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 21:23:47.395093 inspect_ai-0.3.5/src/inspect_ai/util/
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/util/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 21:23:47.395093 inspect_ai-0.3.5/src/inspect_ai/util/_context/
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/util/_context/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2777 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/util/_context/concurrency.py
--rw-r--r--   0 runner    (1001) docker     (127)      690 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/util/_context/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     3146 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/util/_context/resource.py
--rw-r--r--   0 runner    (1001) docker     (127)     4734 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/src/inspect_ai/util/_context/subprocess.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 21:23:47.407093 inspect_ai-0.3.5/src/inspect_ai.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4148 2024-05-04 21:23:47.000000 inspect_ai-0.3.5/src/inspect_ai.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10858 2024-05-04 21:23:47.000000 inspect_ai-0.3.5/src/inspect_ai.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 21:23:47.000000 inspect_ai-0.3.5/src/inspect_ai.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-04 21:23:47.000000 inspect_ai-0.3.5/src/inspect_ai.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      618 2024-05-04 21:23:47.000000 inspect_ai-0.3.5/src/inspect_ai.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-04 21:23:47.000000 inspect_ai-0.3.5/src/inspect_ai.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 21:23:47.399093 inspect_ai-0.3.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/tests/test_anthropic.py
--rw-r--r--   0 runner    (1001) docker     (127)      380 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/tests/test_cloudlfare.py
--rw-r--r--   0 runner    (1001) docker     (127)     1730 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/tests/test_collapse_user_message.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 21:23:47.403093 inspect_ai-0.3.5/tests/test_dataset/
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/tests/test_dataset/samples.csv
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/tests/test_dataset/samples.json
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/tests/test_dataset/samples.jsonl
--rw-r--r--   0 runner    (1001) docker     (127)     2206 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/tests/test_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)      881 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/tests/test_eval_log.py
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/tests/test_examples.py
--rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/tests/test_hf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 21:23:47.403093 inspect_ai-0.3.5/tests/test_images/
--rw-r--r--   0 runner    (1001) docker     (127)   732622 2024-05-04 21:23:42.000000 inspect_ai-0.3.5/tests/test_images/images.jsonl
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-04 21:23:41.000000 inspect_ai-0.3.5/tests/test_images.py
--rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-05-04 21:23:42.000000 inspect_ai-0.3.5/tests/test_list_task.py
--rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-05-04 21:23:42.000000 inspect_ai-0.3.5/tests/test_logprobs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3112 2024-05-04 21:23:42.000000 inspect_ai-0.3.5/tests/test_metric.py
--rw-r--r--   0 runner    (1001) docker     (127)      920 2024-05-04 21:23:42.000000 inspect_ai-0.3.5/tests/test_num_choices.py
--rw-r--r--   0 runner    (1001) docker     (127)      746 2024-05-04 21:23:42.000000 inspect_ai-0.3.5/tests/test_openai.py
--rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-05-04 21:23:42.000000 inspect_ai-0.3.5/tests/test_plan.py
--rw-r--r--   0 runner    (1001) docker     (127)      728 2024-05-04 21:23:42.000000 inspect_ai-0.3.5/tests/test_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-05-04 21:23:42.000000 inspect_ai-0.3.5/tests/test_retry.py
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-04 21:23:42.000000 inspect_ai-0.3.5/tests/test_scorer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1897 2024-05-04 21:23:42.000000 inspect_ai-0.3.5/tests/test_solver.py
--rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-05-04 21:23:42.000000 inspect_ai-0.3.5/tests/test_stop_reason.py
--rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-05-04 21:23:42.000000 inspect_ai-0.3.5/tests/test_subprocess.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 21:23:47.403093 inspect_ai-0.3.5/tests/test_task_list/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 21:23:42.000000 inspect_ai-0.3.5/tests/test_task_list/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      394 2024-05-04 21:23:42.000000 inspect_ai-0.3.5/tests/test_task_list/attribs.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-04 21:23:42.000000 inspect_ai-0.3.5/tests/test_task_list/multiple.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 21:23:47.403093 inspect_ai-0.3.5/tests/test_task_list/multiple_dir/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 21:23:47.403093 inspect_ai-0.3.5/tests/test_task_list/multiple_dir/_decoy/
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-04 21:23:42.000000 inspect_ai-0.3.5/tests/test_task_list/multiple_dir/_decoy/testit.py
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-04 21:23:42.000000 inspect_ai-0.3.5/tests/test_task_list/multiple_dir/_decoy2.py
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-04 21:23:42.000000 inspect_ai-0.3.5/tests/test_task_list/multiple_dir/bar.py
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-04 21:23:42.000000 inspect_ai-0.3.5/tests/test_task_list/multiple_dir/foo.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 21:23:47.343093 inspect_ai-0.3.5/tests/test_task_list/recurse/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 21:23:47.403093 inspect_ai-0.3.5/tests/test_task_list/recurse/.folder3/
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-04 21:23:42.000000 inspect_ai-0.3.5/tests/test_task_list/recurse/.folder3/epsilon.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 21:23:47.403093 inspect_ai-0.3.5/tests/test_task_list/recurse/folder1/
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-04 21:23:42.000000 inspect_ai-0.3.5/tests/test_task_list/recurse/folder1/_decoy.py
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-04 21:23:42.000000 inspect_ai-0.3.5/tests/test_task_list/recurse/folder1/theta.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 21:23:47.403093 inspect_ai-0.3.5/tests/test_task_list/recurse/folder2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 21:23:47.403093 inspect_ai-0.3.5/tests/test_task_list/recurse/folder2/.folder3/
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-04 21:23:42.000000 inspect_ai-0.3.5/tests/test_task_list/recurse/folder2/.folder3/epsilon.py
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-04 21:23:42.000000 inspect_ai-0.3.5/tests/test_task_list/recurse/folder2/another.py
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-04 21:23:42.000000 inspect_ai-0.3.5/tests/test_task_list/recurse/folder2/first.py
--rw-r--r--   0 runner    (1001) docker     (127)     5420 2024-05-04 21:23:42.000000 inspect_ai-0.3.5/tests/test_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     1838 2024-05-04 21:23:42.000000 inspect_ai-0.3.5/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:23:28.605315 inspect_ai-0.3.6/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:23:28.541315 inspect_ai-0.3.6/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:23:28.541315 inspect_ai-0.3.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      544 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/.github/workflows/pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3194 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:23:28.541315 inspect_ai-0.3.6/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/.vscode/extensions.json
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3617 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4148 2024-05-06 20:23:28.601315 inspect_ai-0.3.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:23:28.541315 inspect_ai-0.3.6/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/benchmarks/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/benchmarks/arc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:23:28.545315 inspect_ai-0.3.6/benchmarks/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/benchmarks/datasets/math_test.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/benchmarks/datasets/mmlu.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/benchmarks/gpqa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2453 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/benchmarks/gsm8k.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/benchmarks/hellaswag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3555 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/benchmarks/mathematics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6930 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/benchmarks/mmlu.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:23:28.545315 inspect_ai-0.3.6/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/docs/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:23:28.549315 inspect_ai-0.3.6/docs/_examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     4560 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/docs/_examples/arc.qmd
+-rw-r--r--   0 runner    (1001) docker     (127)     3010 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/docs/_examples/biology_qa.qmd
+-rw-r--r--   0 runner    (1001) docker     (127)      998 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/docs/_examples/footer.qmd
+-rw-r--r--   0 runner    (1001) docker     (127)     5579 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/docs/_examples/gsm8k.qmd
+-rw-r--r--   0 runner    (1001) docker     (127)     3234 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/docs/_examples/hellaswag.qmd
+-rw-r--r--   0 runner    (1001) docker     (127)     2624 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/docs/_examples/index.qmd
+-rw-r--r--   0 runner    (1001) docker     (127)     6808 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/docs/_examples/mathematics.qmd
+-rw-r--r--   0 runner    (1001) docker     (127)     2992 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/docs/_examples/popularity.qmd
+-rw-r--r--   0 runner    (1001) docker     (127)     2153 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/docs/_examples/security_guide.qmd
+-rw-r--r--   0 runner    (1001) docker     (127)     2158 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/docs/_examples/theory_of_mind.qmd
+-rw-r--r--   0 runner    (1001) docker     (127)     4655 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/docs/_examples/tool_use.qmd
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:23:28.549315 inspect_ai-0.3.6/docs/_format/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      364 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/docs/_format/pre-render.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     2504 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/docs/_quarto.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/docs/_variables.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    11333 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/docs/datasets.qmd
+-rw-r--r--   0 runner    (1001) docker     (127)     9905 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/docs/eval-logs.qmd
+-rw-r--r--   0 runner    (1001) docker     (127)     8386 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/docs/eval-suites.qmd
+-rw-r--r--   0 runner    (1001) docker     (127)    10373 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/docs/eval-tuning.qmd
+-rw-r--r--   0 runner    (1001) docker     (127)    35808 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/docs/examples.qmd
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:23:28.557315 inspect_ai-0.3.6/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (127)   170128 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/docs/images/aisi-logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)    68030 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/docs/images/eval-log.png
+-rw-r--r--   0 runner    (1001) docker     (127)   314093 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/docs/images/inspect-view-answers.png
+-rw-r--r--   0 runner    (1001) docker     (127)   280184 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/docs/images/inspect-view-filter.png
+-rw-r--r--   0 runner    (1001) docker     (127)   284131 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/docs/images/inspect-view-history.png
+-rw-r--r--   0 runner    (1001) docker     (127)   413188 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/docs/images/inspect-view-home.png
+-rw-r--r--   0 runner    (1001) docker     (127)   241738 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/docs/images/inspect-view-info.png
+-rw-r--r--   0 runner    (1001) docker     (127)   143202 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/docs/images/inspect-view-logging-console.png
+-rw-r--r--   0 runner    (1001) docker     (127)   155304 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/docs/images/inspect-view-logging.png
+-rw-r--r--   0 runner    (1001) docker     (127)   373146 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/docs/images/inspect-view-main.png
+-rw-r--r--   0 runner    (1001) docker     (127)   321793 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/docs/images/inspect-view-messages.png
+-rw-r--r--   0 runner    (1001) docker     (127)   165394 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/docs/images/inspect-view-metadata.png
+-rw-r--r--   0 runner    (1001) docker     (127)   272733 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/docs/images/inspect-view-scoring.png
+-rw-r--r--   0 runner    (1001) docker     (127)   274383 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/docs/images/inspect-view-sort.png
+-rw-r--r--   0 runner    (1001) docker     (127)    90624 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/docs/images/inspect-view-splash.png
+-rw-r--r--   0 runner    (1001) docker     (127)    68787 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/docs/images/popularity.png
+-rw-r--r--   0 runner    (1001) docker     (127)    54252 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/docs/images/rate-limit.png
+-rw-r--r--   0 runner    (1001) docker     (127)    48461 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/docs/images/running-theory.png
+-rw-r--r--   0 runner    (1001) docker     (127)    10437 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/docs/index.qmd
+-rw-r--r--   0 runner    (1001) docker     (127)     9421 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/docs/log-viewer.qmd
+-rw-r--r--   0 runner    (1001) docker     (127)    18564 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/docs/models.qmd
+-rw-r--r--   0 runner    (1001) docker     (127)    15801 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/docs/scorers.qmd
+-rw-r--r--   0 runner    (1001) docker     (127)    14283 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/docs/solvers.qmd
+-rw-r--r--   0 runner    (1001) docker     (127)      825 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/docs/theme.scss
+-rw-r--r--   0 runner    (1001) docker     (127)    15937 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/docs/tools.qmd
+-rw-r--r--   0 runner    (1001) docker     (127)    12752 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/docs/workflow.qmd
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:23:28.557315 inspect_ai-0.3.6/examples/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:23:28.533316 inspect_ai-0.3.6/examples/agents/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:23:28.557315 inspect_ai-0.3.6/examples/agents/langchain/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/examples/agents/langchain/.env.example
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/examples/agents/langchain/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     2029 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/examples/agents/langchain/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     8266 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/examples/agents/langchain/inspect_langchain.py
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/examples/agents/langchain/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/examples/agents/langchain/wikipedia.jsonl
+-rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/examples/agents/langchain/wikipedia.py
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/examples/biology_qa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/examples/popularity.py
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/examples/security_guide.py
+-rw-r--r--   0 runner    (1001) docker     (127)      514 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/examples/theory_of_mind.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1980 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/examples/tool_use.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2988 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 20:23:28.605315 inspect_ai-0.3.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:23:28.533316 inspect_ai-0.3.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:23:28.561315 inspect_ai-0.3.6/src/inspect_ai/
+-rw-r--r--   0 runner    (1001) docker     (127)      671 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:23:28.561315 inspect_ai-0.3.6/src/inspect_ai/_cli/
+-rw-r--r--   0 runner    (1001) docker     (127)     1705 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_cli/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7639 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_cli/eval.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_cli/info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3716 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_cli/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2807 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_cli/score.py
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_cli/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      942 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_cli/view.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:23:28.561315 inspect_ai-0.3.6/src/inspect_ai/_display/
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_display/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_display/_display.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2720 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_display/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11708 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_display/rich.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:23:28.565315 inspect_ai-0.3.6/src/inspect_ai/_eval/
+-rw-r--r--   0 runner    (1001) docker     (127)    16214 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_eval/eval.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1767 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_eval/images.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11631 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_eval/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2347 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_eval/loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3653 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_eval/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3998 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_eval/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5586 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_eval/score.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22961 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_eval/task.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:23:28.569315 inspect_ai-0.3.6/src/inspect_ai/_util/
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_util/appdirs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_util/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_util/datetime.py
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_util/dev.py
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_util/docstring.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3040 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_util/dotenv.py
+-rw-r--r--   0 runner    (1001) docker     (127)      737 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_util/error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5969 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_util/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)      886 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_util/git.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3628 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_util/http.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_util/images.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_util/json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2998 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_util/notebook.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2160 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_util/path.py
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_util/pattern.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_util/platform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8512 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_util/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2038 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_util/retry.py
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_util/samples.py
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_util/text.py
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_util/url.py
+-rw-r--r--   0 runner    (1001) docker     (127)      491 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_util/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:23:28.569315 inspect_ai-0.3.6/src/inspect_ai/_view/
+-rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_view/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8607 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_view/view.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:23:28.569315 inspect_ai-0.3.6/src/inspect_ai/_view/www/
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_view/www/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    10102 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_view/www/App.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_view/www/api.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_view/www/favicon.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     2231 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_view/www/index.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:23:28.569315 inspect_ai-0.3.6/src/inspect_ai/_view/www/libs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:23:28.533316 inspect_ai-0.3.6/src/inspect_ai/_view/www/libs/bootstrap/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:23:28.569315 inspect_ai-0.3.6/src/inspect_ai/_view/www/libs/bootstrap/css/
+-rw-r--r--   0 runner    (1001) docker     (127)    85877 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_view/www/libs/bootstrap/css/bootstrap-icons.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)   232903 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_view/www/libs/bootstrap/css/bootstrap.min.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:23:28.569315 inspect_ai-0.3.6/src/inspect_ai/_view/www/libs/bootstrap/css/fonts/
+-rw-r--r--   0 runner    (1001) docker     (127)   176196 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_view/www/libs/bootstrap/css/fonts/bootstrap-icons.woff
+-rw-r--r--   0 runner    (1001) docker     (127)   130764 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_view/www/libs/bootstrap/css/fonts/bootstrap-icons.woff2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:23:28.573315 inspect_ai-0.3.6/src/inspect_ai/_view/www/libs/bootstrap/js/
+-rw-r--r--   0 runner    (1001) docker     (127)    80615 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_view/www/libs/bootstrap/js/bootstrap.bundle.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)     9160 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_view/www/libs/clipboard.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    31629 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_view/www/libs/json5.min.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:23:28.573315 inspect_ai-0.3.6/src/inspect_ai/_view/www/libs/prism/
+-rw-r--r--   0 runner    (1001) docker     (127)     3481 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_view/www/libs/prism/prism-dark.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1896 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_view/www/libs/prism/prism.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)    16934 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_view/www/libs/prism/prism.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    21104 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_view/www/libs/purify.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    75207 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_view/www/libs/showdown.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    34863 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_view/www/log-schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8721 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_view/www/log.d.ts
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:23:28.573315 inspect_ai-0.3.6/src/inspect_ai/_view/www/preact/
+-rw-r--r--   0 runner    (1001) docker     (127)     3669 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_view/www/preact/hooks.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:23:28.573315 inspect_ai-0.3.6/src/inspect_ai/_view/www/preact/htm/
+-rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_view/www/preact/htm/htm.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_view/www/preact/htm/preact.js
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_view/www/preact/htm/preact.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_view/www/preact/preact-hooks.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)    11268 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_view/www/preact/preact.mjs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:23:28.573315 inspect_ai-0.3.6/src/inspect_ai/_view/www/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     7233 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_view/www/src/App.css
+-rw-r--r--   0 runner    (1001) docker     (127)     2701 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_view/www/src/Constants.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_view/www/src/Register.mjs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:23:28.577315 inspect_ai-0.3.6/src/inspect_ai/_view/www/src/components/
+-rw-r--r--   0 runner    (1001) docker     (127)      994 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_view/www/src/components/AnsiDisplay.css
+-rw-r--r--   0 runner    (1001) docker     (127)     4058 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_view/www/src/components/AnsiDisplay.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)      869 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_view/www/src/components/AppErrorBoundary.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)     2248 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_view/www/src/components/Card.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)     5498 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_view/www/src/components/ChatView.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_view/www/src/components/CopyButton.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_view/www/src/components/Dialog.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_view/www/src/components/EmptyPanel.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_view/www/src/components/ErrorPanel.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_view/www/src/components/LabeledValue.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)      833 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_view/www/src/components/LoadingScreen.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_view/www/src/components/MarkdownDiv.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)     1595 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_view/www/src/components/MessageContent.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)     2101 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_view/www/src/components/MetaDataView.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)     6941 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_view/www/src/components/RenderedContent.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)     2745 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_view/www/src/components/TabSet.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_view/www/src/components/ToolButton.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)    20289 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_view/www/src/components/ansi-output.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:23:28.577315 inspect_ai-0.3.6/src/inspect_ai/_view/www/src/log-reader/
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_view/www/src/log-reader/Log-Reader.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_view/www/src/log-reader/Native-Log-Reader.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)     8046 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_view/www/src/log-reader/Open-AI-Log-Reader.mjs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:23:28.577315 inspect_ai-0.3.6/src/inspect_ai/_view/www/src/logging/
+-rw-r--r--   0 runner    (1001) docker     (127)     2946 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_view/www/src/logging/LoggingPanel.mjs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:23:28.577315 inspect_ai-0.3.6/src/inspect_ai/_view/www/src/plan/
+-rw-r--r--   0 runner    (1001) docker     (127)     8260 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_view/www/src/plan/PlanCard.mjs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:23:28.577315 inspect_ai-0.3.6/src/inspect_ai/_view/www/src/samples/
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_view/www/src/samples/SampleGroupSeparator.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)     3249 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_view/www/src/samples/SampleScoreView.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)     8207 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_view/www/src/samples/SampleView.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)     4467 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_view/www/src/samples/SamplesCard.mjs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:23:28.577315 inspect_ai-0.3.6/src/inspect_ai/_view/www/src/title/
+-rw-r--r--   0 runner    (1001) docker     (127)     5378 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_view/www/src/title/TitleBlock.mjs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:23:28.577315 inspect_ai-0.3.6/src/inspect_ai/_view/www/src/usage/
+-rw-r--r--   0 runner    (1001) docker     (127)     1281 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_view/www/src/usage/ModelTokenTable.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)     1890 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_view/www/src/usage/UsageCard.mjs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:23:28.581315 inspect_ai-0.3.6/src/inspect_ai/_view/www/src/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     3072 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_view/www/src/utils/Format.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_view/www/src/utils/Git.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_view/www/src/utils/Path.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_view/www/src/utils/Type.mjs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:23:28.581315 inspect_ai-0.3.6/src/inspect_ai/_view/www/src/workspace/
+-rw-r--r--   0 runner    (1001) docker     (127)      822 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_view/www/src/workspace/EpochFilter.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)     4853 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_view/www/src/workspace/SampleFilter.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)     7027 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_view/www/src/workspace/SamplesDescriptor.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)     2684 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_view/www/src/workspace/SortFilter.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_view/www/src/workspace/TaskErrorPanel.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)    15380 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_view/www/src/workspace/WorkSpace.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)     8721 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/_view/www/tools.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:23:28.581315 inspect_ai-0.3.6/src/inspect_ai/dataset/
+-rw-r--r--   0 runner    (1001) docker     (127)      534 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7465 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/dataset/_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:23:28.581315 inspect_ai-0.3.6/src/inspect_ai/dataset/_examples/
+-rw-r--r--   0 runner    (1001) docker     (127)    20756 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/dataset/_examples/bias_detection.jsonl
+-rw-r--r--   0 runner    (1001) docker     (127)     2009 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/dataset/_examples/biology_qa.jsonl
+-rw-r--r--   0 runner    (1001) docker     (127)    32773 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/dataset/_examples/popularity.jsonl
+-rw-r--r--   0 runner    (1001) docker     (127)     2659 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/dataset/_examples/security_guide.jsonl
+-rw-r--r--   0 runner    (1001) docker     (127)    31831 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/dataset/_examples/theory_of_mind.jsonl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:23:28.581315 inspect_ai-0.3.6/src/inspect_ai/dataset/_sources/
+-rw-r--r--   0 runner    (1001) docker     (127)     3035 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/dataset/_sources/csv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1702 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/dataset/_sources/example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2557 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/dataset/_sources/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3559 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/dataset/_sources/hf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3335 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/dataset/_sources/json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3766 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/dataset/_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:23:28.585315 inspect_ai-0.3.6/src/inspect_ai/log/
+-rw-r--r--   0 runner    (1001) docker     (127)      776 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/log/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10183 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/log/_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9174 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/log/_log.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:23:28.585315 inspect_ai-0.3.6/src/inspect_ai/model/
+-rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31683 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/model/_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:23:28.585315 inspect_ai-0.3.6/src/inspect_ai/model/_providers/
+-rw-r--r--   0 runner    (1001) docker     (127)    29724 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/model/_providers/anthropic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7885 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/model/_providers/azureai.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10818 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/model/_providers/bedrock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3043 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/model/_providers/cloudflare.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10170 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/model/_providers/google.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10061 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/model/_providers/hf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7859 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/model/_providers/mistral.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13476 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/model/_providers/openai.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3298 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/model/_providers/providers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      990 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/model/_providers/together.py
+-rw-r--r--   0 runner    (1001) docker     (127)      857 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/model/_providers/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2426 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/model/_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/model/_tool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4749 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/model/_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:23:28.589315 inspect_ai-0.3.6/src/inspect_ai/scorer/
+-rw-r--r--   0 runner    (1001) docker     (127)      893 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/scorer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2054 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/scorer/_answer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2717 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/scorer/_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1686 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/scorer/_match.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7209 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/scorer/_metric.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:23:28.589315 inspect_ai-0.3.6/src/inspect_ai/scorer/_metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/scorer/_metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      943 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/scorer/_metrics/accuracy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      555 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/scorer/_metrics/mean.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/scorer/_metrics/std.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7089 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/scorer/_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1802 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/scorer/_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4362 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/scorer/_scorer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:23:28.589315 inspect_ai-0.3.6/src/inspect_ai/solver/
+-rw-r--r--   0 runner    (1001) docker     (127)      671 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/solver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3100 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/solver/_critique.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6146 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/solver/_multiple_choice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5189 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/solver/_plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2292 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/solver/_prompt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8101 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/solver/_solver.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:23:28.589315 inspect_ai-0.3.6/src/inspect_ai/solver/_tool/
+-rw-r--r--   0 runner    (1001) docker     (127)     3810 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/solver/_tool/tool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2434 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/solver/_tool/tool_def.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1680 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/solver/_tool/use_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7376 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/solver/_tool/web_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/solver/_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:23:28.589315 inspect_ai-0.3.6/src/inspect_ai/util/
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/util/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:23:28.593315 inspect_ai-0.3.6/src/inspect_ai/util/_context/
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/util/_context/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2777 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/util/_context/concurrency.py
+-rw-r--r--   0 runner    (1001) docker     (127)      690 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/util/_context/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3146 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/util/_context/resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4734 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/src/inspect_ai/util/_context/subprocess.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:23:28.601315 inspect_ai-0.3.6/src/inspect_ai.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4148 2024-05-06 20:23:28.000000 inspect_ai-0.3.6/src/inspect_ai.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10858 2024-05-06 20:23:28.000000 inspect_ai-0.3.6/src/inspect_ai.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 20:23:28.000000 inspect_ai-0.3.6/src/inspect_ai.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-06 20:23:28.000000 inspect_ai-0.3.6/src/inspect_ai.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-05-06 20:23:28.000000 inspect_ai-0.3.6/src/inspect_ai.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-06 20:23:28.000000 inspect_ai-0.3.6/src/inspect_ai.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:23:28.597315 inspect_ai-0.3.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/tests/test_anthropic.py
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/tests/test_cloudlfare.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1730 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/tests/test_collapse_user_message.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:23:28.597315 inspect_ai-0.3.6/tests/test_dataset/
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/tests/test_dataset/samples.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/tests/test_dataset/samples.json
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/tests/test_dataset/samples.jsonl
+-rw-r--r--   0 runner    (1001) docker     (127)     2206 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/tests/test_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      881 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/tests/test_eval_log.py
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/tests/test_examples.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/tests/test_hf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:23:28.597315 inspect_ai-0.3.6/tests/test_images/
+-rw-r--r--   0 runner    (1001) docker     (127)   732622 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/tests/test_images/images.jsonl
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/tests/test_images.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/tests/test_list_task.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/tests/test_logprobs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3112 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/tests/test_metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)      920 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/tests/test_num_choices.py
+-rw-r--r--   0 runner    (1001) docker     (127)      746 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/tests/test_openai.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/tests/test_plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)      728 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/tests/test_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/tests/test_retry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/tests/test_scorer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1897 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/tests/test_solver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/tests/test_stop_reason.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/tests/test_subprocess.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:23:28.597315 inspect_ai-0.3.6/tests/test_task_list/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/tests/test_task_list/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/tests/test_task_list/attribs.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/tests/test_task_list/multiple.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:23:28.597315 inspect_ai-0.3.6/tests/test_task_list/multiple_dir/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:23:28.597315 inspect_ai-0.3.6/tests/test_task_list/multiple_dir/_decoy/
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/tests/test_task_list/multiple_dir/_decoy/testit.py
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/tests/test_task_list/multiple_dir/_decoy2.py
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/tests/test_task_list/multiple_dir/bar.py
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/tests/test_task_list/multiple_dir/foo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:23:28.537315 inspect_ai-0.3.6/tests/test_task_list/recurse/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:23:28.597315 inspect_ai-0.3.6/tests/test_task_list/recurse/.folder3/
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/tests/test_task_list/recurse/.folder3/epsilon.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:23:28.597315 inspect_ai-0.3.6/tests/test_task_list/recurse/folder1/
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/tests/test_task_list/recurse/folder1/_decoy.py
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/tests/test_task_list/recurse/folder1/theta.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:23:28.601315 inspect_ai-0.3.6/tests/test_task_list/recurse/folder2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:23:28.601315 inspect_ai-0.3.6/tests/test_task_list/recurse/folder2/.folder3/
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/tests/test_task_list/recurse/folder2/.folder3/epsilon.py
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/tests/test_task_list/recurse/folder2/another.py
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/tests/test_task_list/recurse/folder2/first.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5420 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/tests/test_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1838 2024-05-06 20:23:23.000000 inspect_ai-0.3.6/tests/utils.py
```

### Comparing `inspect_ai-0.3.5/.github/workflows/build.yml` & `inspect_ai-0.3.6/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/.github/workflows/docs.yml` & `inspect_ai-0.3.6/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/.github/workflows/pypi.yml` & `inspect_ai-0.3.6/.github/workflows/pypi.yml`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/.gitignore` & `inspect_ai-0.3.6/.gitignore`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/.pre-commit-config.yaml` & `inspect_ai-0.3.6/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/CHANGELOG.md` & `inspect_ai-0.3.6/CHANGELOG.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,15 @@
 # Changelog
 
+## v0.3.6 (06 May 2024)
+
+- Show first log file immediately (don't wait for fetching metadata for other logs)
+- Add `--version` CLI arg and `inspect info version` command for interogating version and runtime source path.
+- Fix: exclude `null` config values in output from `inspect info log-file`
+
 ## v0.3.5 (04 May 2024)
 
 - Fix issue with logs from S3 buckets in inspect view.
 - Add `sort()` method to `Dataset` (defaults to sorting by sample input length).
 - Improve tokenization for HF provider (left padding, attention mask, and allow for custom chat template)
 - Improve batching for HF provider (generate as soon as queue fills, thread safety for future.set_result).
 - Various improvements to documentation.
```

### Comparing `inspect_ai-0.3.5/LICENSE` & `inspect_ai-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/PKG-INFO` & `inspect_ai-0.3.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inspect_ai
-Version: 0.3.5
+Version: 0.3.6
 Summary: Framework for large language model evaluations
 Author: UK AI Safety Institute
 License: MIT License
 Project-URL: Documentation, https://UKGovernmentBEIS.github.io/inspect_ai/
 Project-URL: Source Code, https://github.com/UKGovernmentBEIS/inspect_ai
 Project-URL: Issue Tracker, https://github.com/UKGovernmentBEIS/inspect_ai/issues
 Classifier: Development Status :: 4 - Beta
```

### Comparing `inspect_ai-0.3.5/README.md` & `inspect_ai-0.3.6/README.md`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/benchmarks/README.md` & `inspect_ai-0.3.6/benchmarks/README.md`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/benchmarks/arc.py` & `inspect_ai-0.3.6/benchmarks/arc.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/benchmarks/gpqa.py` & `inspect_ai-0.3.6/benchmarks/gpqa.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/benchmarks/gsm8k.py` & `inspect_ai-0.3.6/benchmarks/gsm8k.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/benchmarks/hellaswag.py` & `inspect_ai-0.3.6/benchmarks/hellaswag.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/benchmarks/mathematics.py` & `inspect_ai-0.3.6/benchmarks/mathematics.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/benchmarks/mmlu.py` & `inspect_ai-0.3.6/benchmarks/mmlu.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/docs/_examples/arc.qmd` & `inspect_ai-0.3.6/docs/_examples/arc.qmd`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/docs/_examples/biology_qa.qmd` & `inspect_ai-0.3.6/docs/_examples/biology_qa.qmd`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/docs/_examples/footer.qmd` & `inspect_ai-0.3.6/docs/_examples/footer.qmd`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/docs/_examples/gsm8k.qmd` & `inspect_ai-0.3.6/docs/_examples/gsm8k.qmd`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/docs/_examples/hellaswag.qmd` & `inspect_ai-0.3.6/docs/_examples/hellaswag.qmd`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/docs/_examples/index.qmd` & `inspect_ai-0.3.6/docs/_examples/index.qmd`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/docs/_examples/mathematics.qmd` & `inspect_ai-0.3.6/docs/_examples/mathematics.qmd`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/docs/_examples/popularity.qmd` & `inspect_ai-0.3.6/docs/_examples/popularity.qmd`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/docs/_examples/security_guide.qmd` & `inspect_ai-0.3.6/docs/_examples/security_guide.qmd`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/docs/_examples/theory_of_mind.qmd` & `inspect_ai-0.3.6/docs/_examples/theory_of_mind.qmd`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/docs/_examples/tool_use.qmd` & `inspect_ai-0.3.6/docs/_examples/tool_use.qmd`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/docs/_quarto.yml` & `inspect_ai-0.3.6/docs/_quarto.yml`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/docs/datasets.qmd` & `inspect_ai-0.3.6/docs/datasets.qmd`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/docs/eval-logs.qmd` & `inspect_ai-0.3.6/docs/eval-logs.qmd`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/docs/eval-suites.qmd` & `inspect_ai-0.3.6/docs/eval-suites.qmd`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/docs/eval-tuning.qmd` & `inspect_ai-0.3.6/docs/eval-tuning.qmd`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/docs/examples.qmd` & `inspect_ai-0.3.6/docs/examples.qmd`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/docs/images/aisi-logo.png` & `inspect_ai-0.3.6/docs/images/aisi-logo.png`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/docs/images/eval-log.png` & `inspect_ai-0.3.6/docs/images/eval-log.png`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/docs/images/inspect-view-answers.png` & `inspect_ai-0.3.6/docs/images/inspect-view-answers.png`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/docs/images/inspect-view-filter.png` & `inspect_ai-0.3.6/docs/images/inspect-view-filter.png`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/docs/images/inspect-view-history.png` & `inspect_ai-0.3.6/docs/images/inspect-view-history.png`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/docs/images/inspect-view-home.png` & `inspect_ai-0.3.6/docs/images/inspect-view-home.png`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/docs/images/inspect-view-info.png` & `inspect_ai-0.3.6/docs/images/inspect-view-info.png`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/docs/images/inspect-view-logging-console.png` & `inspect_ai-0.3.6/docs/images/inspect-view-logging-console.png`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/docs/images/inspect-view-logging.png` & `inspect_ai-0.3.6/docs/images/inspect-view-logging.png`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/docs/images/inspect-view-main.png` & `inspect_ai-0.3.6/docs/images/inspect-view-main.png`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/docs/images/inspect-view-messages.png` & `inspect_ai-0.3.6/docs/images/inspect-view-messages.png`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/docs/images/inspect-view-metadata.png` & `inspect_ai-0.3.6/docs/images/inspect-view-metadata.png`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/docs/images/inspect-view-scoring.png` & `inspect_ai-0.3.6/docs/images/inspect-view-scoring.png`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/docs/images/inspect-view-sort.png` & `inspect_ai-0.3.6/docs/images/inspect-view-sort.png`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/docs/images/inspect-view-splash.png` & `inspect_ai-0.3.6/docs/images/inspect-view-splash.png`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/docs/images/popularity.png` & `inspect_ai-0.3.6/docs/images/popularity.png`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/docs/images/rate-limit.png` & `inspect_ai-0.3.6/docs/images/rate-limit.png`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/docs/images/running-theory.png` & `inspect_ai-0.3.6/docs/images/running-theory.png`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/docs/index.qmd` & `inspect_ai-0.3.6/docs/index.qmd`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/docs/log-viewer.qmd` & `inspect_ai-0.3.6/docs/log-viewer.qmd`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/docs/models.qmd` & `inspect_ai-0.3.6/docs/models.qmd`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/docs/scorers.qmd` & `inspect_ai-0.3.6/docs/scorers.qmd`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/docs/solvers.qmd` & `inspect_ai-0.3.6/docs/solvers.qmd`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/docs/theme.scss` & `inspect_ai-0.3.6/docs/theme.scss`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/docs/tools.qmd` & `inspect_ai-0.3.6/docs/tools.qmd`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/docs/workflow.qmd` & `inspect_ai-0.3.6/docs/workflow.qmd`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/examples/agents/langchain/README.md` & `inspect_ai-0.3.6/examples/agents/langchain/README.md`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/examples/agents/langchain/inspect_langchain.py` & `inspect_ai-0.3.6/examples/agents/langchain/inspect_langchain.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/examples/agents/langchain/wikipedia.jsonl` & `inspect_ai-0.3.6/examples/agents/langchain/wikipedia.jsonl`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/examples/agents/langchain/wikipedia.py` & `inspect_ai-0.3.6/examples/agents/langchain/wikipedia.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/examples/biology_qa.py` & `inspect_ai-0.3.6/examples/biology_qa.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/examples/popularity.py` & `inspect_ai-0.3.6/examples/popularity.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/examples/security_guide.py` & `inspect_ai-0.3.6/examples/security_guide.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/examples/theory_of_mind.py` & `inspect_ai-0.3.6/examples/theory_of_mind.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/examples/tool_use.py` & `inspect_ai-0.3.6/examples/tool_use.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/pyproject.toml` & `inspect_ai-0.3.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/src/inspect_ai/__init__.py` & `inspect_ai-0.3.6/src/inspect_ai/__init__.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/src/inspect_ai/_cli/common.py` & `inspect_ai-0.3.6/src/inspect_ai/_cli/common.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/src/inspect_ai/_cli/eval.py` & `inspect_ai-0.3.6/src/inspect_ai/_cli/eval.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/src/inspect_ai/_cli/info.py` & `inspect_ai-0.3.6/src/inspect_ai/_cli/info.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,32 +1,51 @@
+from json import dumps
+
 import click
 
+from inspect_ai import __version__
 from inspect_ai._util.constants import PKG_PATH
-from inspect_ai.log import read_eval_log
+from inspect_ai.log import eval_log_json, read_eval_log
 
 
 @click.group("info")
 def info_command() -> None:
     """Read configuration and log info."""
     return None
 
 
+@info_command.command("version")
+@click.option(
+    "--json",
+    type=bool,
+    is_flag=True,
+    default=False,
+    help="Output version and path info as JSON",
+)
+def version(json: bool) -> None:
+    if json:
+        print(dumps(dict(version=__version__, path=PKG_PATH.as_posix()), indent=2))
+    else:
+        print(f"version: {__version__}")
+        print(f"path: {PKG_PATH.as_posix()}")
+
+
 @info_command.command("log-file")
 @click.argument("path")
 @click.option(
     "--header-only",
     type=bool,
     is_flag=True,
     default=False,
     help="Read and print only the header of the log file (i.e. no samples).",
 )
 def log(path: str, header_only: bool) -> None:
     """Print log file contents."""
     log = read_eval_log(path, header_only=header_only)
-    print(log.model_dump_json(indent=2))
+    print(eval_log_json(log))
 
 
 @info_command.command("log-schema")
 def log_schema() -> None:
     """Print JSON schema for log files."""
     print(view_resource("log-schema.json"))
 
@@ -34,10 +53,10 @@
 @info_command.command("log-types")
 def log_types() -> None:
     """Print TS declarations for log files."""
     print(view_resource("log.d.ts"))
 
 
 def view_resource(file: str) -> str:
-    resource = PKG_PATH / "src" / "inspect_ai" / "_view" / "www" / file
+    resource = PKG_PATH / "_view" / "www" / file
     with open(resource, "r", encoding="utf-8") as f:
         return f.read()
```

### Comparing `inspect_ai-0.3.5/src/inspect_ai/_cli/list.py` & `inspect_ai-0.3.6/src/inspect_ai/_cli/list.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/src/inspect_ai/_cli/score.py` & `inspect_ai-0.3.6/src/inspect_ai/_cli/score.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/src/inspect_ai/_cli/util.py` & `inspect_ai-0.3.6/src/inspect_ai/_cli/util.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/src/inspect_ai/_cli/view.py` & `inspect_ai-0.3.6/src/inspect_ai/_cli/view.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/src/inspect_ai/_display/_display.py` & `inspect_ai-0.3.6/src/inspect_ai/_display/_display.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/src/inspect_ai/_display/logger.py` & `inspect_ai-0.3.6/src/inspect_ai/_display/logger.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/src/inspect_ai/_display/rich.py` & `inspect_ai-0.3.6/src/inspect_ai/_display/rich.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/src/inspect_ai/_eval/eval.py` & `inspect_ai-0.3.6/src/inspect_ai/_eval/eval.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/src/inspect_ai/_eval/images.py` & `inspect_ai-0.3.6/src/inspect_ai/_eval/images.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/src/inspect_ai/_eval/list.py` & `inspect_ai-0.3.6/src/inspect_ai/_eval/list.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/src/inspect_ai/_eval/loader.py` & `inspect_ai-0.3.6/src/inspect_ai/_eval/loader.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/src/inspect_ai/_eval/log.py` & `inspect_ai-0.3.6/src/inspect_ai/_eval/log.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/src/inspect_ai/_eval/registry.py` & `inspect_ai-0.3.6/src/inspect_ai/_eval/registry.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/src/inspect_ai/_eval/score.py` & `inspect_ai-0.3.6/src/inspect_ai/_eval/score.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/src/inspect_ai/_eval/task.py` & `inspect_ai-0.3.6/src/inspect_ai/_eval/task.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/src/inspect_ai/_util/dotenv.py` & `inspect_ai-0.3.6/src/inspect_ai/_util/dotenv.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/src/inspect_ai/_util/error.py` & `inspect_ai-0.3.6/src/inspect_ai/_util/error.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/src/inspect_ai/_util/file.py` & `inspect_ai-0.3.6/src/inspect_ai/_util/file.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/src/inspect_ai/_util/git.py` & `inspect_ai-0.3.6/src/inspect_ai/_util/git.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/src/inspect_ai/_util/http.py` & `inspect_ai-0.3.6/src/inspect_ai/_util/http.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/src/inspect_ai/_util/images.py` & `inspect_ai-0.3.6/src/inspect_ai/_util/images.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/src/inspect_ai/_util/json.py` & `inspect_ai-0.3.6/src/inspect_ai/_util/json.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/src/inspect_ai/_util/notebook.py` & `inspect_ai-0.3.6/src/inspect_ai/_util/notebook.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/src/inspect_ai/_util/path.py` & `inspect_ai-0.3.6/src/inspect_ai/_util/path.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/src/inspect_ai/_util/platform.py` & `inspect_ai-0.3.6/src/inspect_ai/_util/platform.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/src/inspect_ai/_util/registry.py` & `inspect_ai-0.3.6/src/inspect_ai/_util/registry.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/src/inspect_ai/_util/retry.py` & `inspect_ai-0.3.6/src/inspect_ai/_util/retry.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/src/inspect_ai/_util/url.py` & `inspect_ai-0.3.6/src/inspect_ai/_util/url.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/src/inspect_ai/_view/schema.py` & `inspect_ai-0.3.6/src/inspect_ai/_view/schema.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/src/inspect_ai/_view/view.py` & `inspect_ai-0.3.6/src/inspect_ai/_view/view.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/src/inspect_ai/_view/www/App.mjs` & `inspect_ai-0.3.6/src/inspect_ai/_view/www/App.mjs`

 * *Files 3% similar despite different names*

```diff
@@ -18,61 +18,60 @@
   const [logHeaders, setLogHeaders] = useState({});
   const [offcanvas, setOffcanvas] = useState(false);
 
   // reset selection when logs are refreshed
   useEffect(() => {
     // Default select the first item
     let index = 0;
-
     setSelected(index);
   }, [logs]);
 
-  useEffect(() => {
+  useEffect(async () => {
+    // Read header information for the logs
+    // and then update
+    const headerResults = await Promise.all(logs.files.map((file) => {
+        return eval_log(file.name, true).then((result) => {
+          return { file: file.name, result };
+        }).catch(() => { return undefined});
+    }));
+    
+    // Update the headers
+    const updatedHeaders = logHeaders;
+    for (const headerResult of headerResults) {
+      if (headerResult) {
+        updatedHeaders[headerResult.file] = headerResult.result;
+      }
+    }
+    setLogHeaders({ ...updatedHeaders });
+  }, [logs]);
+
+  useEffect(async () => {
     const urlParams = new URLSearchParams(window.location.search);
 
     // Note whether we should default off canvas the sidebar
     setOffcanvas(true);
 
     // If the URL provides a task file, load that
     const logPath = urlParams.get("task_file");
     const loadLogs = logPath
-      ? () => {
+      ? async () => {
           setLogs({
             log_dir: "",
             files: [{ name: logPath }],
           });
         }
-      : () => {
-          eval_logs().then((logresult) => {
-            // Set the list of logs
-            setLogs(logresult);
-
-            // Read header information for the logs
-            // and then update
-            const updatedHeaders = logHeaders;
-            Promise.all(
-              logresult.files.map(async (file) => {
-                try { 
-                  const result = await eval_log(file.name, true);
-                  return { file: file.name, result };
-                } catch { }
-              })
-            ).then((headerResults) => {
-              for (const headerResult of headerResults) {
-                if (headerResult) {
-                  updatedHeaders[headerResult.file] = headerResult.result;
-                }
-              }
-              setLogHeaders({ ...updatedHeaders });
-            });
-          });
+      : async () => {
+        // Set the list of logs
+          const logresult = await eval_logs();            
+          setLogs(logresult);
+
         };
 
     // initial fetch of logs
-    loadLogs();
+    await loadLogs();
 
     // poll every 1s for events
     setInterval(() => {
       client_events().then((events) => {
         if (events.includes("reload")) {
           window.location.reload(true);
         }
```

### Comparing `inspect_ai-0.3.5/src/inspect_ai/_view/www/api.mjs` & `inspect_ai-0.3.6/src/inspect_ai/_view/www/api.mjs`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/src/inspect_ai/_view/www/favicon.svg` & `inspect_ai-0.3.6/src/inspect_ai/_view/www/favicon.svg`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/src/inspect_ai/_view/www/index.html` & `inspect_ai-0.3.6/src/inspect_ai/_view/www/index.html`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/src/inspect_ai/_view/www/libs/bootstrap/css/bootstrap-icons.min.css` & `inspect_ai-0.3.6/src/inspect_ai/_view/www/libs/bootstrap/css/bootstrap-icons.min.css`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/src/inspect_ai/_view/www/libs/bootstrap/css/bootstrap.min.css` & `inspect_ai-0.3.6/src/inspect_ai/_view/www/libs/bootstrap/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/src/inspect_ai/_view/www/libs/bootstrap/css/fonts/bootstrap-icons.woff` & `inspect_ai-0.3.6/src/inspect_ai/_view/www/libs/bootstrap/css/fonts/bootstrap-icons.woff`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/src/inspect_ai/_view/www/libs/bootstrap/css/fonts/bootstrap-icons.woff2` & `inspect_ai-0.3.6/src/inspect_ai/_view/www/libs/bootstrap/css/fonts/bootstrap-icons.woff2`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/src/inspect_ai/_view/www/libs/bootstrap/js/bootstrap.bundle.min.js` & `inspect_ai-0.3.6/src/inspect_ai/_view/www/libs/bootstrap/js/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/src/inspect_ai/_view/www/libs/clipboard.min.js` & `inspect_ai-0.3.6/src/inspect_ai/_view/www/libs/clipboard.min.js`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/src/inspect_ai/_view/www/libs/json5.min.js` & `inspect_ai-0.3.6/src/inspect_ai/_view/www/libs/json5.min.js`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/src/inspect_ai/_view/www/libs/prism/prism-dark.css` & `inspect_ai-0.3.6/src/inspect_ai/_view/www/libs/prism/prism-dark.css`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/src/inspect_ai/_view/www/libs/prism/prism.min.css` & `inspect_ai-0.3.6/src/inspect_ai/_view/www/libs/prism/prism.min.css`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/src/inspect_ai/_view/www/libs/prism/prism.min.js` & `inspect_ai-0.3.6/src/inspect_ai/_view/www/libs/prism/prism.min.js`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/src/inspect_ai/_view/www/libs/purify.min.js` & `inspect_ai-0.3.6/src/inspect_ai/_view/www/libs/purify.min.js`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/src/inspect_ai/_view/www/libs/showdown.min.js` & `inspect_ai-0.3.6/src/inspect_ai/_view/www/libs/showdown.min.js`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/src/inspect_ai/_view/www/log-schema.json` & `inspect_ai-0.3.6/src/inspect_ai/_view/www/log-schema.json`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/src/inspect_ai/_view/www/log.d.ts` & `inspect_ai-0.3.6/src/inspect_ai/_view/www/log.d.ts`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/src/inspect_ai/_view/www/preact/hooks.js` & `inspect_ai-0.3.6/src/inspect_ai/_view/www/preact/hooks.js`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/src/inspect_ai/_view/www/preact/htm/htm.mjs` & `inspect_ai-0.3.6/src/inspect_ai/_view/www/preact/htm/htm.mjs`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/src/inspect_ai/_view/www/preact/preact.mjs` & `inspect_ai-0.3.6/src/inspect_ai/_view/www/preact/preact.mjs`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/src/inspect_ai/_view/www/src/App.css` & `inspect_ai-0.3.6/src/inspect_ai/_view/www/src/App.css`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/src/inspect_ai/_view/www/src/Constants.mjs` & `inspect_ai-0.3.6/src/inspect_ai/_view/www/src/Constants.mjs`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/src/inspect_ai/_view/www/src/components/AnsiDisplay.css` & `inspect_ai-0.3.6/src/inspect_ai/_view/www/src/components/AnsiDisplay.css`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/src/inspect_ai/_view/www/src/components/AnsiDisplay.mjs` & `inspect_ai-0.3.6/src/inspect_ai/_view/www/src/components/AnsiDisplay.mjs`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/src/inspect_ai/_view/www/src/components/AppErrorBoundary.mjs` & `inspect_ai-0.3.6/src/inspect_ai/_view/www/src/components/AppErrorBoundary.mjs`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/src/inspect_ai/_view/www/src/components/Card.mjs` & `inspect_ai-0.3.6/src/inspect_ai/_view/www/src/components/Card.mjs`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/src/inspect_ai/_view/www/src/components/ChatView.mjs` & `inspect_ai-0.3.6/src/inspect_ai/_view/www/src/components/ChatView.mjs`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/src/inspect_ai/_view/www/src/components/CopyButton.mjs` & `inspect_ai-0.3.6/src/inspect_ai/_view/www/src/components/CopyButton.mjs`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/src/inspect_ai/_view/www/src/components/Dialog.mjs` & `inspect_ai-0.3.6/src/inspect_ai/_view/www/src/components/Dialog.mjs`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/src/inspect_ai/_view/www/src/components/ErrorPanel.mjs` & `inspect_ai-0.3.6/src/inspect_ai/_view/www/src/components/ErrorPanel.mjs`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/src/inspect_ai/_view/www/src/components/LabeledValue.mjs` & `inspect_ai-0.3.6/src/inspect_ai/_view/www/src/components/LabeledValue.mjs`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/src/inspect_ai/_view/www/src/components/LoadingScreen.mjs` & `inspect_ai-0.3.6/src/inspect_ai/_view/www/src/components/LoadingScreen.mjs`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/src/inspect_ai/_view/www/src/components/MarkdownDiv.mjs` & `inspect_ai-0.3.6/src/inspect_ai/_view/www/src/components/MarkdownDiv.mjs`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/src/inspect_ai/_view/www/src/components/MessageContent.mjs` & `inspect_ai-0.3.6/src/inspect_ai/_view/www/src/components/MessageContent.mjs`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/src/inspect_ai/_view/www/src/components/MetaDataView.mjs` & `inspect_ai-0.3.6/src/inspect_ai/_view/www/src/components/MetaDataView.mjs`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/src/inspect_ai/_view/www/src/components/RenderedContent.mjs` & `inspect_ai-0.3.6/src/inspect_ai/_view/www/src/components/RenderedContent.mjs`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/src/inspect_ai/_view/www/src/components/TabSet.mjs` & `inspect_ai-0.3.6/src/inspect_ai/_view/www/src/components/TabSet.mjs`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/src/inspect_ai/_view/www/src/components/ansi-output.js` & `inspect_ai-0.3.6/src/inspect_ai/_view/www/src/components/ansi-output.js`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/src/inspect_ai/_view/www/src/log-reader/Log-Reader.mjs` & `inspect_ai-0.3.6/src/inspect_ai/_view/www/src/log-reader/Log-Reader.mjs`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/src/inspect_ai/_view/www/src/log-reader/Open-AI-Log-Reader.mjs` & `inspect_ai-0.3.6/src/inspect_ai/_view/www/src/log-reader/Open-AI-Log-Reader.mjs`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/src/inspect_ai/_view/www/src/logging/LoggingPanel.mjs` & `inspect_ai-0.3.6/src/inspect_ai/_view/www/src/logging/LoggingPanel.mjs`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/src/inspect_ai/_view/www/src/plan/PlanCard.mjs` & `inspect_ai-0.3.6/src/inspect_ai/_view/www/src/plan/PlanCard.mjs`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/src/inspect_ai/_view/www/src/samples/SampleScoreView.mjs` & `inspect_ai-0.3.6/src/inspect_ai/_view/www/src/samples/SampleScoreView.mjs`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/src/inspect_ai/_view/www/src/samples/SampleView.mjs` & `inspect_ai-0.3.6/src/inspect_ai/_view/www/src/samples/SampleView.mjs`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/src/inspect_ai/_view/www/src/samples/SamplesCard.mjs` & `inspect_ai-0.3.6/src/inspect_ai/_view/www/src/samples/SamplesCard.mjs`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/src/inspect_ai/_view/www/src/title/TitleBlock.mjs` & `inspect_ai-0.3.6/src/inspect_ai/_view/www/src/title/TitleBlock.mjs`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/src/inspect_ai/_view/www/src/usage/ModelTokenTable.mjs` & `inspect_ai-0.3.6/src/inspect_ai/_view/www/src/usage/ModelTokenTable.mjs`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/src/inspect_ai/_view/www/src/usage/UsageCard.mjs` & `inspect_ai-0.3.6/src/inspect_ai/_view/www/src/usage/UsageCard.mjs`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/src/inspect_ai/_view/www/src/utils/Format.mjs` & `inspect_ai-0.3.6/src/inspect_ai/_view/www/src/utils/Format.mjs`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/src/inspect_ai/_view/www/src/workspace/EpochFilter.mjs` & `inspect_ai-0.3.6/src/inspect_ai/_view/www/src/workspace/EpochFilter.mjs`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/src/inspect_ai/_view/www/src/workspace/SampleFilter.mjs` & `inspect_ai-0.3.6/src/inspect_ai/_view/www/src/workspace/SampleFilter.mjs`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/src/inspect_ai/_view/www/src/workspace/SamplesDescriptor.mjs` & `inspect_ai-0.3.6/src/inspect_ai/_view/www/src/workspace/SamplesDescriptor.mjs`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/src/inspect_ai/_view/www/src/workspace/SortFilter.mjs` & `inspect_ai-0.3.6/src/inspect_ai/_view/www/src/workspace/SortFilter.mjs`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/src/inspect_ai/_view/www/src/workspace/TaskErrorPanel.mjs` & `inspect_ai-0.3.6/src/inspect_ai/_view/www/src/workspace/TaskErrorPanel.mjs`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/src/inspect_ai/_view/www/src/workspace/WorkSpace.mjs` & `inspect_ai-0.3.6/src/inspect_ai/_view/www/src/workspace/WorkSpace.mjs`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/src/inspect_ai/_view/www/tools.js` & `inspect_ai-0.3.6/src/inspect_ai/_view/www/tools.js`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/src/inspect_ai/dataset/__init__.py` & `inspect_ai-0.3.6/src/inspect_ai/dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/src/inspect_ai/dataset/_dataset.py` & `inspect_ai-0.3.6/src/inspect_ai/dataset/_dataset.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/src/inspect_ai/dataset/_examples/bias_detection.jsonl` & `inspect_ai-0.3.6/src/inspect_ai/dataset/_examples/bias_detection.jsonl`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/src/inspect_ai/dataset/_examples/biology_qa.jsonl` & `inspect_ai-0.3.6/src/inspect_ai/dataset/_examples/biology_qa.jsonl`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/src/inspect_ai/dataset/_examples/popularity.jsonl` & `inspect_ai-0.3.6/src/inspect_ai/dataset/_examples/popularity.jsonl`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/src/inspect_ai/dataset/_examples/security_guide.jsonl` & `inspect_ai-0.3.6/src/inspect_ai/dataset/_examples/security_guide.jsonl`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/src/inspect_ai/dataset/_examples/theory_of_mind.jsonl` & `inspect_ai-0.3.6/src/inspect_ai/dataset/_examples/theory_of_mind.jsonl`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/src/inspect_ai/dataset/_sources/csv.py` & `inspect_ai-0.3.6/src/inspect_ai/dataset/_sources/csv.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/src/inspect_ai/dataset/_sources/example.py` & `inspect_ai-0.3.6/src/inspect_ai/dataset/_sources/example.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/src/inspect_ai/dataset/_sources/file.py` & `inspect_ai-0.3.6/src/inspect_ai/dataset/_sources/file.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/src/inspect_ai/dataset/_sources/hf.py` & `inspect_ai-0.3.6/src/inspect_ai/dataset/_sources/hf.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/src/inspect_ai/dataset/_sources/json.py` & `inspect_ai-0.3.6/src/inspect_ai/dataset/_sources/json.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/src/inspect_ai/dataset/_util.py` & `inspect_ai-0.3.6/src/inspect_ai/dataset/_util.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/src/inspect_ai/log/__init__.py` & `inspect_ai-0.3.6/src/inspect_ai/log/__init__.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/src/inspect_ai/log/_file.py` & `inspect_ai-0.3.6/src/inspect_ai/log/_file.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/src/inspect_ai/log/_log.py` & `inspect_ai-0.3.6/src/inspect_ai/log/_log.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/src/inspect_ai/model/__init__.py` & `inspect_ai-0.3.6/src/inspect_ai/model/__init__.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/src/inspect_ai/model/_model.py` & `inspect_ai-0.3.6/src/inspect_ai/model/_model.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/src/inspect_ai/model/_providers/anthropic.py` & `inspect_ai-0.3.6/src/inspect_ai/model/_providers/anthropic.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/src/inspect_ai/model/_providers/azureai.py` & `inspect_ai-0.3.6/src/inspect_ai/model/_providers/azureai.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/src/inspect_ai/model/_providers/bedrock.py` & `inspect_ai-0.3.6/src/inspect_ai/model/_providers/bedrock.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/src/inspect_ai/model/_providers/cloudflare.py` & `inspect_ai-0.3.6/src/inspect_ai/model/_providers/cloudflare.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/src/inspect_ai/model/_providers/google.py` & `inspect_ai-0.3.6/src/inspect_ai/model/_providers/google.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/src/inspect_ai/model/_providers/hf.py` & `inspect_ai-0.3.6/src/inspect_ai/model/_providers/hf.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/src/inspect_ai/model/_providers/mistral.py` & `inspect_ai-0.3.6/src/inspect_ai/model/_providers/mistral.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/src/inspect_ai/model/_providers/openai.py` & `inspect_ai-0.3.6/src/inspect_ai/model/_providers/openai.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/src/inspect_ai/model/_providers/providers.py` & `inspect_ai-0.3.6/src/inspect_ai/model/_providers/providers.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/src/inspect_ai/model/_providers/together.py` & `inspect_ai-0.3.6/src/inspect_ai/model/_providers/together.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/src/inspect_ai/model/_providers/util.py` & `inspect_ai-0.3.6/src/inspect_ai/model/_providers/util.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/src/inspect_ai/model/_registry.py` & `inspect_ai-0.3.6/src/inspect_ai/model/_registry.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/src/inspect_ai/model/_tool.py` & `inspect_ai-0.3.6/src/inspect_ai/model/_tool.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/src/inspect_ai/model/_util.py` & `inspect_ai-0.3.6/src/inspect_ai/model/_util.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/src/inspect_ai/scorer/__init__.py` & `inspect_ai-0.3.6/src/inspect_ai/scorer/__init__.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/src/inspect_ai/scorer/_answer.py` & `inspect_ai-0.3.6/src/inspect_ai/scorer/_answer.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/src/inspect_ai/scorer/_common.py` & `inspect_ai-0.3.6/src/inspect_ai/scorer/_common.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/src/inspect_ai/scorer/_match.py` & `inspect_ai-0.3.6/src/inspect_ai/scorer/_match.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/src/inspect_ai/scorer/_metric.py` & `inspect_ai-0.3.6/src/inspect_ai/scorer/_metric.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/src/inspect_ai/scorer/_metrics/accuracy.py` & `inspect_ai-0.3.6/src/inspect_ai/scorer/_metrics/accuracy.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/src/inspect_ai/scorer/_metrics/mean.py` & `inspect_ai-0.3.6/src/inspect_ai/scorer/_metrics/mean.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/src/inspect_ai/scorer/_metrics/std.py` & `inspect_ai-0.3.6/src/inspect_ai/scorer/_metrics/std.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/src/inspect_ai/scorer/_model.py` & `inspect_ai-0.3.6/src/inspect_ai/scorer/_model.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/src/inspect_ai/scorer/_pattern.py` & `inspect_ai-0.3.6/src/inspect_ai/scorer/_pattern.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/src/inspect_ai/scorer/_scorer.py` & `inspect_ai-0.3.6/src/inspect_ai/scorer/_scorer.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/src/inspect_ai/solver/__init__.py` & `inspect_ai-0.3.6/src/inspect_ai/solver/__init__.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/src/inspect_ai/solver/_critique.py` & `inspect_ai-0.3.6/src/inspect_ai/solver/_critique.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/src/inspect_ai/solver/_multiple_choice.py` & `inspect_ai-0.3.6/src/inspect_ai/solver/_multiple_choice.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/src/inspect_ai/solver/_plan.py` & `inspect_ai-0.3.6/src/inspect_ai/solver/_plan.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/src/inspect_ai/solver/_prompt.py` & `inspect_ai-0.3.6/src/inspect_ai/solver/_prompt.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/src/inspect_ai/solver/_solver.py` & `inspect_ai-0.3.6/src/inspect_ai/solver/_solver.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/src/inspect_ai/solver/_tool/tool.py` & `inspect_ai-0.3.6/src/inspect_ai/solver/_tool/tool.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/src/inspect_ai/solver/_tool/tool_def.py` & `inspect_ai-0.3.6/src/inspect_ai/solver/_tool/tool_def.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/src/inspect_ai/solver/_tool/use_tools.py` & `inspect_ai-0.3.6/src/inspect_ai/solver/_tool/use_tools.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/src/inspect_ai/solver/_tool/web_search.py` & `inspect_ai-0.3.6/src/inspect_ai/solver/_tool/web_search.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/src/inspect_ai/util/_context/concurrency.py` & `inspect_ai-0.3.6/src/inspect_ai/util/_context/concurrency.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/src/inspect_ai/util/_context/logger.py` & `inspect_ai-0.3.6/src/inspect_ai/util/_context/logger.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/src/inspect_ai/util/_context/resource.py` & `inspect_ai-0.3.6/src/inspect_ai/util/_context/resource.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/src/inspect_ai/util/_context/subprocess.py` & `inspect_ai-0.3.6/src/inspect_ai/util/_context/subprocess.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/src/inspect_ai.egg-info/PKG-INFO` & `inspect_ai-0.3.6/src/inspect_ai.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inspect_ai
-Version: 0.3.5
+Version: 0.3.6
 Summary: Framework for large language model evaluations
 Author: UK AI Safety Institute
 License: MIT License
 Project-URL: Documentation, https://UKGovernmentBEIS.github.io/inspect_ai/
 Project-URL: Source Code, https://github.com/UKGovernmentBEIS/inspect_ai
 Project-URL: Issue Tracker, https://github.com/UKGovernmentBEIS/inspect_ai/issues
 Classifier: Development Status :: 4 - Beta
```

### Comparing `inspect_ai-0.3.5/src/inspect_ai.egg-info/SOURCES.txt` & `inspect_ai-0.3.6/src/inspect_ai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/src/inspect_ai.egg-info/requires.txt` & `inspect_ai-0.3.6/src/inspect_ai.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/tests/test_anthropic.py` & `inspect_ai-0.3.6/tests/test_anthropic.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/tests/test_collapse_user_message.py` & `inspect_ai-0.3.6/tests/test_collapse_user_message.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/tests/test_dataset.py` & `inspect_ai-0.3.6/tests/test_dataset.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/tests/test_eval_log.py` & `inspect_ai-0.3.6/tests/test_eval_log.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/tests/test_hf.py` & `inspect_ai-0.3.6/tests/test_hf.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/tests/test_images/images.jsonl` & `inspect_ai-0.3.6/tests/test_images/images.jsonl`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/tests/test_images.py` & `inspect_ai-0.3.6/tests/test_images.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/tests/test_list_task.py` & `inspect_ai-0.3.6/tests/test_list_task.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/tests/test_logprobs.py` & `inspect_ai-0.3.6/tests/test_logprobs.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/tests/test_metric.py` & `inspect_ai-0.3.6/tests/test_metric.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/tests/test_num_choices.py` & `inspect_ai-0.3.6/tests/test_num_choices.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/tests/test_openai.py` & `inspect_ai-0.3.6/tests/test_openai.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/tests/test_plan.py` & `inspect_ai-0.3.6/tests/test_plan.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/tests/test_registry.py` & `inspect_ai-0.3.6/tests/test_registry.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/tests/test_retry.py` & `inspect_ai-0.3.6/tests/test_retry.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/tests/test_scorer.py` & `inspect_ai-0.3.6/tests/test_scorer.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/tests/test_solver.py` & `inspect_ai-0.3.6/tests/test_solver.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/tests/test_stop_reason.py` & `inspect_ai-0.3.6/tests/test_stop_reason.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/tests/test_subprocess.py` & `inspect_ai-0.3.6/tests/test_subprocess.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/tests/test_tools.py` & `inspect_ai-0.3.6/tests/test_tools.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.5/tests/utils.py` & `inspect_ai-0.3.6/tests/utils.py`

 * *Files identical despite different names*

