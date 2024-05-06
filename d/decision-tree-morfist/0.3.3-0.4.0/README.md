# Comparing `tmp/decision-tree-morfist-0.3.3.tar.gz` & `tmp/decision_tree_morfist-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "decision-tree-morfist-0.3.3.tar", last modified: Sun Aug 16 19:36:34 2020, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `decision-tree-morfist-0.3.3.tar` & `decision_tree_morfist-0.4.0.tar`

### file list

```diff
@@ -1,15 +1,26 @@
--rw-r--r--   0        0        0     1072 2019-12-11 10:43:26.427890 decision-tree-morfist-0.3.3/LICENSE
--rw-r--r--   0        0        0     1966 2020-08-10 09:08:54.954793 decision-tree-morfist-0.3.3/README.md
--rw-r--r--   0        0        0      170 2020-08-10 10:04:07.851656 decision-tree-morfist-0.3.3/morfist/__init__.py
--rw-r--r--   0        0        0      104 2020-08-09 10:47:35.368084 decision-tree-morfist-0.3.3/morfist/algo/__init__.py
--rw-r--r--   0        0        0     2377 2020-08-16 15:07:01.945348 decision-tree-morfist-0.3.3/morfist/algo/evaluation.py
--rw-r--r--   0        0        0     1059 2020-07-25 20:53:16.486910 decision-tree-morfist-0.3.3/morfist/algo/histogram.py
--rw-r--r--   0        0        0     4768 2020-08-16 19:25:15.206438 decision-tree-morfist-0.3.3/morfist/core/MixedRandomForest.py
--rw-r--r--   0        0        0     4450 2020-08-16 15:07:01.946042 decision-tree-morfist-0.3.3/morfist/core/MixedRandomTree.py
--rw-r--r--   0        0        0     6173 2020-08-16 15:07:01.946470 decision-tree-morfist-0.3.3/morfist/core/MixedSplitter.py
--rw-r--r--   0        0        0      171 2020-07-24 13:16:46.118497 decision-tree-morfist-0.3.3/morfist/core/__init__.py
--rw-r--r--   0        0        0       29 2020-08-10 10:04:07.826210 decision-tree-morfist-0.3.3/morfist/legacy/__init__.py
--rw-r--r--   0        0        0    11024 2020-08-10 10:04:07.841909 decision-tree-morfist-0.3.3/morfist/legacy/core.py
--rw-r--r--   0        0        0      960 2020-08-16 19:35:22.020972 decision-tree-morfist-0.3.3/pyproject.toml
--rw-r--r--   0        0        0     2870 2020-08-16 19:36:34.488304 decision-tree-morfist-0.3.3/setup.py
--rw-r--r--   0        0        0     2864 2020-08-16 19:36:34.488710 decision-tree-morfist-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 decision_tree_morfist-0.4.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 decision_tree_morfist-0.4.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1450 2020-02-02 00:00:00.000000 decision_tree_morfist-0.4.0/mkdocs.yml
+-rw-r--r--   0        0        0     2121 2020-02-02 00:00:00.000000 decision_tree_morfist-0.4.0/requirements-dev.lock
+-rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 decision_tree_morfist-0.4.0/requirements.lock
+-rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 decision_tree_morfist-0.4.0/.github/workflows/pre-commit.yml
+-rw-r--r--   0        0        0     3981 2020-02-02 00:00:00.000000 decision_tree_morfist-0.4.0/docs/index.md
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 decision_tree_morfist-0.4.0/morfist/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 decision_tree_morfist-0.4.0/morfist/algo/__init__.py
+-rw-r--r--   0        0        0     2360 2020-02-02 00:00:00.000000 decision_tree_morfist-0.4.0/morfist/algo/evaluation.py
+-rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 decision_tree_morfist-0.4.0/morfist/algo/histogram.py
+-rw-r--r--   0        0        0     4840 2020-02-02 00:00:00.000000 decision_tree_morfist-0.4.0/morfist/core/MixedRandomForest.py
+-rw-r--r--   0        0        0     4852 2020-02-02 00:00:00.000000 decision_tree_morfist-0.4.0/morfist/core/MixedRandomTree.py
+-rw-r--r--   0        0        0     6269 2020-02-02 00:00:00.000000 decision_tree_morfist-0.4.0/morfist/core/MixedSplitter.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 decision_tree_morfist-0.4.0/morfist/core/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 decision_tree_morfist-0.4.0/morfist/legacy/__init__.py
+-rw-r--r--   0        0        0    10959 2020-02-02 00:00:00.000000 decision_tree_morfist-0.4.0/morfist/legacy/core.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 decision_tree_morfist-0.4.0/tests/__init__.py
+-rw-r--r--   0        0        0     2672 2020-02-02 00:00:00.000000 decision_tree_morfist-0.4.0/tests/test_comparison_classification.py
+-rw-r--r--   0        0        0     2473 2020-02-02 00:00:00.000000 decision_tree_morfist-0.4.0/tests/test_comparison_regression.py
+-rw-r--r--   0        0        0     3429 2020-02-02 00:00:00.000000 decision_tree_morfist-0.4.0/tests/test_mixed.py
+-rw-r--r--   0        0        0     1337 2020-02-02 00:00:00.000000 decision_tree_morfist-0.4.0/.gitignore
+-rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 decision_tree_morfist-0.4.0/LICENSE
+-rw-r--r--   0        0        0     2265 2020-02-02 00:00:00.000000 decision_tree_morfist-0.4.0/README.md
+-rw-r--r--   0        0        0     1933 2020-02-02 00:00:00.000000 decision_tree_morfist-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     3449 2020-02-02 00:00:00.000000 decision_tree_morfist-0.4.0/PKG-INFO
```

