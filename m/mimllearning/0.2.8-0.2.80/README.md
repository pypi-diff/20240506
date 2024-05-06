# Comparing `tmp/mimllearning-0.2.8.tar.gz` & `tmp/mimllearning-0.2.80.tar.gz`

## Comparing `mimllearning-0.2.8.tar` & `mimllearning-0.2.80.tar`

### file list

```diff
@@ -1,45 +1,44 @@
--rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 mimllearning-0.2.8/readme.md
--rw-r--r--   0        0        0   258069 2020-02-02 00:00:00.000000 mimllearning-0.2.8/documentation/AnteproyectoDamianTFG.pdf
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 mimllearning-0.2.8/src/miml/__init__.py
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 mimllearning-0.2.8/src/miml/classifier/__init__.py
--rw-r--r--   0        0        0     1762 2020-02-02 00:00:00.000000 mimllearning-0.2.8/src/miml/classifier/miml_classifier.py
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 mimllearning-0.2.8/src/miml/classifier/mi/__init__.py
--rw-r--r--   0        0        0     2636 2020-02-02 00:00:00.000000 mimllearning-0.2.8/src/miml/classifier/mi/all_positive_apr_classifier.py
--rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 mimllearning-0.2.8/src/miml/classifier/mi/apr_classifier.py
--rw-r--r--   0        0        0     4541 2020-02-02 00:00:00.000000 mimllearning-0.2.8/src/miml/classifier/mi/iterated_discrim_apr_classifier.py
--rw-r--r--   0        0        0     1246 2020-02-02 00:00:00.000000 mimllearning-0.2.8/src/miml/classifier/mi/miles_classifier.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 mimllearning-0.2.8/src/miml/classifier/mimlTOmi/__init__.py
--rw-r--r--   0        0        0     3059 2020-02-02 00:00:00.000000 mimllearning-0.2.8/src/miml/classifier/mimlTOmi/miml_to_mi_br_classifier.py
--rw-r--r--   0        0        0     1293 2020-02-02 00:00:00.000000 mimllearning-0.2.8/src/miml/classifier/mimlTOmi/miml_to_mi_classifier.py
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 mimllearning-0.2.8/src/miml/classifier/mimlTOml/__init__.py
--rw-r--r--   0        0        0     2366 2020-02-02 00:00:00.000000 mimllearning-0.2.8/src/miml/classifier/mimlTOml/miml_to_ml_classifier.py
--rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 mimllearning-0.2.8/src/miml/data/__init__.py
--rw-r--r--   0        0        0     2496 2020-02-02 00:00:00.000000 mimllearning-0.2.8/src/miml/data/arff_to_csv.py
--rw-r--r--   0        0        0     9086 2020-02-02 00:00:00.000000 mimllearning-0.2.8/src/miml/data/bag.py
--rw-r--r--   0        0        0     6840 2020-02-02 00:00:00.000000 mimllearning-0.2.8/src/miml/data/instance.py
--rw-r--r--   0        0        0     4896 2020-02-02 00:00:00.000000 mimllearning-0.2.8/src/miml/data/load_datasets.py
--rw-r--r--   0        0        0    15513 2020-02-02 00:00:00.000000 mimllearning-0.2.8/src/miml/data/miml_dataset.py
--rw-r--r--   0        0        0   735908 2020-02-02 00:00:00.000000 mimllearning-0.2.8/src/miml/datasets/miml_birds.arff
--rw-r--r--   0        0        0   842801 2020-02-02 00:00:00.000000 mimllearning-0.2.8/src/miml/datasets/miml_birds.csv
--rw-r--r--   0        0        0   134841 2020-02-02 00:00:00.000000 mimllearning-0.2.8/src/miml/datasets/miml_birds_random_20test.arff
--rw-r--r--   0        0        0   498562 2020-02-02 00:00:00.000000 mimllearning-0.2.8/src/miml/datasets/miml_birds_random_80train.arff
--rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 mimllearning-0.2.8/src/miml/datasets/toy.arff
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 mimllearning-0.2.8/src/miml/datasets/toy.csv
--rw-r--r--   0        0        0     2135 2020-02-02 00:00:00.000000 mimllearning-0.2.8/src/miml/test/data_test.py
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 mimllearning-0.2.8/src/miml/transformation/__init__.py
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 mimllearning-0.2.8/src/miml/transformation/mimlTOmi/__init__.py
--rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 mimllearning-0.2.8/src/miml/transformation/mimlTOmi/binary_relevance_transformation.py
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 mimllearning-0.2.8/src/miml/transformation/mimlTOml/__init__.py
--rw-r--r--   0        0        0     2057 2020-02-02 00:00:00.000000 mimllearning-0.2.8/src/miml/transformation/mimlTOml/arithmetic.py
--rw-r--r--   0        0        0     2187 2020-02-02 00:00:00.000000 mimllearning-0.2.8/src/miml/transformation/mimlTOml/geometric.py
--rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 mimllearning-0.2.8/src/miml/transformation/mimlTOml/miml_to_ml_transformation.py
--rw-r--r--   0        0        0     2168 2020-02-02 00:00:00.000000 mimllearning-0.2.8/src/miml/transformation/mimlTOml/minmax.py
--rw-r--r--   0        0        0      958 2020-02-02 00:00:00.000000 mimllearning-0.2.8/src/miml/tutorial/classifiers_tutorial.py
--rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 mimllearning-0.2.8/src/miml/tutorial/datasets_tutorial.py
--rw-r--r--   0        0        0     8579 2020-02-02 00:00:00.000000 mimllearning-0.2.8/src/miml/tutorial/demo_MIML.ipynb
--rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 mimllearning-0.2.8/src/miml/tutorial/tests.py
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 mimllearning-0.2.8/src/miml/tutorial/transformation_tutorial.py
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 mimllearning-0.2.8/.gitignore
--rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 mimllearning-0.2.8/README.md
--rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 mimllearning-0.2.8/pyproject.toml
--rw-r--r--   0        0        0     1476 2020-02-02 00:00:00.000000 mimllearning-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0     2037 2020-02-02 00:00:00.000000 mimllearning-0.2.80/readme.md
+-rw-r--r--   0        0        0   258069 2020-02-02 00:00:00.000000 mimllearning-0.2.80/documentation/AnteproyectoDamianTFG.pdf
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 mimllearning-0.2.80/src/miml/__init__.py
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 mimllearning-0.2.80/src/miml/classifier/__init__.py
+-rw-r--r--   0        0        0     2841 2020-02-02 00:00:00.000000 mimllearning-0.2.80/src/miml/classifier/miml_classifier.py
+-rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 mimllearning-0.2.80/src/miml/classifier/mi/__init__.py
+-rw-r--r--   0        0        0     3016 2020-02-02 00:00:00.000000 mimllearning-0.2.80/src/miml/classifier/mi/all_positive_apr_classifier.py
+-rw-r--r--   0        0        0     2389 2020-02-02 00:00:00.000000 mimllearning-0.2.80/src/miml/classifier/mi/apr_classifier.py
+-rw-r--r--   0        0        0     2499 2020-02-02 00:00:00.000000 mimllearning-0.2.80/src/miml/classifier/mi/miles_classifier.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 mimllearning-0.2.80/src/miml/classifier/mimlTOmi/__init__.py
+-rw-r--r--   0        0        0     3680 2020-02-02 00:00:00.000000 mimllearning-0.2.80/src/miml/classifier/mimlTOmi/miml_to_mi_br_classifier.py
+-rw-r--r--   0        0        0     2214 2020-02-02 00:00:00.000000 mimllearning-0.2.80/src/miml/classifier/mimlTOmi/miml_to_mi_classifier.py
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 mimllearning-0.2.80/src/miml/classifier/mimlTOml/__init__.py
+-rw-r--r--   0        0        0     3459 2020-02-02 00:00:00.000000 mimllearning-0.2.80/src/miml/classifier/mimlTOml/miml_to_ml_classifier.py
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 mimllearning-0.2.80/src/miml/data/__init__.py
+-rw-r--r--   0        0        0     2175 2020-02-02 00:00:00.000000 mimllearning-0.2.80/src/miml/data/arff_to_csv.py
+-rw-r--r--   0        0        0     8990 2020-02-02 00:00:00.000000 mimllearning-0.2.80/src/miml/data/bag.py
+-rw-r--r--   0        0        0     6840 2020-02-02 00:00:00.000000 mimllearning-0.2.80/src/miml/data/instance.py
+-rw-r--r--   0        0        0     4591 2020-02-02 00:00:00.000000 mimllearning-0.2.80/src/miml/data/load_datasets.py
+-rw-r--r--   0        0        0    15553 2020-02-02 00:00:00.000000 mimllearning-0.2.80/src/miml/data/miml_dataset.py
+-rw-r--r--   0        0        0   735908 2020-02-02 00:00:00.000000 mimllearning-0.2.80/src/miml/datasets/miml_birds.arff
+-rw-r--r--   0        0        0   842801 2020-02-02 00:00:00.000000 mimllearning-0.2.80/src/miml/datasets/miml_birds.csv
+-rw-r--r--   0        0        0   134841 2020-02-02 00:00:00.000000 mimllearning-0.2.80/src/miml/datasets/miml_birds_random_20test.arff
+-rw-r--r--   0        0        0   498562 2020-02-02 00:00:00.000000 mimllearning-0.2.80/src/miml/datasets/miml_birds_random_80train.arff
+-rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 mimllearning-0.2.80/src/miml/datasets/toy.arff
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 mimllearning-0.2.80/src/miml/datasets/toy.csv
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 mimllearning-0.2.80/src/miml/report/__init__.py
+-rw-r--r--   0        0        0     6438 2020-02-02 00:00:00.000000 mimllearning-0.2.80/src/miml/report/report.py
+-rw-r--r--   0        0        0     2101 2020-02-02 00:00:00.000000 mimllearning-0.2.80/src/miml/test/data_test.py
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 mimllearning-0.2.80/src/miml/transformation/__init__.py
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 mimllearning-0.2.80/src/miml/transformation/mimlTOmi/__init__.py
+-rw-r--r--   0        0        0     2304 2020-02-02 00:00:00.000000 mimllearning-0.2.80/src/miml/transformation/mimlTOmi/binary_relevance_transformation.py
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 mimllearning-0.2.80/src/miml/transformation/mimlTOml/__init__.py
+-rw-r--r--   0        0        0     2148 2020-02-02 00:00:00.000000 mimllearning-0.2.80/src/miml/transformation/mimlTOml/arithmetic.py
+-rw-r--r--   0        0        0     2367 2020-02-02 00:00:00.000000 mimllearning-0.2.80/src/miml/transformation/mimlTOml/geometric.py
+-rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 mimllearning-0.2.80/src/miml/transformation/mimlTOml/miml_to_ml_transformation.py
+-rw-r--r--   0        0        0     2826 2020-02-02 00:00:00.000000 mimllearning-0.2.80/src/miml/transformation/mimlTOml/minmax.py
+-rw-r--r--   0        0        0     9910 2020-02-02 00:00:00.000000 mimllearning-0.2.80/src/miml/tutorial/demo.ipynb
+-rw-r--r--   0        0        0    13016 2020-02-02 00:00:00.000000 mimllearning-0.2.80/src/miml/tutorial/miml_transformations.ipynb
+-rw-r--r--   0        0        0    11077 2020-02-02 00:00:00.000000 mimllearning-0.2.80/src/miml/tutorial/mimltoml_classifiers.ipynb
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 mimllearning-0.2.80/.gitignore
+-rw-r--r--   0        0        0     2037 2020-02-02 00:00:00.000000 mimllearning-0.2.80/README.md
+-rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 mimllearning-0.2.80/pyproject.toml
+-rw-r--r--   0        0        0     2387 2020-02-02 00:00:00.000000 mimllearning-0.2.80/PKG-INFO
```

