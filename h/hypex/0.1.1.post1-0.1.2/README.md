# Comparing `tmp/hypex-0.1.1.post1.tar.gz` & `tmp/hypex-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hypex-0.1.1.post1.tar", max compression
+gzip compressed data, was "hypex-0.1.2.tar", max compression
```

## Comparing `hypex-0.1.1.post1.tar` & `hypex-0.1.2.tar`

### file list

```diff
@@ -1,26 +1,27 @@
--rw-r--r--   0        0        0    11335 2023-11-03 10:51:38.050851 hypex-0.1.1.post1/LICENSE
--rw-r--r--   0        0        0     7102 2024-03-05 12:40:13.754857 hypex-0.1.1.post1/README.md
--rw-r--r--   0        0        0      229 2024-03-25 15:07:07.945980 hypex-0.1.1.post1/hypex/__init__.py
--rw-r--r--   0        0        0       24 2024-03-25 15:06:44.432678 hypex-0.1.1.post1/hypex/__version__.py
--rw-r--r--   0        0        0        0 2024-03-01 11:30:31.674823 hypex-0.1.1.post1/hypex/ab_test/__init__.py
--rw-r--r--   0        0        0    44330 2024-03-06 12:06:50.408028 hypex-0.1.1.post1/hypex/ab_test/aa_tester.py
--rw-r--r--   0        0        0    12240 2024-03-06 12:06:50.409651 hypex-0.1.1.post1/hypex/ab_test/ab_tester.py
--rw-r--r--   0        0        0      319 2024-03-25 14:59:21.135315 hypex-0.1.1.post1/hypex/abn_test/__init__.py
--rw-r--r--   0        0        0    12230 2024-03-25 14:59:21.135778 hypex-0.1.1.post1/hypex/abn_test/limit_distribution.py
--rw-r--r--   0        0        0      181 2024-01-16 10:16:36.081229 hypex-0.1.1.post1/hypex/algorithms/__init__.py
--rw-r--r--   0        0        0    39079 2024-03-20 08:54:09.976546 hypex-0.1.1.post1/hypex/algorithms/faiss_matcher.py
--rw-r--r--   0        0        0     7034 2024-02-09 08:31:59.268823 hypex-0.1.1.post1/hypex/algorithms/no_replacement_matching.py
--rw-r--r--   0        0        0    37924 2024-03-25 14:59:21.138090 hypex-0.1.1.post1/hypex/matcher.py
--rw-r--r--   0        0        0        0 2024-01-16 10:16:36.082214 hypex-0.1.1.post1/hypex/selectors/__init__.py
--rw-r--r--   0        0        0     1603 2024-01-16 10:16:36.082539 hypex-0.1.1.post1/hypex/selectors/base_filtration.py
--rw-r--r--   0        0        0     2211 2024-03-05 12:40:13.756798 hypex-0.1.1.post1/hypex/selectors/feature_selector.py
--rw-r--r--   0        0        0     3302 2024-02-09 08:31:59.270027 hypex-0.1.1.post1/hypex/selectors/outliers_filter.py
--rw-r--r--   0        0        0    13494 2024-03-01 13:41:56.566402 hypex-0.1.1.post1/hypex/selectors/selector_primal_methods.py
--rw-r--r--   0        0        0     2461 2024-01-16 10:16:36.083220 hypex-0.1.1.post1/hypex/selectors/spearman_filter.py
--rw-r--r--   0        0        0        0 2024-01-15 07:39:39.825522 hypex-0.1.1.post1/hypex/utils/__init__.py
--rw-r--r--   0        0        0     5752 2024-01-16 10:16:36.083517 hypex-0.1.1.post1/hypex/utils/metrics.py
--rw-r--r--   0        0        0    18936 2024-01-16 10:16:36.083715 hypex-0.1.1.post1/hypex/utils/psi_pandas.py
--rw-r--r--   0        0        0     5371 2024-03-05 12:39:18.744254 hypex-0.1.1.post1/hypex/utils/tutorial_data_creation.py
--rw-r--r--   0        0        0     3620 2024-03-05 12:40:13.761639 hypex-0.1.1.post1/hypex/utils/validators.py
--rw-r--r--   0        0        0     2085 2024-03-25 12:59:37.062545 hypex-0.1.1.post1/pyproject.toml
--rw-r--r--   0        0        0     9083 1970-01-01 00:00:00.000000 hypex-0.1.1.post1/PKG-INFO
+-rw-r--r--   0        0        0    11335 2023-11-03 10:51:38.050851 hypex-0.1.2/LICENSE
+-rw-r--r--   0        0        0     8371 2024-05-06 08:39:00.854680 hypex-0.1.2/README.md
+-rw-r--r--   0        0        0      229 2024-05-06 08:38:40.572486 hypex-0.1.2/hypex/__init__.py
+-rw-r--r--   0        0        0       24 2024-05-06 08:38:40.574385 hypex-0.1.2/hypex/__version__.py
+-rw-r--r--   0        0        0        0 2024-05-06 08:38:40.574419 hypex-0.1.2/hypex/ab_test/__init__.py
+-rw-r--r--   0        0        0    49543 2024-05-06 08:41:16.753090 hypex-0.1.2/hypex/ab_test/aa_tester.py
+-rw-r--r--   0        0        0    12240 2024-05-06 08:38:40.579040 hypex-0.1.2/hypex/ab_test/ab_tester.py
+-rw-r--r--   0        0        0      319 2024-05-06 08:38:40.579548 hypex-0.1.2/hypex/abn_test/__init__.py
+-rw-r--r--   0        0        0    12230 2024-05-06 08:38:40.579938 hypex-0.1.2/hypex/abn_test/limit_distribution.py
+-rw-r--r--   0        0        0      181 2024-05-06 08:38:40.581916 hypex-0.1.2/hypex/algorithms/__init__.py
+-rw-r--r--   0        0        0    39079 2024-05-06 08:38:40.582302 hypex-0.1.2/hypex/algorithms/faiss_matcher.py
+-rw-r--r--   0        0        0     7034 2024-05-06 08:38:40.583068 hypex-0.1.2/hypex/algorithms/no_replacement_matching.py
+-rw-r--r--   0        0        0    37924 2024-05-06 08:38:40.583366 hypex-0.1.2/hypex/matcher.py
+-rw-r--r--   0        0        0        0 2024-05-06 08:38:40.583514 hypex-0.1.2/hypex/selectors/__init__.py
+-rw-r--r--   0        0        0     1603 2024-05-06 08:38:40.583749 hypex-0.1.2/hypex/selectors/base_filtration.py
+-rw-r--r--   0        0        0     2211 2024-05-06 08:38:40.583960 hypex-0.1.2/hypex/selectors/feature_selector.py
+-rw-r--r--   0        0        0     3302 2024-05-06 08:38:40.584290 hypex-0.1.2/hypex/selectors/outliers_filter.py
+-rw-r--r--   0        0        0    13494 2024-05-06 08:38:40.584968 hypex-0.1.2/hypex/selectors/selector_primal_methods.py
+-rw-r--r--   0        0        0     2461 2024-05-06 08:38:40.585235 hypex-0.1.2/hypex/selectors/spearman_filter.py
+-rw-r--r--   0        0        0        0 2024-05-06 08:38:40.585330 hypex-0.1.2/hypex/utils/__init__.py
+-rw-r--r--   0        0        0     5854 2024-05-06 08:39:00.865875 hypex-0.1.2/hypex/utils/datasets.py
+-rw-r--r--   0        0        0     5752 2024-05-06 08:38:40.585522 hypex-0.1.2/hypex/utils/metrics.py
+-rw-r--r--   0        0        0    18936 2024-05-06 08:38:40.585724 hypex-0.1.2/hypex/utils/psi_pandas.py
+-rw-r--r--   0        0        0     5456 2024-05-06 08:39:00.866086 hypex-0.1.2/hypex/utils/tutorial_data_creation.py
+-rw-r--r--   0        0        0     3620 2024-05-06 08:38:40.586235 hypex-0.1.2/hypex/utils/validators.py
+-rw-r--r--   0        0        0     2083 2024-05-06 08:41:45.524600 hypex-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0    10346 1970-01-01 00:00:00.000000 hypex-0.1.2/PKG-INFO
```

### Comparing `hypex-0.1.1.post1/LICENSE` & `hypex-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hypex-0.1.1.post1/README.md` & `hypex-0.1.2/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 # HypEx: Advanced Causal Inference and AB Testing Toolkit
 