### Comparing `decision-tree-morfist-0.3.3/LICENSE` & `decision_tree_morfist-0.4.0/LICENSE`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2018 Henrik Linusson
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2018 Henrik Linusson
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `decision-tree-morfist-0.3.3/README.md` & `decision_tree_morfist-0.4.0/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,59 +1,66 @@
-# morfist: mixed-output-rf
-Multi-target Random Forest implementation that can mix both classification and regression tasks.
-
-Morfist implements the Random Forest algorithm (Breiman, 2001)
-with support for mixed-task multi-task learning, i.e., it is possible to train the model on any number
-of classification tasks and regression tasks, simultaneously. Morfist's mixed multi-task learning implementation follows that proposed by Linusson (2013). 
-
-* [Breiman, L. (2001). Random forests. Machine learning, 45(1), 5-32](https://link.springer.com/article/10.1023%2FA%3A1010933404324).
-* [Linusson, H. (2013). Multi-output random forests](https://pdfs.semanticscholar.org/4219/f87ed41c558d43cf78f63976cf87bcd7ebb0.pdf).
-
-## Installation
-
-With pip:
-```
-pip install decision-tree-morfist
-```
-With conda:
-```
-conda install -c systemallica decision-tree-morfist
-```
-## Usage
-
-### Initialising the model
-
-- Similarly to a scikit-learn [RandomForestClassifier](https://scikit-learn.org/stable/modules/generated/sklearn.ensemble.RandomForestClassifier.html), a MixedRandomForest can be initialised in this way:
-```
-from morfist import MixedRandomForest
-
-mrf = MixedRandomForest(
-    n_estimators=n_trees,
-    min_samples_leaf=1,
-    classification_targets=[0]
-)
-```
-
-For more info on the possible parameters, visit the [documentation](https://systemallica.github.io/morfist/).
-
-### Training the model
-
-- Once the model is initialised, it can be fitted like this:
-    ```
-    mrf.fit(X, y)
-    ```
-    Where X are the training examples and Y are their respective labels(if they are categorical) or values(if they are numerical)
-
-### Prediction
-
-- The model can be now used to predict new instances.
-    - Class/value:
-    ```
-    mrf.predict(x)
-    ```
-    - Probability:
-    ```
-    mrf.predict_proba(x)
-    ```
-  
-## TODO:
-* Speed up the learning algorithm implementation (morfist is currently **much** slower than the Random Forest implementation available in scikit-learn) 
+# morfist: mixed-output-rf
+Multi-target Random Forest implementation that can mix both classification and regression tasks.
+
+Morfist implements the Random Forest algorithm (Breiman, 2001)
+with support for mixed-task multi-task learning, i.e., it is possible to train the model on any number
+of classification tasks and regression tasks, simultaneously. Morfist's mixed multi-task learning implementation follows that proposed by Linusson (2013). 
+
+* [Breiman, L. (2001). Random forests. Machine learning, 45(1), 5-32](https://link.springer.com/article/10.1023%2FA%3A1010933404324).
+* [Linusson, H. (2013). Multi-output random forests](https://pdfs.semanticscholar.org/4219/f87ed41c558d43cf78f63976cf87bcd7ebb0.pdf).
+
+## Installation
+
+With pip:
+```
+pip install decision-tree-morfist
+```
+With conda:
+```
+conda install -c systemallica decision-tree-morfist
+```
+## Usage
+
+### Initialising the model
+
+- Similarly to a scikit-learn [RandomForestClassifier](https://scikit-learn.org/stable/modules/generated/sklearn.ensemble.RandomForestClassifier.html), a MixedRandomForest can be initialised in this way:
+```
+from morfist import MixedRandomForest
+
+mrf = MixedRandomForest(
+    n_estimators=n_trees,
+    min_samples_leaf=1,
+    classification_targets=[0]
+)
+```
+
+For more info on the possible parameters, visit the [documentation](https://systemallica.github.io/morfist/).
+
+### Training the model
+
+- Once the model is initialised, it can be fitted like this:
+    ```
+    mrf.fit(X, y)
+    ```
+    Where X are the training examples and Y are their respective labels(if they are categorical) or values(if they are numerical)
+
+### Prediction
+
+- The model can be now used to predict new instances.
+    - Class/value:
+    ```
+    mrf.predict(x)
+    ```
+    - Probability:
+    ```
+    mrf.predict_proba(x)
+    ``` 
+ 
+## Run/Build locally
+To run the project, you need [Poetry](https://python-poetry.org). Once installed:
+
+1. Clone the repository.
+2. Run `poetry install`.
+3. The development environment is ready. You can test it by running `pytest`.
+
+## TODO:
+* Speed up the learning algorithm implementation (morfist is currently **much** slower than the Random Forest implementation available in scikit-learn)
```