### Comparing `mimllearning-0.2.8/documentation/AnteproyectoDamianTFG.pdf` & `mimllearning-0.2.80/documentation/AnteproyectoDamianTFG.pdf`

 * *Files identical despite different names*

### Comparing `mimllearning-0.2.8/src/miml/classifier/mi/all_positive_apr_classifier.py` & `mimllearning-0.2.80/src/miml/classifier/mi/all_positive_apr_classifier.py`

 * *Files 12% similar despite different names*

```diff
@@ -30,17 +30,17 @@
 
     def fit(self, x_train, y_train) -> None:
         """
         Fit the classifier to the training data.
 
         Parameters
         ----------
-        x_train : np.ndarray
+        x_train : ndarray of shape (n_bags, n_instances, n_features)
             Features values of bags in the training set.
-        y_train : np.ndarray
+        y_train : ndarray (n_bags, n_instances, n_labels)
             Labels of bags in the training set.
         """
         self.generate_apr(x_train, y_train)
 
     def predict(self, bag: np.array) -> int:
         """
         Predict the label of the bag
@@ -52,28 +52,35 @@
 
         Returns
         -------
         label: int
             Predicted label of the bag
 
         """
+        print("apr", self.apr)
         if np.all(bag >= self.apr[0]):
             if np.all(bag <= self.apr[1]):
                 return 1
         return 0
 
+    def predict_proba(self, x: np.ndarray):
+        result = np.zeros(x.shape[0])
+        for i in range(x.shape[0]):
+            result[i] = self.predict(x[i])
+        return result
+
     def generate_apr(self, x_train, y_train) -> None:
         """
         Generate the axis-parallel rectangle
 
         Parameters
         ----------
-        x_train : np.ndarray
+        x_train : np.ndarray of shape (n_bags, n_instances, n_features)
             Features values of bags in the training set.
-        y_train : np.ndarray
+        y_train : np.ndarray of shape    (n_bags, n_instances, n_features)
             Labels of bags in the training set.
         """
 
         positive_bag_indices = np.where(y_train == 1)[0]
 
         initial_bag_index = np.random.choice(positive_bag_indices)
         initial_index_instance = np.random.choice(x_train[initial_bag_index].shape[0])
```