+![Last release](https://img.shields.io/badge/pypi-v0.1.1-darkgreen)
 [![Telegram](https://img.shields.io/badge/chat-on%20Telegram-2ba2d9.svg)](https://t.me/hypexchat)
+![Pypi downloads](https://img.shields.io/badge/downloads-5K-1E782B)
+![Python versions](https://img.shields.io/badge/python-3.8_|_3.9_|_3.10_|_3.11_|_3.12-blue)
+![Pypi downloads\month](https://img.shields.io/badge/downloads\month->1K-1E782B)
 
 ## Introduction
 
 HypEx (Hypotheses and Experiments) is a comprehensive library crafted to streamline the causal inference and AB testing
 processes in data analytics. Developed for efficiency and effectiveness, HypEx employs Rubin's Causal Model (RCM) for
 matching closely related pairs, ensuring equitable group comparisons when estimating treatment effects.
 
@@ -19,15 +23,15 @@
 
 - **Faiss KNN Matching**: Utilizes Faiss for efficient and precise nearest neighbor searches, aligning with RCM for
   optimal pair matching.
 - **Data Filters**: Built-in outlier and Spearman filters ensure data quality for matching.
 - **Result Validation**: Offers multiple validation methods, including random treatment, feature, and subset
   validations.
 - **Data Tests**: Incorporates SMD, KS, PSI, and Repeats tests to affirm the robustness of effect estimations.
-- **Automated Feature Selection**: Employs LGBM feature selection to pinpoint the most impactful features for causal
+- **Feature Selection**: Employs LGBM and Catboost feature selection to pinpoint the most impactful features for causal
   analysis.
 - **AB Testing Suite**: Features a suite of AB testing tools for comprehensive hypothesis evaluation.
 - **Stratification support**: Stratify groups for nuanced analysis
 - **Weights support**:  Empower your analysis by assigning custom weights to features, enhancing the matching precision
   to suit your specific research needs
 
 ## Warnings
@@ -50,51 +54,33 @@
 * All features significantly affecting the target should be included.
 * The business rationale of features.
 * The feature selection function can be useful for addressing these tasks, but it does not solve them nor does it
   absolve the user of the responsibility for their selection, nor does it justify it.
 
 [Link to ReadTheDocs](https://hypex.readthedocs.io/en/latest/pages/modules/selectors.html#selector-classes)
 
-### Multitarget
-
-**Multitarget** involves studying the impact on multiple targets.
-
-The algorithm is implemented as a repetition of the same matching on the same feature space and samples, but with
-different targets. To ensure the algorithm's correct operation, it's necessary to guarantee the independence of the
-targets from each other.
-
-The best solution would be to conduct several independent experiments, each with its own set of features for each
-target.
-
-[Link to ReadTheDocs](https://hypex.readthedocs.io/en/latest/pages/modules/matcher.html#matcher)
-
-### Random Treatment и Random Feature
+### Random Treatment
 
 **Random Treatment** algorithm randomly shuffles the actual treatment. It is expected that the treatment's effect on the
 target will be close to 0.
 
-**Random Feature** adds a feature with random values. It is expected that adding a random feature will maintain the same
-impact of the treatment on the target.
-
-These methods are not sufficiently accurate markers of a successful experiment.
+These method is not sufficiently accurate marker of a successful experiment.
 
 [Link to ReadTheDocs](https://hypex.readthedocs.io/en/latest/pages/modules/utils.html#validators)
 
-## Quick Start
-
-Explore usage examples and tutorials [here](https://github.com/sb-ai-lab/Hypex/blob/master/examples/tutorials/).
-
 ## Installation
 
 ```bash
-pip install hypex
+pip install -U hypex
 ```
 
 ## Quick start
 
+Explore usage examples and tutorials [here](https://github.com/sb-ai-lab/Hypex/blob/master/examples/tutorials/).
+
 ### Matching example
 
 ```python
 from hypex import Matcher
 from hypex.utils.tutorial_data_creation import create_test_data
 
 # Define your data and parameters
@@ -146,27 +132,51 @@
 
 For more detailed information about the library and its features, visit
 our [documentation on ReadTheDocs](https://hypex.readthedocs.io/en/latest/).
 
 You'll find comprehensive guides and tutorials that will help you get started with HypEx, as well as detailed API
 documentation for advanced use cases.
 
-## Community and Contributions
+## Contributions
 
 Join our vibrant community! For guidelines on contributing, reporting issues, or seeking support, please refer to
 our [Contributing Guidelines](https://github.com/sb-ai-lab/Hypex/blob/master/.github/CONTRIBUTING.md).
 
-## Success Stories
+## More Information & Resources
 
-Discover how HypEx is revolutionizing causal inference in various fields. Check out our featured article
-on [Habr (ru)](https://habr.com/ru/companies/sberbank/articles/778774/).
+[Habr (ru)](https://habr.com/ru/companies/sberbank/articles/778774/) - discover how HypEx is revolutionizing causal
+inference in various fields.      
+[A/B testing seminar](https://www.youtube.com/watch?v=B9BE_yk8CjA&t=53s&ab_channel=NoML) - Seminar in NoML about
+matching and A/B testing       
+[Matching with HypEx: Simple Guide](https://www.kaggle.com/code/kseniavasilieva/matching-with-hypex-simple-guide) -
+Simple matching guide with explanation           
+[Matching with HypEx: Grouping](https://www.kaggle.com/code/kseniavasilieva/matching-with-hypex-grouping) - Matching
+with grouping guide    
+[HypEx vs Causal Inference and DoWhy](https://www.kaggle.com/code/kseniavasilieva/hypex-vs-causal-inference-and-dowhy) -
+discover why HypEx is the best solution for causal inference           
+[HypEx vs Causal Inference and DoWhy: part 2](https://www.kaggle.com/code/kseniavasilieva/hypex-vs-causal-inference-part-2) -
+discover why HypEx is the best solution for causal inference
+
+### Testing different libraries for the speed of matching
+
+Visit [this](https://www.kaggle.com/code/kseniavasilieva/hypex-vs-causal-inference-part-2) notebook ain Kaggle and
+estimate results by yourself.
+
+| Group size             | 32 768   | 65 536     | 131 072   | 262 144   | 524 288    | 1 048 576   | 2 097 152    | 4 194 304     |
+|------------------------|---------|-----------|----------|----------|-----------|-----------|------------|-------------|
+| Causal Inference       | 46s | 169s | None     | None     | None      | None      | None       | None        |
+| DoWhy                  | 9s | 19s  | 40s | 77s | 159s | 312s | 615s  | 1 235s  |
+| HypEx with grouping    | 2s | 6s   | 16s | 42s | 167s | 509s | 1 932s | 7 248s  |
+| HypEx without grouping | 2s  | 7s   | 21s | 101s | 273s | 982s | 3 750s | 14 720s |
 
 ## Join Our Community
 
 Have questions or want to discuss HypEx? Join our [Telegram chat](https://t.me/HypExChat) and connect with the community
 and the developers.
 
 ## Conclusion
 
 HypEx stands as an indispensable resource for data analysts and researchers delving into causal inference and AB
 testing. With its automated capabilities, sophisticated matching techniques, and thorough validation procedures, HypEx
 is poised to unravel causal relationships in complex datasets with unprecedented speed and precision.
+
+##
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `hypex-0.1.1.post1/hypex/ab_test/aa_tester.py` & `hypex-0.1.2/hypex/ab_test/aa_tester.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 """Module for AA tests"""
 
+import math
 import warnings
+from decimal import Decimal
 from itertools import combinations
 from pathlib import Path
 from typing import Iterable, Union, Optional, Dict, Any, Tuple, List
 
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 import seaborn as sns
-from scipy.stats import ttest_ind, ks_2samp, norm
+from scipy.stats import ttest_ind, ks_2samp, norm, chi2_contingency
 from sklearn.utils import shuffle
 from statsmodels.stats.power import TTestIndPower
 
 try:
     from tqdm.auto import tqdm
 except:
     try:
@@ -63,14 +65,16 @@
             Computes the average score for passed tests in AA testing.
         uniform_tests_interpretation(experiment_results):
             Analyzes and plots the results of uniform tests.
         num_feature_uniform_analysis(control_data, test_data, plot_set):
             Analyzes and plots numerical feature distributions in control and test data.
         cat_feature_uniform_analysis(control_data, test_data):
             Analyzes and plots categorical feature distributions in control and test data.
+        calc_mde_unbalanced_group(data, target_field, group_flag_col, power):
+            Finds minimum detectable effect (MDE) and effect size for unbalanced groups.
         experiment_result_transform(experiment):
             Transforms the result of an experiment into a readable format.
         split_analysis(splited_data):
             Analyzes split data for both target and group columns.
         get_resume(aa_score, best_experiment_stat):
             Formats the final results of AA testing for clarity.
         process(data, optimize_groups, iterations, show_plots, test_size, pbar):
@@ -783,86 +787,164 @@
                     "test_group and control_group cannot be None if data and target_field are None"
                 )
             splited_data = self.split_splited_data(data)
             test_group = splited_data["test"][target_field]
             control_group = splited_data["control"][target_field]
         return {"test_group": test_group, "control_group": control_group}
 
+    def __mde_unbalanced_non_binomial(
+        self,
+        control_group_size: int,
+        all_data_size: int,
+        standard_deviation: float = 2.0,
+        power: float = 0.8,
+    ) -> Tuple:
+        """Calculates minimum detectable effect (MDE) and significance
+        of the effect size for unbalanced non-binomial groups.
+
+                       Args:
+                           control_group_size:
+                               Size of the control group
+                           all_data_size:
+                               Size of the all data sample
+                           standard_deviation:
+                               Standard_deviation
+                           power:
+                               Level of power
+
+
+                       Returns:
+                           Tuple with MDE and significance of the effect size
+        """
+        proportion = round((all_data_size - control_group_size) / control_group_size, 2)
+        z_alpha = norm.ppf(1 - self.alpha / 2)
+        z_power = norm.ppf(power)
+        mde = (standard_deviation * (z_alpha - z_power)) * math.sqrt(
+            (1 + proportion) / (control_group_size * proportion)
+        )
+        effect_size = mde / standard_deviation  # effect_size
+
+        return (
+            float(Decimal(float(mde)).quantize(Decimal("1.00"))),
+            float(Decimal(float(effect_size)).quantize(Decimal("1.00"))),
+        )
+
+    def __mde_unbalanced_binomial(
+        self,
+        control_group_size: int,
+        all_data_size: int,
+        fact_conversion: float,
+        power: float = 0.8,
+    ) -> Tuple:
+        """Calculates minimum detectable effect (MDE) and significance
+        of the effect size (Cohen's d) for unbalanced binomial groups.
+
+               Args:
+                   control_group_size:
+                       Size of the control group
+                   all_data_size:
+                       Size of the all data sample
+                   fact_conversion:
+                       Conversion in the control group
+                   power:
+                       Level of power
+
+
+               Returns:
+                   Tuple with MDE and Cohen's d
+        """
+        proportion = round((all_data_size - control_group_size) / control_group_size, 2)
+        z_alpha = norm.ppf(1 - self.alpha / 2)
+        z_power = norm.ppf(power)
+        cohen_d = (z_alpha - z_power) * math.sqrt(
+            (1 + proportion) / (control_group_size * proportion)
+        )  # effect_size
+        expect_conversion = (
+            math.sin(math.asin(math.sqrt(fact_conversion)) + cohen_d / 2) ** 2
+        )  # expect_conversion
+        mde = abs(expect_conversion - fact_conversion)
+
+        return (
+            float(Decimal(float(mde)).quantize(Decimal("1.00"))),
+            float(Decimal(float(cohen_d)).quantize(Decimal("1.00"))),
+        )
+
     def calc_mde(
         self,
-        test_group: pd.Series = None,
-        control_group: pd.Series = None,
-        data: pd.DataFrame = None,
-        target_field: str = None,
-        reliability: float = 0.95,
+        data: pd.DataFrame,
+        target_field: str,
+        group_field: str,
         power: float = 0.8,
-    ) -> float:
-        """Calculates the minimum detectable effect (MDE) for a given test and control groups.
+    ) -> Tuple:
+        """Finds minimum detectable effect (MDE) and effect size for unbalanced groups.
 
         Args:
-            test_group:
-                The test group as a pandas Series
-            control_group:
-                The control group as a pandas Series
             data:
-                The input data as a pandas DataFrame used if test_group and control_group are None
+                Input data
             target_field:
-                The target field used if given data is a DataFrame
-            reliability:
-                The reliability of the test
+                Name of the target feature
+            group_field:
+                Name of the column with the group flag
             power:
-                The power of the test
+                Level of power
+
 
         Returns:
-            The minimum detectable effect
+            Tuple with MDE and effect size
         """
+        fact_conversion = float(
+            Decimal(float(data[target_field].mean())).quantize(Decimal("1.00"))
+        )  # fact_conversion
+        control_group = data[
+            (data[group_field] == data[group_field].unique()[0])
+        ]  # control_group
+        control_group_size = len(control_group)  # control_group_size
+        all_data_size = len(data[group_field])  # all_data_size (???)
+
+        if data[target_field].nunique() == 2:
+            res = self.__mde_unbalanced_binomial(
+                control_group_size=control_group_size,
+                all_data_size=all_data_size,
+                fact_conversion=fact_conversion,
+                power=power,
+            )
+        else:
+            res = self.__mde_unbalanced_non_binomial(
+                control_group_size=control_group_size,
+                all_data_size=all_data_size,
+                standard_deviation=data[target_field].std(),
+                power=power,
+            )
 
-        m = norm.ppf(1 - (1 - reliability) / 2) + norm.ppf(power)
-
-        groups = self.__get_test_and_control_series(
-            test_group=test_group,
-            control_group=control_group,
-            data=data,
-            target_field=target_field,
-        )
-        test_group = groups["test_group"]
-        control_group = groups["control_group"]
-
-        n_test, n_control = len(test_group), len(control_group)
-        proportion = n_test / (n_test + n_control)
-        p = np.sqrt(1 / (proportion * (1 - proportion)))
-
-        var_test, var_control = np.var(test_group, ddof=1), np.var(
-            control_group, ddof=1
-        )
-        s = np.sqrt(var_test / n_test + var_control / n_control)
-
-        return p * m * s
+        return res
 
     def calc_sample_size(
         self,
         test_group: pd.Series = None,
         control_group: pd.Series = None,
         data: pd.DataFrame = None,
         target_field: str = None,
-        mde=None,
+        group_field: str = "group",
+        mde: float = None,
         significance: float = 0.05,
         power: float = 0.8,
     ) -> float:
         """Calculates sample size of dataframe depends on mde and power.
 
         Args:
             test_group:
                 The test group as a pandas Series
             control_group:
                 The control group as a pandas Series
             data:
                 The input data as a pandas DataFrame used if test_group and control_group are None
             target_field:
                 The target field used if given data is a DataFrame
+            group_field:
+                The group field used if given data is a DataFrame
             mde:
                 Minimum detectable effect. If None, it will be calculated. If it is a tuple, it will be used as relative mde
             significance:
                 Level of significance (alpha)
             power:
                 Power of criterion
 
@@ -886,19 +968,18 @@
                 test_group=test_group,
                 control_group=control_group,
                 data=data,
                 target_field=target_field,
             )
             control_group = groups["control_group"]
             test_group = groups["test_group"]
-
             mde = mde or self.calc_mde(
-                test_group=test_group,
-                control_group=control_group,
-                reliability=1 - significance,
+                data=data,
+                target_field=target_field,
+                group_field=group_field,
                 power=power,
             )
 
             control_std = control_group.std()
             test_std = test_group.std()
 
             test_proportion = len(test_group) / (len(test_group) + len(control_group))
@@ -985,14 +1066,67 @@
         return analysis.power(
             effect_size=effect_size,
             nobs1=test_size,
             ratio=ratio,
             alpha=significance,
         )
 
+    def calc_chi2(self, df: pd.DataFrame, treated_column: str):
+        """Chi2 criterio calculation.
+
+        Args:
+            df:
+                Input data
+            treated_column:
+                Column name with group markers (treated/untreated)
+
+        Returns:
+            Dictionary with pvalues for all target fields.
+        """
+        df = df.sort_values(by=treated_column)
+        groups = df[treated_column].unique().tolist()
+        all_pvalues = {}
+        for target_field in self.target_fields:
+            group_a, group_b = (
+                df[df[treated_column] == groups[0]][target_field],
+                df[df[treated_column] == groups[1]][target_field],
+            )
+            proportions = group_a.shape[0] / (group_a.shape[0] + group_b.shape[0])
+            group_a = group_a.value_counts().rename(target_field).sort_index()
+            group_b = group_b.value_counts().rename(target_field).sort_index()
+            index = (
+                pd.Series(group_a.index.tolist() + group_b.index.tolist())
+                .unique()
+                .tolist()
+            )
+            group_a, group_b = [
+                group.reindex(index, fill_value=0) for group in [group_a, group_b]
+            ]
+            merged_data = pd.DataFrame(
+                {
+                    "index_x": group_a * (1 - proportions),
+                    "index_y": group_b * proportions,
+                }
+            ).fillna(0)
+            sub_group = merged_data.sum(axis=1).sort_values()
+            _filter = sub_group <= 15
+            if _filter.sum():
+                other = {
+                    "index_x": merged_data["index_x"][_filter].sum(),
+                    "index_y": merged_data["index_y"][_filter].sum(),
+                }
+                merged_data.drop(sub_group[_filter].index, inplace=True)
+                merged_data = pd.concat(
+                    [merged_data, pd.DataFrame([other], index=["Other"])]
+                )
+            all_pvalues[target_field] = chi2_contingency(
+                merged_data[["index_x", "index_y"]]
+            ).pvalue
+        return all_pvalues
+
     def experiment_result_transform(self, experiment: pd.Series):
         """
         Transform experiments results into readable view.
 
         Args:
             experiment:
                 Results of experiments
```

### Comparing `hypex-0.1.1.post1/hypex/ab_test/ab_tester.py` & `hypex-0.1.2/hypex/ab_test/ab_tester.py`

 * *Files identical despite different names*

### Comparing `hypex-0.1.1.post1/hypex/abn_test/limit_distribution.py` & `hypex-0.1.2/hypex/abn_test/limit_distribution.py`

 * *Files identical despite different names*

### Comparing `hypex-0.1.1.post1/hypex/algorithms/faiss_matcher.py` & `hypex-0.1.2/hypex/algorithms/faiss_matcher.py`

 * *Files identical despite different names*

### Comparing `hypex-0.1.1.post1/hypex/algorithms/no_replacement_matching.py` & `hypex-0.1.2/hypex/algorithms/no_replacement_matching.py`

 * *Files identical despite different names*

### Comparing `hypex-0.1.1.post1/hypex/matcher.py` & `hypex-0.1.2/hypex/matcher.py`

 * *Files identical despite different names*

### Comparing `hypex-0.1.1.post1/hypex/selectors/base_filtration.py` & `hypex-0.1.2/hypex/selectors/base_filtration.py`

 * *Files identical despite different names*

### Comparing `hypex-0.1.1.post1/hypex/selectors/feature_selector.py` & `hypex-0.1.2/hypex/selectors/feature_selector.py`

 * *Files identical despite different names*

### Comparing `hypex-0.1.1.post1/hypex/selectors/outliers_filter.py` & `hypex-0.1.2/hypex/selectors/outliers_filter.py`

 * *Files identical despite different names*

### Comparing `hypex-0.1.1.post1/hypex/selectors/selector_primal_methods.py` & `hypex-0.1.2/hypex/selectors/selector_primal_methods.py`

 * *Files identical despite different names*

### Comparing `hypex-0.1.1.post1/hypex/selectors/spearman_filter.py` & `hypex-0.1.2/hypex/selectors/spearman_filter.py`

 * *Files identical despite different names*

### Comparing `hypex-0.1.1.post1/hypex/utils/metrics.py` & `hypex-0.1.2/hypex/utils/metrics.py`

 * *Files identical despite different names*

### Comparing `hypex-0.1.1.post1/hypex/utils/psi_pandas.py` & `hypex-0.1.2/hypex/utils/psi_pandas.py`

 * *Files identical despite different names*

### Comparing `hypex-0.1.1.post1/hypex/utils/tutorial_data_creation.py` & `hypex-0.1.2/hypex/utils/tutorial_data_creation.py`

 * *Files 5% similar despite different names*

```diff
@@ -68,27 +68,29 @@
 
 
 def create_test_data(
         num_users: int = 10000,
         na_step: Union[Iterable[int], int] = None,
         nan_cols: Union[Iterable[str], str] = None,
         file_name: str = None,
-        rs=None
+        exact_ATT: int = 100,
+        rs=None,
 ):
     """Creates data for tutorial.
 
     Args:
         num_users: num of strings
         na_step: 
             num or list of nums of period to make NaN (step of range)
             If list - iterates accordingly order of columns
         nan_cols: 
             name of one or several columns to fill with NaN
             If list - iterates accordingly order of na_step
         file_name: name of file to save; doesn't save file if None
+        exact_ATT: an accurate synthetic effect
 
     Returns:
         data: dataframe with
     """
     if rs is not None:
         np.random.seed(rs)
 
@@ -113,15 +115,15 @@
     data["treat"] = data["signup_month"] > 0
 
     # Simulating an effect of month (monotonically decreasing--customers buy less later in the year)
     data["spend"] = data["spend"] - data["month"] * 10
 
     # Simulating a simple treatment effect of 100
     after_signup = (data["signup_month"] < data["month"]) & (data["treat"])
-    data.loc[after_signup, "spend"] = data[after_signup]["spend"] + 100
+    data.loc[after_signup, "spend"] = data[after_signup]["spend"] + exact_ATT
 
     # Setting the signup month (for ease of analysis)
     i = 3
     data = (
         data
         .groupby(["user_id", "signup_month", "treat"])
         .apply(
```

### Comparing `hypex-0.1.1.post1/hypex/utils/validators.py` & `hypex-0.1.2/hypex/utils/validators.py`

 * *Files identical despite different names*

### Comparing `hypex-0.1.1.post1/pyproject.toml` & `hypex-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "HypEx"
-version = "0.1.1-1"
+version = "0.1.2"
 description = "Fast and customizable framework for Causal Inference"
 authors = [
     "Dmitry Tikhomirov <dimasta00@gmail.com>",
     "Dmitry Bulychev <dmatryus.sqrt49@yandex.ru>",
     "Ksenia Vasilieva <vasilievaxeniaa@gmail.com>"
 ]
 readme = "README.md"
```

### Comparing `hypex-0.1.1.post1/PKG-INFO` & `hypex-0.1.2/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hypex
-Version: 0.1.1.post1
+Version: 0.1.2
 Summary: Fast and customizable framework for Causal Inference
 Home-page: https://github.com/sb-ai-lab/HypEx
 License: Apache-2.0
 Author: Dmitry Tikhomirov
 Author-email: dimasta00@gmail.com
 Requires-Python: >=3.8,<3.13
 Classifier: Development Status :: 4 - Beta
@@ -40,15 +40,19 @@
 Requires-Dist: statsmodels (<=0.14.1)
 Requires-Dist: tqdm
 Project-URL: Repository, https://github.com/sb-ai-lab/HypEx
 Description-Content-Type: text/markdown
 
 # HypEx: Advanced Causal Inference and AB Testing Toolkit
 
+![Last release](https://img.shields.io/badge/pypi-v0.1.1-darkgreen)
 [![Telegram](https://img.shields.io/badge/chat-on%20Telegram-2ba2d9.svg)](https://t.me/hypexchat)
+![Pypi downloads](https://img.shields.io/badge/downloads-5K-1E782B)
+![Python versions](https://img.shields.io/badge/python-3.8_|_3.9_|_3.10_|_3.11_|_3.12-blue)
+![Pypi downloads\month](https://img.shields.io/badge/downloads\month->1K-1E782B)
 
 ## Introduction
 
 HypEx (Hypotheses and Experiments) is a comprehensive library crafted to streamline the causal inference and AB testing
 processes in data analytics. Developed for efficiency and effectiveness, HypEx employs Rubin's Causal Model (RCM) for
 matching closely related pairs, ensuring equitable group comparisons when estimating treatment effects.
 
@@ -63,15 +67,15 @@
 
 - **Faiss KNN Matching**: Utilizes Faiss for efficient and precise nearest neighbor searches, aligning with RCM for
   optimal pair matching.
 - **Data Filters**: Built-in outlier and Spearman filters ensure data quality for matching.
 - **Result Validation**: Offers multiple validation methods, including random treatment, feature, and subset
   validations.
 - **Data Tests**: Incorporates SMD, KS, PSI, and Repeats tests to affirm the robustness of effect estimations.
-- **Automated Feature Selection**: Employs LGBM feature selection to pinpoint the most impactful features for causal
+- **Feature Selection**: Employs LGBM and Catboost feature selection to pinpoint the most impactful features for causal
   analysis.
 - **AB Testing Suite**: Features a suite of AB testing tools for comprehensive hypothesis evaluation.
 - **Stratification support**: Stratify groups for nuanced analysis
 - **Weights support**:  Empower your analysis by assigning custom weights to features, enhancing the matching precision
   to suit your specific research needs
 
 ## Warnings
@@ -94,51 +98,33 @@
 * All features significantly affecting the target should be included.
 * The business rationale of features.
 * The feature selection function can be useful for addressing these tasks, but it does not solve them nor does it
   absolve the user of the responsibility for their selection, nor does it justify it.
 
 [Link to ReadTheDocs](https://hypex.readthedocs.io/en/latest/pages/modules/selectors.html#selector-classes)
 
-### Multitarget
-
-**Multitarget** involves studying the impact on multiple targets.
-
-The algorithm is implemented as a repetition of the same matching on the same feature space and samples, but with
-different targets. To ensure the algorithm's correct operation, it's necessary to guarantee the independence of the
-targets from each other.
-
-The best solution would be to conduct several independent experiments, each with its own set of features for each
-target.
-
-[Link to ReadTheDocs](https://hypex.readthedocs.io/en/latest/pages/modules/matcher.html#matcher)
-
-### Random Treatment и Random Feature
+### Random Treatment
 
 **Random Treatment** algorithm randomly shuffles the actual treatment. It is expected that the treatment's effect on the
 target will be close to 0.
 
-**Random Feature** adds a feature with random values. It is expected that adding a random feature will maintain the same
-impact of the treatment on the target.
-
-These methods are not sufficiently accurate markers of a successful experiment.
+These method is not sufficiently accurate marker of a successful experiment.
 
 [Link to ReadTheDocs](https://hypex.readthedocs.io/en/latest/pages/modules/utils.html#validators)
 
-## Quick Start
-
-Explore usage examples and tutorials [here](https://github.com/sb-ai-lab/Hypex/blob/master/examples/tutorials/).
-
 ## Installation
 
 ```bash
-pip install hypex
+pip install -U hypex
 ```
 
 ## Quick start
 
+Explore usage examples and tutorials [here](https://github.com/sb-ai-lab/Hypex/blob/master/examples/tutorials/).
+
 ### Matching example
 
 ```python
 from hypex import Matcher
 from hypex.utils.tutorial_data_creation import create_test_data
 
 # Define your data and parameters
@@ -190,28 +176,52 @@
 
 For more detailed information about the library and its features, visit
 our [documentation on ReadTheDocs](https://hypex.readthedocs.io/en/latest/).
 
 You'll find comprehensive guides and tutorials that will help you get started with HypEx, as well as detailed API
 documentation for advanced use cases.
 
-## Community and Contributions
+## Contributions
 
 Join our vibrant community! For guidelines on contributing, reporting issues, or seeking support, please refer to
 our [Contributing Guidelines](https://github.com/sb-ai-lab/Hypex/blob/master/.github/CONTRIBUTING.md).
 
-## Success Stories
+## More Information & Resources
 
-Discover how HypEx is revolutionizing causal inference in various fields. Check out our featured article
-on [Habr (ru)](https://habr.com/ru/companies/sberbank/articles/778774/).
+[Habr (ru)](https://habr.com/ru/companies/sberbank/articles/778774/) - discover how HypEx is revolutionizing causal
+inference in various fields.      
+[A/B testing seminar](https://www.youtube.com/watch?v=B9BE_yk8CjA&t=53s&ab_channel=NoML) - Seminar in NoML about
+matching and A/B testing       
+[Matching with HypEx: Simple Guide](https://www.kaggle.com/code/kseniavasilieva/matching-with-hypex-simple-guide) -
+Simple matching guide with explanation           
+[Matching with HypEx: Grouping](https://www.kaggle.com/code/kseniavasilieva/matching-with-hypex-grouping) - Matching
+with grouping guide    
+[HypEx vs Causal Inference and DoWhy](https://www.kaggle.com/code/kseniavasilieva/hypex-vs-causal-inference-and-dowhy) -
+discover why HypEx is the best solution for causal inference           
+[HypEx vs Causal Inference and DoWhy: part 2](https://www.kaggle.com/code/kseniavasilieva/hypex-vs-causal-inference-part-2) -
+discover why HypEx is the best solution for causal inference
+
+### Testing different libraries for the speed of matching
+
+Visit [this](https://www.kaggle.com/code/kseniavasilieva/hypex-vs-causal-inference-part-2) notebook ain Kaggle and
+estimate results by yourself.
+
+| Group size             | 32 768   | 65 536     | 131 072   | 262 144   | 524 288    | 1 048 576   | 2 097 152    | 4 194 304     |
+|------------------------|---------|-----------|----------|----------|-----------|-----------|------------|-------------|
+| Causal Inference       | 46s | 169s | None     | None     | None      | None      | None       | None        |
+| DoWhy                  | 9s | 19s  | 40s | 77s | 159s | 312s | 615s  | 1 235s  |
+| HypEx with grouping    | 2s | 6s   | 16s | 42s | 167s | 509s | 1 932s | 7 248s  |
+| HypEx without grouping | 2s  | 7s   | 21s | 101s | 273s | 982s | 3 750s | 14 720s |
 
 ## Join Our Community
 
 Have questions or want to discuss HypEx? Join our [Telegram chat](https://t.me/HypExChat) and connect with the community
 and the developers.
 
 ## Conclusion
 
 HypEx stands as an indispensable resource for data analysts and researchers delving into causal inference and AB
 testing. With its automated capabilities, sophisticated matching techniques, and thorough validation procedures, HypEx
 is poised to unravel causal relationships in complex datasets with unprecedented speed and precision.
 
+##                                                                              
+
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