### Comparing `decision-tree-morfist-0.3.3/morfist/algo/evaluation.py` & `decision_tree_morfist-0.4.0/morfist/algo/evaluation.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,75 +1,79 @@
-import copy
-
-import numpy as np
-
-
-def accuracy(y, y_hat):
-    # Calculate classification accuracy of model
-    return (y.astype(int) == y_hat.astype(int)).sum() / y.size
-
-
-def rmse(y, y_hat):
-    # Calculate root squared mean error of model
-    return np.sqrt(((y - y_hat) ** 2).mean())
-
-
-def cross_validation(model,
-                     x,
-                     y,
-                     folds=10,
-                     classification_targets=None,
-                     classification_eval=accuracy,
-                     reg_eval=rmse,
-                     verbose=False):
-    """Perform cross validation on a model
-
-    :param model:  model to be validated
-    :param x: X values of the data set
-    :param y: Y values of the data set
-    :param folds: number of folds
-    :param classification_targets: features that are part of the classification task
-    :param classification_eval: function to evaluate model classification accuracy
-    :param reg_eval: function to evaluate model regression accuracy
-    :param verbose: used for debug purposes
-    :return: scores[]:
-                 0: classification accuracy
-                 1: regression RMSE
-    """
-    classification_targets = classification_targets if classification_targets is not None else []
-
-    idx = np.random.permutation(x.shape[0])
-    fold_size = int(idx.size / folds)
-
-    if y.ndim == 1:
-        y = y.reshape((y.size, 1))
-
-    y_hat = np.zeros((idx.size, y.shape[1]))
-
-    # Perform the cross-validation
-    # Train and fit the model for different subsets of the data
-    for i in range(folds):
-        if verbose:
-            print('Running fold {} of {} ...'.format(i + 1, folds))
-
-        fold_start = i * fold_size
-        fold_stop = min((i + 1) * fold_size, idx.size)
-
-        mask = np.ones(idx.size, dtype=bool)
-        mask[fold_start:fold_stop] = 0
-
-        train_idx = idx[mask]
-        test_idx = idx[(1 - mask).astype(bool)]
-
-        m = copy.copy(model)
-        m.fit(x[train_idx, :], y[train_idx, :])
-        y_hat[test_idx, :] = m.predict(x[test_idx, :])
-
-    scores = np.zeros(y.shape[1])
-    # Calculate the classification and regression accuracy of the model
-    for i in range(y.shape[1]):
-        if i in classification_targets:
-            scores[i] = classification_eval(y[:, i], y_hat[:, i])
-        else:
-            scores[i] = reg_eval(y[:, i], y_hat[:, i])
-
-    return scores
+import copy
+
+import numpy as np
+
+
+def accuracy(y, y_hat):
+    # Calculate classification accuracy of model
+    return (y.astype(int) == y_hat.astype(int)).sum() / y.size
+
+
+def rmse(y, y_hat):
+    # Calculate root squared mean error of model
+    return np.sqrt(((y - y_hat) ** 2).mean())
+
+
+def cross_validation(
+    model,
+    x,
+    y,
+    folds=10,
+    classification_targets=None,
+    classification_eval=accuracy,
+    reg_eval=rmse,
+    verbose=False,
+):
+    """Perform cross validation on a model
+
+    :param model:  model to be validated
+    :param x: X values of the data set
+    :param y: Y values of the data set
+    :param folds: number of folds
+    :param classification_targets: features that are part of the classification task
+    :param classification_eval: function to evaluate model classification accuracy
+    :param reg_eval: function to evaluate model regression accuracy
+    :param verbose: used for debug purposes
+    :return: scores[]:
+                 0: classification accuracy
+                 1: regression RMSE
+    """
+    classification_targets = (
+        classification_targets if classification_targets is not None else []
+    )
+
+    idx = np.random.permutation(x.shape[0])
+    fold_size = int(idx.size / folds)
+
+    if y.ndim == 1:
+        y = y.reshape((y.size, 1))
+
+    y_hat = np.zeros((idx.size, y.shape[1]))
+
+    # Perform the cross-validation
+    # Train and fit the model for different subsets of the data
+    for i in range(folds):
+        if verbose:
+            print("Running fold {} of {} ...".format(i + 1, folds))
+
+        fold_start = i * fold_size
+        fold_stop = min((i + 1) * fold_size, idx.size)
+
+        mask = np.ones(idx.size, dtype=bool)
+        mask[fold_start:fold_stop] = 0
+
+        train_idx = idx[mask]
+        test_idx = idx[(1 - mask).astype(bool)]
+
+        m = copy.copy(model)
+        m.fit(x[train_idx, :], y[train_idx, :])
+        y_hat[test_idx, :] = m.predict(x[test_idx, :])
+
+    scores = np.zeros(y.shape[1])
+    # Calculate the classification and regression accuracy of the model
+    for i in range(y.shape[1]):
+        if i in classification_targets:
+            scores[i] = classification_eval(y[:, i], y_hat[:, i])
+        else:
+            scores[i] = reg_eval(y[:, i], y_hat[:, i])
+
+    return scores
```

### Comparing `decision-tree-morfist-0.3.3/morfist/core/MixedRandomForest.py` & `decision_tree_morfist-0.4.0/morfist/core/MixedRandomForest.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,117 +1,125 @@
-import numpy as np
-import scipy.stats
-
-from morfist.core.MixedRandomTree import MixedRandomTree
-
-
-class MixedRandomForest:
-    def __str__(self):
-        params = "("
-        i = 0
-        for key in self.__dict__:
-            if i == 0:
-                params += str(key) + "=" + str(self.__dict__[key]) + ", \n"
-            elif i == len(self.__dict__) - 1:
-                params += "\t\t\t" + str(key) + "=" + str(self.__dict__[key]) + ")"
-            else:
-                params += "\t\t\t" + str(key) + "=" + str(self.__dict__[key]) + ", \n"
-            i += 1
-        return self.__class__.__name__ + params
-
-    def __init__(self,
-                 n_estimators=10,
-                 max_features='sqrt',
-                 min_samples_leaf=5,
-                 choose_split='mean',
-                 classification_targets=None):
-        """Build a printable Random Forest model
-
-        :param n_estimators: number of trees in the forest
-        :param max_features: the number of features to consider when looking for the best split
-        :param min_samples_leaf: minimum amount of samples in each leaf
-        :param choose_split: method to use to find the best split
-        :param classification_targets: features that are part of the classification task
-        """
-        self.n_estimators = n_estimators
-        self.min_samples_leaf = min_samples_leaf
-        self.max_features = max_features
-        self.classification_targets = classification_targets if classification_targets is not None else []
-        self.choose_split = choose_split
-        self.n_targets = 0
-        self.classification_labels = {}
-        self.estimators = []
-
-    # Fit the model
-    def fit(self, x, y):
-        self.estimators = []
-
-        if y.ndim == 1:
-            y = y.reshape((y.size, 1))
-        self.n_targets = y.shape[1]
-
-        # Get the classification labels
-        # It takes the unique labels of the specified classification variables
-        for i in filter(lambda j: j in self.classification_targets, range(self.n_targets)):
-            self.classification_labels[i] = np.unique(y[:, i])
-
-        n_train = x.shape[0]
-        # Train the random trees that are part of the forest
-        for i in range(self.n_estimators):
-            m = MixedRandomTree(self.max_features,
-                                self.min_samples_leaf,
-                                self.choose_split,
-                                self.classification_targets)
-
-            # It is a random forest so the trees are built with random subsets of the data
-            sample_idx = np.random.choice(np.arange(n_train),
-                                          n_train,
-                                          replace=True)
-
-            m.fit(x[sample_idx, :], y[sample_idx, :])
-            self.estimators.append(m)
-
-    # Predict the class/value of an instance
-    def predict(self, x):
-        n_test = x.shape[0]
-        pred = np.zeros((n_test, self.n_targets, self.n_estimators))
-        for i, m in enumerate(self.estimators):
-            pred[:, :, i] = m.predict(x)
-
-        pred_avg = np.zeros((n_test, self.n_targets))
-        for i in range(self.n_targets):
-            # Predict categorical value
-            if i in self.classification_targets:
-                pred_avg[:, i], _ = scipy.stats.mode(pred[:, i, :].T)
-            # Predict numerical value
-            else:
-                pred_avg[:, i] = pred[:, i, :].mean(axis=1)
-
-        return pred_avg
-
-    # Predict the probability of an instance
-    def predict_proba(self, x):
-        n_test = x.shape[0]
-        pred = np.zeros((n_test, self.n_targets, self.n_estimators))
-        for i, m in enumerate(self.estimators):
-            pred[:, :, i] = m.predict(x)
-
-        pred_avg = np.zeros((n_test, self.n_targets), dtype=object)
-        for i in range(self.n_targets):
-            if i in self.classification_targets:
-                for j in range(n_test):
-                    freq = np.bincount(pred[j, i, :].T.astype(int),
-                                       minlength=self.classification_labels[i].size)
-
-                    # Fix for a weird bug TODO: find the root cause
-                    if len(freq) > self.classification_labels[i].size:
-                        freq_fixed = np.zeros(self.classification_labels[i].size)
-                        for x in range(len(self.classification_labels[i])):
-                            idx = int(self.classification_labels[i][x])
-                            freq_fixed[x] = freq[idx]
-                        pred_avg[j, i] = freq_fixed / self.n_estimators
-                    else:
-                        pred_avg[j, i] = freq / self.n_estimators
-            else:
-                pred_avg[:, i] = pred[:, i, :].mean(axis=1)
-
-        return pred_avg
+import numpy as np
+import scipy.stats
+
+from morfist.core.MixedRandomTree import MixedRandomTree
+
+
+class MixedRandomForest:
+    def __str__(self):
+        params = "("
+        i = 0
+        for key in self.__dict__:
+            if i == 0:
+                params += str(key) + "=" + str(self.__dict__[key]) + ", \n"
+            elif i == len(self.__dict__) - 1:
+                params += "\t\t\t" + str(key) + "=" + str(self.__dict__[key]) + ")"
+            else:
+                params += "\t\t\t" + str(key) + "=" + str(self.__dict__[key]) + ", \n"
+            i += 1
+        return self.__class__.__name__ + params
+
+    def __init__(
+        self,
+        n_estimators=10,
+        max_features="sqrt",
+        min_samples_leaf=5,
+        choose_split="mean",
+        classification_targets=None,
+    ):
+        """Build a printable Random Forest model
+
+        :param n_estimators: number of trees in the forest
+        :param max_features: the number of features to consider when looking for the best split
+        :param min_samples_leaf: minimum amount of samples in each leaf
+        :param choose_split: method to use to find the best split
+        :param classification_targets: features that are part of the classification task
+        """
+        self.n_estimators = n_estimators
+        self.min_samples_leaf = min_samples_leaf
+        self.max_features = max_features
+        self.classification_targets = (
+            classification_targets if classification_targets is not None else []
+        )
+        self.choose_split = choose_split
+        self.n_targets = 0
+        self.classification_labels = {}
+        self.estimators = []
+
+    # Fit the model
+    def fit(self, x, y):
+        self.estimators = []
+
+        if y.ndim == 1:
+            y = y.reshape((y.size, 1))
+        self.n_targets = y.shape[1]
+
+        # Get the classification labels
+        # It takes the unique labels of the specified classification variables
+        for i in filter(
+            lambda j: j in self.classification_targets, range(self.n_targets)
+        ):
+            self.classification_labels[i] = np.unique(y[:, i])
+
+        n_train = x.shape[0]
+        # Train the random trees that are part of the forest
+        for i in range(self.n_estimators):
+            m = MixedRandomTree(
+                self.max_features,
+                self.min_samples_leaf,
+                self.choose_split,
+                self.classification_targets,
+            )
+
+            # It is a random forest so the trees are built with random subsets of the data
+            sample_idx = np.random.choice(np.arange(n_train), n_train, replace=True)
+
+            m.fit(x[sample_idx, :], y[sample_idx, :])
+            self.estimators.append(m)
+
+    # Predict the class/value of an instance
+    def predict(self, x):
+        n_test = x.shape[0]
+        pred = np.zeros((n_test, self.n_targets, self.n_estimators))
+        for i, m in enumerate(self.estimators):
+            pred[:, :, i] = m.predict(x)
+
+        pred_avg = np.zeros((n_test, self.n_targets))
+        for i in range(self.n_targets):
+            # Predict categorical value
+            if i in self.classification_targets:
+                pred_avg[:, i], _ = scipy.stats.mode(pred[:, i, :].T)
+            # Predict numerical value
+            else:
+                pred_avg[:, i] = pred[:, i, :].mean(axis=1)
+
+        return pred_avg
+
+    # Predict the probability of an instance
+    def predict_proba(self, x):
+        n_test = x.shape[0]
+        pred = np.zeros((n_test, self.n_targets, self.n_estimators))
+        for i, m in enumerate(self.estimators):
+            pred[:, :, i] = m.predict(x)
+
+        pred_avg = np.zeros((n_test, self.n_targets), dtype=object)
+        for i in range(self.n_targets):
+            if i in self.classification_targets:
+                for j in range(n_test):
+                    freq = np.bincount(
+                        pred[j, i, :].T.astype(int),
+                        minlength=self.classification_labels[i].size,
+                    )
+
+                    # Fix for a weird bug TODO: find the root cause
+                    if len(freq) > self.classification_labels[i].size:
+                        freq_fixed = np.zeros(self.classification_labels[i].size)
+                        for x in range(len(self.classification_labels[i])):
+                            idx = int(self.classification_labels[i][x])
+                            freq_fixed[x] = freq[idx]
+                        pred_avg[j, i] = freq_fixed / self.n_estimators
+                    else:
+                        pred_avg[j, i] = freq / self.n_estimators
+            else:
+                pred_avg[:, i] = pred[:, i, :].mean(axis=1)
+
+        return pred_avg
```

### Comparing `decision-tree-morfist-0.3.3/morfist/core/MixedSplitter.py` & `decision_tree_morfist-0.4.0/morfist/core/MixedSplitter.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,172 +1,176 @@
-import numpy as np
-from numba import njit
-
-from morfist.algo.histogram import numba_histogram
-
-
-@njit
-def impurity_classification(y_classification):
-    # Calculate the impurity value for the classification task
-
-    # Cast to integer
-    y_class = y_classification.astype(np.int8)
-
-    # Calculate frequencies
-    frequency = np.bincount(y_class) / y_class.size
-
-    result = 0
-    for i in range(frequency.size):
-        if frequency[i]:
-            result += frequency[i] * np.log2(frequency[i])
-
-    return 0 - result
-
-
-@njit
-def impurity_regression(y, y_regression):
-    # Calculate the impurity value for the regression task
-
-    if np.unique(y_regression).size < 2:
-        return 0
-
-    n_bins = 100
-    bin_width = (y.max() - y.min()) / n_bins
-
-    frequency, _ = numba_histogram(y_regression, n_bins)
-    frequency_float = frequency.astype(np.float64)
-    frequency_float = (frequency_float / len(y)) / bin_width
-
-    probability = (frequency_float + 1) / (frequency_float.sum() + n_bins)
-
-    return 0 - bin_width * (probability * np.log2(probability)).sum()
-
-
-@njit
-def get_gain(imp_n_left, imp_n_right, imp_n, imp_root, n_left, n_right, n_parent):
-    impurity_left = imp_n_left / imp_root
-    impurity_right = imp_n_right / imp_root
-    impurity_parent = imp_n / imp_root
-
-    gain_left = (n_left / n_parent) * (impurity_parent - impurity_left)
-    gain_right = (n_right / n_parent) * (impurity_parent - impurity_right)
-    return gain_left + gain_right
-
-
-def get_max_features(max_features, n_features):
-    # Maximum number of features to try for the best split
-    n_max_features = n_features
-    if max_features == 'sqrt':
-        n_max_features = int(np.sqrt(n_features))
-    elif max_features == 'log2':
-        n_max_features = int(np.log2(n_features))
-    elif isinstance(max_features, float):
-        n_max_features = int(max_features * n_features)
-    elif max_features is None:
-        n_max_features = n_features
-
-    return n_max_features
-
-
-class MixedSplitter:
-    def __init__(self,
-                 x,
-                 y,
-                 max_features='sqrt',
-                 min_samples_leaf=5,
-                 choose_split='mean',
-                 classification_targets=None):
-        """Class in charge of finding the best split at every given moment
-
-        :param x: training data
-        :param y: target data
-        :param max_features: the number of features to consider when looking for the best split
-        :param min_samples_leaf: minimum amount of samples in each leaf
-        :param choose_split:  method used to find the best split
-        :param classification_targets: features that are part of the classification task
-        """
-        self.n_train = x.shape[0]
-        self.n_features = x.shape[1]
-        self.n_targets = y.shape[1]
-        self.classification_targets = classification_targets if classification_targets is not None else []
-        self.max_features = get_max_features(max_features, self.n_features)
-        self.min_samples_leaf = min_samples_leaf
-        self.root_impurity = self.__impurity_node(y)
-        self.choose_split = choose_split
-
-    def split(self, x, y):
-        # If there are not enough features in the leaf, stop splitting
-        if x.shape[0] <= self.min_samples_leaf:
-            return None, None, np.inf
-
-        # Best feature
-        best_feature = None
-        # Best value
-        best_value = None
-        # Best impurity
-        best_impurity = -np.inf
-
-        # Random selection of the features to try for the best split
-        try_features = np.random.choice(
-            np.arange(self.n_features),
-            self.max_features,
-            replace=False
-        )
-
-        # Try each of the selected features and find which of them gives the best split(higher impurity)
-        for feature in try_features:
-            # Get the unique possible values for this particular feature
-            values = np.unique(x[:, feature])
-
-            # Split value selection(random value subsampling): Boström (2011)
-            #   Two random feature values are selected, and a split is attempted at their mean
-            if values.size < 2:
-                continue
-            values = (values[:-1] + values[1:]) / 2
-            value = np.random.choice(values)
-
-            # Try to split with this specific combination of feature and value
-            left_idx = x[:, feature] <= value
-            right_idx = x[:, feature] > value
-
-            impurity = self.__impurity_split(y, y[left_idx, :], y[right_idx, :])
-            # If it's better than the previous saved one, save the values
-            if impurity > best_impurity:
-                best_feature, best_value, best_impurity = feature, value, impurity
-
-        return best_feature, best_value, best_impurity
-
-    # Calculate the impurity of a split
-    def __impurity_split(self, y_parent, y_left, y_right):
-        n_left = y_left.shape[0]
-        n_right = y_right.shape[0]
-        if n_left < self.min_samples_leaf or n_right < self.min_samples_leaf:
-            return np.inf
-        else:
-            n_parent = y_parent.shape[0]
-
-            gain = get_gain(self.__impurity_node(y_left),
-                            self.__impurity_node(y_right),
-                            self.__impurity_node(y_parent),
-                            self.root_impurity,
-                            n_left,
-                            n_right,
-                            n_parent)
-
-            if self.choose_split == 'mean':
-                return gain.mean()
-            elif self.choose_split == 'random':
-                return np.random.choice(gain)
-            else:
-                return gain.max()
-
-    def __impurity_node(self, y):
-        # Calculate the impurity of a node
-        delta = 0.0001
-        impurity = np.zeros(self.n_targets)
-        # Calculate the impurity value for each of the targets(classification or regression)
-        for i in range(self.n_targets):
-            if i in self.classification_targets:
-                impurity[i] = impurity_classification(y[:, i]) + delta
-            else:
-                impurity[i] = impurity_regression(y, y[:, i]) + delta
-        return impurity
+import numpy as np
+from numba import njit
+
+from morfist.algo.histogram import numba_histogram
+
+
+@njit
+def impurity_classification(y_classification):
+    # Calculate the impurity value for the classification task
+
+    # Cast to integer
+    y_class = y_classification.astype(np.int8)
+
+    # Calculate frequencies
+    frequency = np.bincount(y_class) / y_class.size
+
+    result = 0
+    for i in range(frequency.size):
+        if frequency[i]:
+            result += frequency[i] * np.log2(frequency[i])
+
+    return 0 - result
+
+
+@njit
+def impurity_regression(y, y_regression):
+    # Calculate the impurity value for the regression task
+
+    if np.unique(y_regression).size < 2:
+        return 0
+
+    n_bins = 100
+    bin_width = (y.max() - y.min()) / n_bins
+
+    frequency, _ = numba_histogram(y_regression, n_bins)
+    frequency_float = frequency.astype(np.float64)
+    frequency_float = (frequency_float / len(y)) / bin_width
+
+    probability = (frequency_float + 1) / (frequency_float.sum() + n_bins)
+
+    return 0 - bin_width * (probability * np.log2(probability)).sum()
+
+
+@njit
+def get_gain(imp_n_left, imp_n_right, imp_n, imp_root, n_left, n_right, n_parent):
+    impurity_left = imp_n_left / imp_root
+    impurity_right = imp_n_right / imp_root
+    impurity_parent = imp_n / imp_root
+
+    gain_left = (n_left / n_parent) * (impurity_parent - impurity_left)
+    gain_right = (n_right / n_parent) * (impurity_parent - impurity_right)
+    return gain_left + gain_right
+
+
+def get_max_features(max_features, n_features):
+    # Maximum number of features to try for the best split
+    n_max_features = n_features
+    if max_features == "sqrt":
+        n_max_features = int(np.sqrt(n_features))
+    elif max_features == "log2":
+        n_max_features = int(np.log2(n_features))
+    elif isinstance(max_features, float):
+        n_max_features = int(max_features * n_features)
+    elif max_features is None:
+        n_max_features = n_features
+
+    return n_max_features
+
+
+class MixedSplitter:
+    def __init__(
+        self,
+        x,
+        y,
+        max_features="sqrt",
+        min_samples_leaf=5,
+        choose_split="mean",
+        classification_targets=None,
+    ):
+        """Class in charge of finding the best split at every given moment
+
+        :param x: training data
+        :param y: target data
+        :param max_features: the number of features to consider when looking for the best split
+        :param min_samples_leaf: minimum amount of samples in each leaf
+        :param choose_split:  method used to find the best split
+        :param classification_targets: features that are part of the classification task
+        """
+        self.n_train = x.shape[0]
+        self.n_features = x.shape[1]
+        self.n_targets = y.shape[1]
+        self.classification_targets = (
+            classification_targets if classification_targets is not None else []
+        )
+        self.max_features = get_max_features(max_features, self.n_features)
+        self.min_samples_leaf = min_samples_leaf
+        self.root_impurity = self.__impurity_node(y)
+        self.choose_split = choose_split
+
+    def split(self, x, y):
+        # If there are not enough features in the leaf, stop splitting
+        if x.shape[0] <= self.min_samples_leaf:
+            return None, None, np.inf
+
+        # Best feature
+        best_feature = None
+        # Best value
+        best_value = None
+        # Best impurity
+        best_impurity = -np.inf
+
+        # Random selection of the features to try for the best split
+        try_features = np.random.choice(
+            np.arange(self.n_features), self.max_features, replace=False
+        )
+
+        # Try each of the selected features and find which of them gives the best split(higher impurity)
+        for feature in try_features:
+            # Get the unique possible values for this particular feature
+            values = np.unique(x[:, feature])
+
+            # Split value selection(random value subsampling): Boström (2011)
+            #   Two random feature values are selected, and a split is attempted at their mean
+            if values.size < 2:
+                continue
+            values = (values[:-1] + values[1:]) / 2
+            value = np.random.choice(values)
+
+            # Try to split with this specific combination of feature and value
+            left_idx = x[:, feature] <= value
+            right_idx = x[:, feature] > value
+
+            impurity = self.__impurity_split(y, y[left_idx, :], y[right_idx, :])
+            # If it's better than the previous saved one, save the values
+            if impurity > best_impurity:
+                best_feature, best_value, best_impurity = feature, value, impurity
+
+        return best_feature, best_value, best_impurity
+
+    # Calculate the impurity of a split
+    def __impurity_split(self, y_parent, y_left, y_right):
+        n_left = y_left.shape[0]
+        n_right = y_right.shape[0]
+        if n_left < self.min_samples_leaf or n_right < self.min_samples_leaf:
+            return np.inf
+        else:
+            n_parent = y_parent.shape[0]
+
+            gain = get_gain(
+                self.__impurity_node(y_left),
+                self.__impurity_node(y_right),
+                self.__impurity_node(y_parent),
+                self.root_impurity,
+                n_left,
+                n_right,
+                n_parent,
+            )
+
+            if self.choose_split == "mean":
+                return gain.mean()
+            elif self.choose_split == "random":
+                return np.random.choice(gain)
+            else:
+                return gain.max()
+
+    def __impurity_node(self, y):
+        # Calculate the impurity of a node
+        delta = 0.0001
+        impurity = np.zeros(self.n_targets)
+        # Calculate the impurity value for each of the targets(classification or regression)
+        for i in range(self.n_targets):
+            if i in self.classification_targets:
+                impurity[i] = impurity_classification(y[:, i]) + delta
+            else:
+                impurity[i] = impurity_regression(y, y[:, i]) + delta
+        return impurity
```

### Comparing `decision-tree-morfist-0.3.3/setup.py` & `decision_tree_morfist-0.4.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,30 +1,92 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.3
+Name: decision-tree-morfist
+Version: 0.4.0
+Summary: Multi-target Random Forest implementation that can mix both classification and regression tasks.
+Project-URL: Documentation, https://systemallica.github.io/morfist/
+Project-URL: Repository, https://github.com/systemallica/morfist
+Project-URL: Changelog, https://github.com/systemallica/morfist/blob/main/CHANGELOG.md
+Author-email: Andrés Reverón Molina <andres@reveronmolina.me>, Henrik Linusson <henrik.linusson@hb.se>
+Maintainer-email: Andrés Reverón Molina <andres@reveronmolina.me>
+License-Expression: MIT
+License-File: LICENSE
+Classifier: Development Status :: 3 - Alpha
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Python: >=3.8
+Requires-Dist: numba>=0.59.1
+Requires-Dist: numpy>=1.26.4
+Requires-Dist: scipy>=1.13.0
+Description-Content-Type: text/markdown
+
+# morfist: mixed-output-rf
+Multi-target Random Forest implementation that can mix both classification and regression tasks.
+
+Morfist implements the Random Forest algorithm (Breiman, 2001)
+with support for mixed-task multi-task learning, i.e., it is possible to train the model on any number
+of classification tasks and regression tasks, simultaneously. Morfist's mixed multi-task learning implementation follows that proposed by Linusson (2013). 
+
+* [Breiman, L. (2001). Random forests. Machine learning, 45(1), 5-32](https://link.springer.com/article/10.1023%2FA%3A1010933404324).
+* [Linusson, H. (2013). Multi-output random forests](https://pdfs.semanticscholar.org/4219/f87ed41c558d43cf78f63976cf87bcd7ebb0.pdf).
+
+## Installation
+
+With pip:
+```
+pip install decision-tree-morfist
+```
+With conda:
+```
+conda install -c systemallica decision-tree-morfist
+```
+## Usage
+
+### Initialising the model
+
+- Similarly to a scikit-learn [RandomForestClassifier](https://scikit-learn.org/stable/modules/generated/sklearn.ensemble.RandomForestClassifier.html), a MixedRandomForest can be initialised in this way:
+```
+from morfist import MixedRandomForest
+
+mrf = MixedRandomForest(
+    n_estimators=n_trees,
+    min_samples_leaf=1,
+    classification_targets=[0]
+)
+```
+
+For more info on the possible parameters, visit the [documentation](https://systemallica.github.io/morfist/).
+
+### Training the model
+
+- Once the model is initialised, it can be fitted like this:
+    ```
+    mrf.fit(X, y)
+    ```
+    Where X are the training examples and Y are their respective labels(if they are categorical) or values(if they are numerical)
+
+### Prediction
+
+- The model can be now used to predict new instances.
+    - Class/value:
+    ```
+    mrf.predict(x)
+    ```
+    - Probability:
+    ```
+    mrf.predict_proba(x)
+    ``` 
+ 
+## Run/Build locally
+To run the project, you need [Poetry](https://python-poetry.org). Once installed:
+
+1. Clone the repository.
+2. Run `poetry install`.
+3. The development environment is ready. You can test it by running `pytest`.
 
-packages = \
-['morfist', 'morfist.algo', 'morfist.core', 'morfist.legacy']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['numba>=0.51.0,<0.52.0', 'numpy>=1.19.1,<2.0.0', 'scipy>=1.5.2,<2.0.0']
-
-setup_kwargs = {
-    'name': 'decision-tree-morfist',
-    'version': '0.3.3',
-    'description': 'Multi-target Random Forest implementation that can mix both classification and regression tasks.',
-    'long_description': "# morfist: mixed-output-rf\nMulti-target Random Forest implementation that can mix both classification and regression tasks.\n\nMorfist implements the Random Forest algorithm (Breiman, 2001)\nwith support for mixed-task multi-task learning, i.e., it is possible to train the model on any number\nof classification tasks and regression tasks, simultaneously. Morfist's mixed multi-task learning implementation follows that proposed by Linusson (2013). \n\n* [Breiman, L. (2001). Random forests. Machine learning, 45(1), 5-32](https://link.springer.com/article/10.1023%2FA%3A1010933404324).\n* [Linusson, H. (2013). Multi-output random forests](https://pdfs.semanticscholar.org/4219/f87ed41c558d43cf78f63976cf87bcd7ebb0.pdf).\n\n## Installation\n\nWith pip:\n```\npip install decision-tree-morfist\n```\nWith conda:\n```\nconda install -c systemallica decision-tree-morfist\n```\n## Usage\n\n### Initialising the model\n\n- Similarly to a scikit-learn [RandomForestClassifier](https://scikit-learn.org/stable/modules/generated/sklearn.ensemble.RandomForestClassifier.html), a MixedRandomForest can be initialised in this way:\n```\nfrom morfist import MixedRandomForest\n\nmrf = MixedRandomForest(\n    n_estimators=n_trees,\n    min_samples_leaf=1,\n    classification_targets=[0]\n)\n```\n\nFor more info on the possible parameters, visit the [documentation](https://systemallica.github.io/morfist/).\n\n### Training the model\n\n- Once the model is initialised, it can be fitted like this:\n    ```\n    mrf.fit(X, y)\n    ```\n    Where X are the training examples and Y are their respective labels(if they are categorical) or values(if they are numerical)\n\n### Prediction\n\n- The model can be now used to predict new instances.\n    - Class/value:\n    ```\n    mrf.predict(x)\n    ```\n    - Probability:\n    ```\n    mrf.predict_proba(x)\n    ```\n  \n## TODO:\n* Speed up the learning algorithm implementation (morfist is currently **much** slower than the Random Forest implementation available in scikit-learn) \n",
-    'author': 'Andrés Reverón Molina',
-    'author_email': 'andres@reveronmolina.me',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://github.com/systemallica/morfist',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.8.0,<4.0.0',
-}
-
-
-setup(**setup_kwargs)
+## TODO:
+* Speed up the learning algorithm implementation (morfist is currently **much** slower than the Random Forest implementation available in scikit-learn)
```