### Comparing `mimllearning-0.2.8/src/miml/classifier/mimlTOmi/miml_to_mi_br_classifier.py` & `mimllearning-0.2.80/src/miml/classifier/miml_classifier.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,93 +1,102 @@
-import importlib
 import numpy as np
+from abc import ABC, abstractmethod
 
-from copy import deepcopy
-from sklearn.metrics import classification_report, hamming_loss
+from ..data import Bag
+from ..data import MIMLDataset
 
-from .miml_to_mi_classifier import MIMLtoMIClassifier
 
-BinaryRelevanceTransformation = importlib.import_module(
-    ".binary_relevance_transformation", package="miml.transformation.mimlTOmi").BinaryRelevanceTransformation
-Bag = importlib.import_module(".bag", package="miml.data").Bag
-MIMLDataset = importlib.import_module(".miml_dataset", package="miml.data").MIMLDataset
-
-
-class MIMLtoMIBRClassifier(MIMLtoMIClassifier):
+class MIMLClassifier(ABC):
     """
-    Class to represent a multiinstance classifier
+    Class to represent a MIMLClassifier
     """
 
-    def __init__(self, classifier) -> None:
+    def __init__(self) -> None:
+        """
+        Constructor of the class MIMLClassifier
+        """
+        self.classifier = None
+
+    def fit(self, dataset_train: MIMLDataset) -> None:
         """
-        Constructor of the class MIMLtoMIBRClassifier
+        Training the classifier
 
         Parameters
         ----------
-        classifier
-            Specific classifier to be used
+        dataset_train : MIMLDataset
+            Dataset to train the classifier
         """
-        super().__init__(classifier)
-        self.transformation = BinaryRelevanceTransformation()
-        self.classifiers = []
+        # if not isinstance(dataset_train, MIMLDataset):
+        #    raise Exception("Fit function should receive a MIMLDataset as parameter")
+
+        self.fit_internal(dataset_train)
 
+    @abstractmethod
     def fit_internal(self, dataset_train: MIMLDataset) -> None:
         """
-        Training the classifier
+        Internal method to train the classifier
 
         Parameters
         ----------
-        dataset_train: MIMLDataset
+        dataset_train : MIMLDataset
             Dataset to train the classifier
         """
-        for x in range(dataset_train.get_number_labels()):
-            classifier = deepcopy(self.classifier)
-            self.classifiers.append(classifier)
-
-        datasets = self.transformation.transform_dataset(dataset_train)
-        for i in range(len(datasets)):
-            self.classifiers[i].fit(datasets[i][0], datasets[i][1])
-
-    def predict(self, x):
-        results = np.zeros((len(self.classifiers)))
-        # Prediction of each label
-        for i in range(len(self.classifiers)):
-            results[i] = self.classifiers[i].predict(x)
-        return results
+        pass
 
-    def predict_bag(self, bag: Bag):
+    @abstractmethod
+    def predict(self, x: np.ndarray) -> np.ndarray:
         """
-        Predict labels of given data
+         Predict labels of given data
 
-        Parameters
+         Parameters
+         ----------
+         x : ndarray of shape (n, n_labels)
+             Data to predict their labels
+
+        Returns
         ----------
-        bag : Bag
-            Bag to predict their classes
+        results : ndarray of shape (n_bags, n_labels)
+            Predicted labels of data
         """
-        super().predict_bag(bag)
-        bags = self.transformation.transform_bag(bag)
-
-        return self.predict(bags[0][0])
+        # if not isinstance(x, np.ndarray):
+        #    raise Exception("Predict function should receive a Numpy array as parameter")
 
-    def evaluate(self, dataset_test: MIMLDataset):
+    @abstractmethod
+    def predict_bag(self, bag: Bag) -> np.ndarray:
         """
+        Predict labels of a given bag
 
         Parameters
         ----------
-        dataset_test: MIMLDataset
-            Dataset to test the classifier
+        bag : Bag
+            Bag to predict their labels
+
+        Returns
+        ----------
+        results : ndarray of shape (n_bags, n_labels)
+            Predicted labels of the bag
         """
-        super().evaluate(dataset_test)
+        # if not isinstance(bag, Bag):
+        #    raise Exception("Predict function should receive a Numpy array as parameter")
 
-        datasets = self.transformation.transform_dataset(dataset_test)
+    @abstractmethod
+    def predict_proba(self, dataset_test: MIMLDataset) -> np.ndarray:
+        # TODO: DOC
+        pass
 
-        results = np.zeros((dataset_test.get_number_bags(), dataset_test.get_number_labels()))
-        for i, bag in enumerate(datasets[0][0]):
-            results[i] = self.predict(bag)
+    @abstractmethod
+    def evaluate(self, dataset_test: MIMLDataset) -> np.ndarray:
+        """
+        Evaluate the model on a test dataset
 
-        print(classification_report(dataset_test.get_labels_by_bag(), results, zero_division=0))
-        print("Hamming Loss: ", hamming_loss(dataset_test.get_labels_by_bag(), results))
+        Parameters
+        ----------
+        dataset_test : MIMLDataset
+            Test dataset to evaluate the model on.
 
-        # TODO: To Csv file
-        # report = classification_report(y_test, y_pred, output_dict=True)
-        # df = pandas.DataFrame(report).transpose()
-        # df.to_csv
+        Returns
+        ----------
+        results : ndarray of shape (n_bags, n_labels)
+            Predicted labels of dataset_test
+        """
+        # if not isinstance(dataset_test, MIMLDataset):
+        #    raise Exception("Evaluate function should receive a MIMLDataset as parameter")
```

### Comparing `mimllearning-0.2.8/src/miml/classifier/mimlTOml/miml_to_ml_classifier.py` & `mimllearning-0.2.80/src/miml/transformation/mimlTOmi/binary_relevance_transformation.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,73 +1,71 @@
-import importlib
 import numpy as np
+from copy import deepcopy
+from ...data import Bag
+from ...data import MIMLDataset
 
-from sklearn.metrics import classification_report, hamming_loss
-from ..miml_classifier import MIMLClassifier
 
-MIMLtoMLTransformation = importlib.import_module(".miml_to_ml_transformation", package="miml.transformation.mimlTOml")
-Bag = importlib.import_module(".bag", package="miml.data").Bag
-MIMLDataset = importlib.import_module(".miml_dataset", package="miml.data").MIMLDataset
+class BinaryRelevanceTransformation:
+    """
+    Class that performs a binary relevance transformation to convert a MIMLDataset class to numpy ndarrays.
+    """
 
+    def __init__(self):
+        self.dataset = None
 
-class MIMLtoMLClassifier(MIMLClassifier):
-
-    def __init__(self, ml_classifier, transformation: MIMLtoMLTransformation) -> None:
+    def transform_dataset(self, dataset: MIMLDataset) -> list:
         """
-        Constructor of the class MIMLtoMIClassifier
+        Transform the dataset to multiinstance datasets dividing the original dataset into n datasets with a single
+        label, where n is the number of labels.
 
-        Parameters
-        ----------
-        ml_classifier
-            Specific classifier to be used
+        Returns
+        -------
 
-        transformation : MIMLtoMLTransformation
-            Transformation to be used
-        """
-        super().__init__()
-        self.classifier = ml_classifier
-        self.transformation = transformation
+        datasets: list
+            Multi instance datasets
 
-    def fit_internal(self, dataset_train: MIMLDataset) -> None:
         """
+        self.dataset = dataset
+        datasets = []
+        for i in range(self.dataset.get_number_labels()):
+            dataset = deepcopy(self.dataset)
+            count = 0
+            for j in range(self.dataset.get_number_labels()):
+                if i != j:
+                    dataset.delete_attribute(self.dataset.get_number_features()-count+j)
+                    labels_name = dataset.get_labels_name()
+                    labels_name.pop(j-count)
+                    dataset.set_labels_name(labels_name)
+                    count += 1
+            datasets.append(dataset)
 
-        Parameters
-        ----------
-        dataset_train
-        """
-        x_train, y_train = self.transformation.transform_dataset(dataset_train)
-        self.classifier.fit(x_train, y_train)
+        return datasets
 
-    def predict(self, x: np.ndarray):
-        return self.classifier.predict(x)
-
-    def predict_bag(self, bag: Bag) -> np.ndarray:
+    def transform_bag(self, bag: Bag) -> list:
         """
+        Transform miml bag to multi instance bags
 
         Parameters
         ----------
-        bag
-        """
-        # TODO: Check number attributes of bag with dataset
-        super().predict_bag(bag)
-        x_bag, _ = self.transformation.transform_bag(bag)
-        x_bag = np.array(x_bag, ndmin=2)
-        return self.predict(x_bag)
+        bag :
+            Bag to be transformed to multiinstance bag
 
-    def evaluate(self, dataset_test: MIMLDataset):
-        """
+        Returns
+        -------
+        bags : list[Bag]
+            List of n_labels transformed bags
+
+        """
+        bags = []
+        for i in range(bag.get_number_labels()):
+            transformed_bag = deepcopy(bag)
+            count = 0
+            for j in range(bag.get_number_labels()):
+                if i != j:
+                    transformed_bag.data = np.delete(transformed_bag.data, bag.get_number_features() - count + j, axis=1)
+                    labels_name = transformed_bag.dataset.get_labels_name()
+                    labels_name.pop(j - count)
+                    transformed_bag.dataset.set_labels_name(labels_name)
+                    count += 1
+            bags.append(transformed_bag)
 
-        Parameters
-        ----------
-        dataset_test
-        """
-        super().evaluate(dataset_test)
-        x_test, y_test = self.transformation.transform_dataset(dataset_test)
-        results = self.predict(x_test)
-
-        print(classification_report(dataset_test.get_labels_by_bag(), results, zero_division=0))
-        print("Hamming Loss: ", hamming_loss(dataset_test.get_labels_by_bag(), results))
-
-        # TODO: To Csv file
-        # report = classification_report(y_test, y_pred, output_dict=True)
-        # df = pandas.DataFrame(report).transpose()
-        # df.to_csv
+        return bags
```

### Comparing `mimllearning-0.2.8/src/miml/data/arff_to_csv.py` & `mimllearning-0.2.80/src/miml/data/arff_to_csv.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,40 +5,34 @@
     Parameters
     ----------
     file : str
         Filepath of the file to be converted
 
     delimiter : str, default = '
         Delimiter used in arff file for the start and end of the bag values ( ' or " )
-
     """
 
     arff = open(file)
     csv = open(file[:-5] + ".csv", "w")
     attrib = []
     flag = 0
 
     for line in arff:
         # Comprobamos que la cadena no contenga espacios en blanco a la izquierda ni que sea vacía
         line = line.lstrip()
         if line == "":
             continue
 
         if line.startswith("%") or line.startswith("@"):
-            if line.startswith("@attribute"):
-                if not (line.startswith("@attribute bag relational")):
-                    attrib.append(line[line.find(" ") + 1:line.find(" ", line.find(" ") + 1)])
+            if line.startswith("@attribute") and not line.startswith("@attribute bag relational"):
+                attrib.append(line.split()[1])
 
         else:
             if flag == 0:
-                for x in range(len(attrib)):
-                    if x == len(attrib) - 1:
-                        csv.write(attrib[x] + "\n")
-                    else:
-                        csv.write(attrib[x] + ",")
+                csv.write(','.join(attrib) + '\n')
                 flag = 1
 
             # Eliminanos el salto de línea del final de la cadena
             line = line.strip("\n")
 
             # Asumimos que el primer elemento de cada instancia es el identificador de la bolsa
             key = line[0:line.find(",")]
@@ -53,14 +47,13 @@
 
             # El resto de la cadena se trata de las etiquetas
             labels = line[line.find(delimiter, line.find(delimiter, line.find(delimiter))) + 2:]
             # print("Labels: ", labels)
 
             for v in values:
                 csv.write(key + "," + v + "," + labels + "\n")
-                # TODO: quizas separar en funciones para data y para atributos
                 # TODO: intentar optimizar la funcion, aprovechar que la string del arff
                 # es parecida, separar solo los values
                 # TODO: control de errores
 
     arff.close()
     csv.close()
```

### Comparing `mimllearning-0.2.8/src/miml/data/bag.py` & `mimllearning-0.2.80/src/miml/data/bag.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,14 @@
         Constructor of the class Bag
 
         Parameters
         ----------
         key : str
             Key of the bag
         """
-        # TODO: Ver si quitar instance del constructor, se puede poner como parametro opcional
         self.data = None
         self.key = key
         self.dataset = None
 
     def get_attributes_name(self) -> list[str]:
         """
         Get attributes name of the bag
```

### Comparing `mimllearning-0.2.8/src/miml/data/instance.py` & `mimllearning-0.2.80/src/miml/data/instance.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.2.8/src/miml/data/load_datasets.py` & `mimllearning-0.2.80/src/miml/data/load_datasets.py`

 * *Files 5% similar despite different names*

```diff
@@ -41,22 +41,18 @@
         Path of the dataset file
 
     Returns
     -------
     dataset : MIMLDataset
         Dataset loaded
     """
-    # dataset = pd.read_csv(file, header=0)
-    # TODO: Hay que ver como diferenciar los atributos de las labels
-    # TODO: Si no se puede implementar la funcionalidad de pandas "[]"
-    # TODO: y poner atributos y labels como parametros opcionales quizas
 
     dataset = MIMLDataset()
     csv_file = open(file)
-
+    dataset.set_name(file.split("/")[-1])
     file_name = os.path.basename(file)
     dataset.set_name(os.path.splitext(file_name)[0])
 
     # TODO: Hacer que se pueda pasar por parametro
     num_labels = int(csv_file.readline().replace("\n", ""))
 
     header_line = csv_file.readline().replace("\n", "").split(",")
@@ -67,17 +63,16 @@
 
     for line in csv_file:
 
         data = line.split(",")
 
         key = data[0]
 
-        # TODO: Revisar porque values tiene el ndmin=2
-        values = np.array([float(i) for i in data[1:-num_labels]], ndmin=2)
-        labels = np.array([int(i) for i in data[-num_labels:]])
+        values = [float(i) for i in data[1:-num_labels]]
+        labels = [int(i) for i in data[-num_labels:]]
 
         instance = Instance(values + labels)
 
         if key not in dataset.data:
             bag = Bag(key)
             dataset.add_bag(bag)
         dataset.add_instance(key, instance)
```

### Comparing `mimllearning-0.2.8/src/miml/data/miml_dataset.py` & `mimllearning-0.2.80/src/miml/data/miml_dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,14 @@
     Class to manage MIML data obtained from datasets
     """
 
     def __init__(self) -> None:
         """
         Constructor of the class MIMLDataset
         """
-        # TODO: Si dataset leido en csv, el nombre poner el del archivo
         self.name = "undefined"
         self.attributes = dict()
         self.data = dict()
 
     def set_name(self, name) -> None:
         """
         Set function for dataset name
@@ -53,19 +52,18 @@
 
     def get_attributes(self) -> np.ndarray:
         """
         Get attributes values of the dataset
 
         Returns
         -------
-        attributes data: numpy array
+        attributes data: ndarray of shape (n_instances, n_attributes)
             Values of the attributes of the dataset
         """
-        pass
-        # TODO: Ver si es necesario
+        return np.hstack((self.get_features(), self.get_labels()))
 
     def get_number_attributes(self) -> int:
         """
         Get numbers of attributes of the bag
 
         Returns
         ----------
@@ -107,27 +105,27 @@
 
     def get_features(self) -> np.ndarray:
         """
         Get features values of the dataset
 
         Returns
         -------
-        features: numpy array
+        features: ndarray of shape (n_instances, n_features)
             Values of the features of the dataset
         """
-        # TODO: Test
         features = np.zeros((self.get_number_instances(), self.get_number_features()))
         count = 0
         for key in self.data.keys():
             for instance in self.get_bag(key).get_features():
                 features[count] = instance
                 count += 1
         return features
 
     def get_features_by_bag(self) -> np.ndarray:
+        # TODO: Doc
         features = []
         for key in self.data.keys():
             features.append(self.get_bag(key).get_features())
         return np.array(features, dtype=object)
 
     def get_number_features(self) -> int:
         """
@@ -276,15 +274,14 @@
             Index of the instance in the bag
 
         Returns
         -------
         instance : Instance
             Instance of Instance class
         """
-        # TODO: check
         return self.get_bag(key_bag).get_instance(index_instance)
 
     def get_number_instances(self) -> int:
         """
         Get numbers of instances of the dataset
 
         Returns
@@ -298,14 +295,15 @@
         """
         Add an Instance to a Bag of the dataset
 
         Parameters
         ----------
         key : str
             Key of the bag where the instance will be added
+
         instance : Instance
             Instance of Instance class to be added
         """
         self.get_bag(key).add_instance(instance)
 
     def delete_instance(self, key_bag: str, index_instance: int) -> None:
         """
@@ -368,59 +366,62 @@
         Add attribute to the dataset
 
         Parameters
         ----------
         position : int
             Index for the new attribute
 
-        values:  numpy array
+        values:  ndarray of shape(n_instances)
             Values for the new attribute
         """
         # TODO: Test
         for bag_index, bag in enumerate(self.data.keys()):
             add_values = values[bag_index]
             if values is None:
-                add_values = np.zeros(self.data[bag].get_number_instances)
+                add_values = np.zeros(self.data[bag].get_number_instances())
             self.data[bag].add_attribute(position, add_values)
 
     def delete_attribute(self, position: int) -> None:
 
         """
         Delete attribute of the dataset
 
         Parameters
         ----------
         position : int
             Index of the attribute to be deleted
         """
-
         for bag in self.data.keys():
-            self.data[bag].delete_attribute(position)
+            self.data[bag].data = np.delete(self.data[bag].data, position, axis=1)
 
-    def show_dataset(self, head: int = None, attributes=None, labels=None) -> None:
+    def show_dataset(self, head: int = None, attributes=None, labels=None, info=True) -> None:
         """
         Function to show information about the dataset
 
         Parameters
         ----------
             head : int
                 Number of the nth firsts bag to show
 
             attributes: List of string
                 Attributes to show
 
             labels : List of string
                 Labels to show
+
+            info: Boolean
+                Show more info
         """
         # TODO: Hacer algo como head y tail de pandas, ponerlo como parametro quizas, tambien lista atributos y labels
         #  a mostrar opcionales
-        print("Name: ", self.get_name())
-        print("Features: ", self.get_features_name())
-        print("Labels: ", self.get_labels_name())
-        print("Bags:")
+        if info:
+            print("Name: ", self.get_name())
+            print("Features: ", self.get_features_name())
+            print("Labels: ", self.get_labels_name())
+            print("Bags:")
         count = 0
         for key in self.data:
             # print("\n")
             bag = self.get_bag(key)
             # print("Key: ", key_bag)
             # print("Attributes: ", bag[0])
             # print("Labels: ", bag[1])
@@ -486,42 +487,38 @@
             Number of instances in the bag with maximum number of instances
 
         distribution : dict
             Distribution of number of instances in bags
         """
         n_instances = self.get_number_instances()
         max_instances = 0
-        # TODO: check
         min_instances = float("inf")
         distribution = dict()
         for key in self.data:
             instances_bag = self.get_bag(key).get_number_instances()
             if instances_bag in distribution:
                 distribution[instances_bag] += 1
             else:
                 distribution[instances_bag] = 1
             if instances_bag < min_instances:
                 min_instances = instances_bag
-            elif instances_bag > max_instances:
+            if instances_bag > max_instances:
                 max_instances = instances_bag
         return n_instances, min_instances, max_instances, distribution
 
     def describe(self):
         """
         Print statistics about the dataset
         """
 
-        # TODO: Ponerlo bonito con tabulate
-
         print("-----MULTILABEL-----")
         print("Cardinalidad: ", self.cardinality())
         print("Densidad: ", self.density())
         print("Distinct: ", self.distinct())
         print("")
-        # TODO: Testearlo
         n_instances, min_instances, max_instances, distribution = self.get_statistics()
         print("-----MULTIINSTANCE-----")
         print("Nº of bags: ", self.get_number_bags())
         print("Total instances: ", n_instances)
         print("Average Instances per bag: ", n_instances / self.get_number_bags())
         print("Min Instances per bag: ", min_instances)
         print("Max Instances per bag: ", max_instances)
```

### Comparing `mimllearning-0.2.8/src/miml/datasets/miml_birds.arff` & `mimllearning-0.2.80/src/miml/datasets/miml_birds.arff`

 * *Files identical despite different names*

### Comparing `mimllearning-0.2.8/src/miml/datasets/miml_birds.csv` & `mimllearning-0.2.80/src/miml/datasets/miml_birds.csv`

 * *Files identical despite different names*

### Comparing `mimllearning-0.2.8/src/miml/datasets/miml_birds_random_20test.arff` & `mimllearning-0.2.80/src/miml/datasets/miml_birds_random_20test.arff`

 * *Files identical despite different names*

### Comparing `mimllearning-0.2.8/src/miml/datasets/miml_birds_random_80train.arff` & `mimllearning-0.2.80/src/miml/datasets/miml_birds_random_80train.arff`

 * *Files identical despite different names*

### Comparing `mimllearning-0.2.8/src/miml/test/data_test.py` & `mimllearning-0.2.80/src/miml/test/data_test.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,15 +17,14 @@
         instance.set_attribute(4, 1)
         self.assertEqual(list(instance.get_attributes()), [2, 0.8, 5.09, 1, 1])
         with self.assertRaises(Exception) as error:
             instance.get_number_features()
         self.assertEqual(error.exception.args[0], "The instance isn't in any dataset, so there is no features info")
 
     def test_bag(self):
-        # TODO:
         values = [2, 7, 5.09, 1, 0]
         instance = Instance(values)
         bag = Bag("1")
         bag.add_instance(instance)
         self.assertEqual(bag.get_number_instances(), 1)
         self.assertEqual(list(bag.get_instance(0).get_attributes()), list(instance.get_attributes()))
         self.assertEqual(bag.get_number_attributes(), 5)
@@ -34,15 +33,14 @@
         # bag.add_instance(instance)
 
     def test_mimldataset(self):
         # TODO:
         pass
 
     def test_final(self):
-        # TODO:
         values = [2, 7, 5.09, 1, 0]
         instance1 = Instance(values)
         instance2 = Instance(values)
         bag = Bag("bag1")
         bag.add_instance(instance1)
         bag.add_instance(instance2)
```

### Comparing `mimllearning-0.2.8/src/miml/transformation/mimlTOmi/binary_relevance_transformation.py` & `mimllearning-0.2.80/src/miml/transformation/mimlTOml/geometric.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,52 +1,70 @@
-import importlib
 
-Bag = importlib.import_module(".bag", package="miml.data").Bag
-MIMLDataset = importlib.import_module(".miml_dataset", package="miml.data").MIMLDataset
+import numpy as np
 
+from .miml_to_ml_transformation import MIMLtoMLTransformation
+from ...data import Instance
+from ...data import Bag
+from ...data import MIMLDataset
 
-class BinaryRelevanceTransformation:
+
+class GeometricTransformation(MIMLtoMLTransformation):
     """
-    Class that performs a binary relevance transformation to convert a MIMLDataset class to numpy ndarrays.
+    Class that performs a geometric transformation to convert a MIMLDataset class to numpy ndarrays.
     """
 
     def __init__(self):
-        self.dataset = None
+        super().__init__()
 
-    def transform_dataset(self, dataset: MIMLDataset) -> list:
+    def transform_dataset(self, dataset: MIMLDataset) -> MIMLDataset:
         """
-        Transform the dataset to multiinstance datasets dividing the original dataset into n datasets with a single
-        label, where n is the number of labels.
+        Transform the dataset to multilabel dataset converting each bag into a single instance being the value of each
+        attribute the geometric center of the instances in the bag.
 
         Returns
         -------
-
-        datasets: list
-            Multi instance datasets
-
         """
         self.dataset = dataset
-        datasets = []
-        x = self.dataset.get_features_by_bag()
-        y = self.dataset.get_labels_by_bag()
-        for i in range(self.dataset.get_number_labels()):
-            datasets.append([x, y[:, i].reshape(-1, 1)])
+        transformed_dataset = MIMLDataset()
+        transformed_dataset.set_name(dataset.get_name())
+        transformed_dataset.set_features_name(dataset.get_features_name())
+        transformed_dataset.set_labels_name(dataset.get_labels_name())
+        for bag_index, key in enumerate(self.dataset.data.keys()):
+            transformed_bag = self.transform_bag(self.dataset.get_bag(key))
+            transformed_dataset.add_bag(transformed_bag)
 
-        return datasets
+        return transformed_dataset
 
-    def transform_bag(self, bag: Bag) -> list:
+    def transform_bag(self, bag: Bag) -> Bag:
         """
-        Transform miml bag to multi instance bags
+        Transform a bag to a multilabel instance
 
         Parameters
         ----------
-        bag :
-            Bag to be transformed to multiinstance bag
+        bag : Bag
+            Bag to be transformed to multilabel instance
 
         Returns
         -------
-        bags : list[ndarray]
-        Tuple of numpy ndarray with attribute values and labels
+        features : ndarray of shape (n_features)
+            Numpy array with feature values
 
+        labels : ndarray of shape (n_labels)
+            Numpy array with label values
         """
-        bags = [[bag.get_features(), label] for label in bag.get_labels()[0]]
-        return bags
+
+        features = bag.get_features()
+        labels = bag.get_labels()[0]
+        min_values = np.min(features, axis=0)
+        max_values = np.max(features, axis=0)
+        features = (min_values + max_values) / 2
+
+        transformed_bag = Bag(bag.key)
+        transformed_bag.add_instance(Instance(list(np.hstack((features, labels)))))
+
+        dataset = MIMLDataset()
+        dataset.set_name(bag.dataset.get_name())
+        dataset.set_features_name(bag.dataset.get_features_name())
+        dataset.set_labels_name(bag.dataset.get_labels_name())
+        dataset.add_bag(transformed_bag)
+
+        return transformed_bag
```

### Comparing `mimllearning-0.2.8/pyproject.toml` & `mimllearning-0.2.80/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,20 +2,20 @@
 requires = ["hatchling", "pkginfo >= 1.10"]
 build-backend = "hatchling.build"
 
 [tool.hatch.build.targets.wheel]
 packages = ["src/miml", "src/miml/*"]
 
 [metadata]
-version = "0.2.8"
+version = "0.2.80"
 name = "mimllearning"
 
 [project]
 name = "mimllearning"
-version = "0.2.8"
+version = "0.2.80"
 authors = [
   { name="Damian Martinez", email="damianmartinezavila@gmail.com" },
 ]
 description = "MIML Learning Library"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `mimllearning-0.2.8/PKG-INFO` & `mimllearning-0.2.80/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: mimllearning
-Version: 0.2.8
+Version: 0.2.80
 Summary: MIML Learning Library
 Project-URL: Homepage, https://github.com/p82maavd/miml
 Author-email: Damian Martinez <damianmartinezavila@gmail.com>
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
@@ -12,14 +12,15 @@
 
 # miml: Multi Instance Multi Label Learning Library for Python
 The aim of the library is to ease the development, testing and comparison of classification algorithms for multi-instance multi-label learning (MIML). 
 
 ## Table of Contents
 
 - [Installation](#installation)
+- [Usage](#usage)
 - [License](#license)
 
 ### Installation
 
 Use the package manager [pip](https://pip.pypa.io/en/stable/) to install miml.
 
 ```bash
@@ -33,10 +34,46 @@
     $ pip install numpy
     $ pip install scikit-learn
     $ pip install scipy
     $ pip install mil
     $ pip install tensorflow
     $ pip install keras==2.12.0
 
+### Usage
+
+
+#### Datasets
+
+``` python
+import pkg_resources
+from miml.data.load_datasets import load_dataset
+
+dataset_train = load_dataset(pkg_resources.resource_filename('miml', 'datasets/miml_birds_random_80train.arff'),
+                             delimiter="'")
+dataset_test = load_dataset(pkg_resources.resource_filename('miml', 'datasets/miml_birds_random_20test.arff'),
+                            delimiter="'")
+```
+
+#### Classifier
+
+``` python
+from miml.classifier import MIMLtoMIBRClassifier, AllPositiveAPRClassifier
+
+classifier_mi = MIMLtoMIBRClassifier(AllPositiveAPRClassifier())
+classifier_mi.fit(dataset_train)
+results_mi=classifier_mi.evaluate(dataset_test)
+```
+
+#### Report
+
+``` python
+from miml.report import Report
+
+report = Report()
+report.to_string(dataset_test.get_labels_by_bag(), results_ml)
+print("")
+report.to_csv(dataset_test.get_labels_by_bag(), results_ml)
+```
+
 ### License
 [![License](http://img.shields.io/:license-mit-blue.svg?style=flat-square)](http://badges.mit-license.org)
 - **[MIT license](http://opensource.org/licenses/mit-license.php)**
```

