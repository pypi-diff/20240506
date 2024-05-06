# Comparing `tmp/mnists-0.1.0.tar.gz` & `tmp/mnists-0.2.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mnists-0.1.0.tar", last modified: Fri May  3 23:00:47 2024, max compression
+gzip compressed data, was "mnists-0.2.0rc1.tar", last modified: Mon May  6 10:56:35 2024, max compression
```

## Comparing `mnists-0.1.0.tar` & `mnists-0.2.0rc1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 pczarnik (4214435) pczarnik (4214435)        0 2024-05-03 23:00:47.766895 mnists-0.1.0/
--rw-r--r--   0 pczarnik (4214435) pczarnik (4214435)     1070 2024-05-03 18:18:09.000000 mnists-0.1.0/LICENSE
--rw-r--r--   0 pczarnik (4214435) pczarnik (4214435)     2970 2024-05-03 23:00:47.766895 mnists-0.1.0/PKG-INFO
--rw-r--r--   0 pczarnik (4214435) pczarnik (4214435)     2136 2024-05-03 22:49:59.000000 mnists-0.1.0/README.md
-drwxr-xr-x   0 pczarnik (4214435) pczarnik (4214435)        0 2024-05-03 23:00:47.764895 mnists-0.1.0/mnists/
--rw-r--r--   0 pczarnik (4214435) pczarnik (4214435)      109 2024-05-03 22:52:34.000000 mnists-0.1.0/mnists/__init__.py
--rw-r--r--   0 pczarnik (4214435) pczarnik (4214435)     7701 2024-05-03 18:18:09.000000 mnists-0.1.0/mnists/_mnist.py
--rw-r--r--   0 pczarnik (4214435) pczarnik (4214435)     2594 2024-05-03 18:18:09.000000 mnists-0.1.0/mnists/utils.py
-drwxr-xr-x   0 pczarnik (4214435) pczarnik (4214435)        0 2024-05-03 23:00:47.765895 mnists-0.1.0/mnists.egg-info/
--rw-r--r--   0 pczarnik (4214435) pczarnik (4214435)     2970 2024-05-03 23:00:47.000000 mnists-0.1.0/mnists.egg-info/PKG-INFO
--rw-r--r--   0 pczarnik (4214435) pczarnik (4214435)      233 2024-05-03 23:00:47.000000 mnists-0.1.0/mnists.egg-info/SOURCES.txt
--rw-r--r--   0 pczarnik (4214435) pczarnik (4214435)        1 2024-05-03 23:00:47.000000 mnists-0.1.0/mnists.egg-info/dependency_links.txt
--rw-r--r--   0 pczarnik (4214435) pczarnik (4214435)       98 2024-05-03 23:00:47.000000 mnists-0.1.0/mnists.egg-info/requires.txt
--rw-r--r--   0 pczarnik (4214435) pczarnik (4214435)        7 2024-05-03 23:00:47.000000 mnists-0.1.0/mnists.egg-info/top_level.txt
--rw-r--r--   0 pczarnik (4214435) pczarnik (4214435)      999 2024-05-03 21:57:43.000000 mnists-0.1.0/pyproject.toml
--rw-r--r--   0 pczarnik (4214435) pczarnik (4214435)       38 2024-05-03 23:00:47.766895 mnists-0.1.0/setup.cfg
+drwxr-xr-x   0 pczarnik (4214435) pczarnik (4214435)        0 2024-05-06 10:56:35.389177 mnists-0.2.0rc1/
+-rw-r--r--   0 pczarnik (4214435) pczarnik (4214435)     1070 2024-05-03 18:18:09.000000 mnists-0.2.0rc1/LICENSE
+-rw-r--r--   0 pczarnik (4214435) pczarnik (4214435)     2995 2024-05-06 10:56:35.388177 mnists-0.2.0rc1/PKG-INFO
+-rw-r--r--   0 pczarnik (4214435) pczarnik (4214435)     2158 2024-05-06 10:29:42.000000 mnists-0.2.0rc1/README.md
+drwxr-xr-x   0 pczarnik (4214435) pczarnik (4214435)        0 2024-05-06 10:56:35.386177 mnists-0.2.0rc1/mnists/
+-rw-r--r--   0 pczarnik (4214435) pczarnik (4214435)      112 2024-05-06 10:55:35.000000 mnists-0.2.0rc1/mnists/__init__.py
+-rw-r--r--   0 pczarnik (4214435) pczarnik (4214435)     8410 2024-05-06 10:53:51.000000 mnists-0.2.0rc1/mnists/_mnist.py
+-rw-r--r--   0 pczarnik (4214435) pczarnik (4214435)     2594 2024-05-03 18:18:09.000000 mnists-0.2.0rc1/mnists/utils.py
+drwxr-xr-x   0 pczarnik (4214435) pczarnik (4214435)        0 2024-05-06 10:56:35.387177 mnists-0.2.0rc1/mnists.egg-info/
+-rw-r--r--   0 pczarnik (4214435) pczarnik (4214435)     2995 2024-05-06 10:56:35.000000 mnists-0.2.0rc1/mnists.egg-info/PKG-INFO
+-rw-r--r--   0 pczarnik (4214435) pczarnik (4214435)      233 2024-05-06 10:56:35.000000 mnists-0.2.0rc1/mnists.egg-info/SOURCES.txt
+-rw-r--r--   0 pczarnik (4214435) pczarnik (4214435)        1 2024-05-06 10:56:35.000000 mnists-0.2.0rc1/mnists.egg-info/dependency_links.txt
+-rw-r--r--   0 pczarnik (4214435) pczarnik (4214435)       98 2024-05-06 10:56:35.000000 mnists-0.2.0rc1/mnists.egg-info/requires.txt
+-rw-r--r--   0 pczarnik (4214435) pczarnik (4214435)        7 2024-05-06 10:56:35.000000 mnists-0.2.0rc1/mnists.egg-info/top_level.txt
+-rw-r--r--   0 pczarnik (4214435) pczarnik (4214435)      999 2024-05-03 21:57:43.000000 mnists-0.2.0rc1/pyproject.toml
+-rw-r--r--   0 pczarnik (4214435) pczarnik (4214435)       38 2024-05-06 10:56:35.389177 mnists-0.2.0rc1/setup.cfg
```

### Comparing `mnists-0.1.0/LICENSE` & `mnists-0.2.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `mnists-0.1.0/PKG-INFO` & `mnists-0.2.0rc1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mnists
-Version: 0.1.0
+Version: 0.2.0rc1
 Summary: MNISTs: All MNIST-like datasets in one package
 Author-email: Piotr Czarnik <ptr.czarnik@gmail.com>
 Project-URL: Homepage, https://github.com/pczarnik/mnists
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
@@ -31,55 +31,55 @@
 
 Each dataset stores train/test images as numpy arrays of shape `(n_samples, img_height, img_width)` and train/test labels as numpy arrays of shape `(n_samples,)`.
 
 MNIST example:
 ```python
 >>> from mnists import MNIST
 >>> mnist = MNIST()
->>> type(mnist.train_images)
+>>> type(mnist.train_images())
 <class 'numpy.ndarray'>
->>> mnist.train_images.dtype
+>>> mnist.train_images().dtype
 dtype('uint8')
->>> mnist.train_images.min()
+>>> mnist.train_images().min()
 0
->>> mnist.train_images.max()
+>>> mnist.train_images().max()
 255
->>> mnist.train_images.shape
+>>> mnist.train_images().shape
 (60000, 28, 28)
->>> mnist.train_labels.shape
+>>> mnist.train_labels().shape
 (60000,)
->>> mnist.test_images.shape
+>>> mnist.test_images().shape
 (10000, 28, 28)
->>> mnist.test_labels.shape
+>>> mnist.test_labels().shape
 (10000,)
 >>> mnist.classes[:3]
 ['0 - zero', '1 - one', '2 - two']
 ```
 
 FashionMNIST example:
 ```python
 from mnists import FashionMNIST
 import matplotlib.pyplot as plt
 
 fmnist = FashionMNIST()
-plt.imshow(fmnist.train_images[0], cmap='gray')
-plt.title(fmnist.classes[fmnist.train_labels[0]])
+plt.imshow(fmnist.train_images()[0], cmap='gray')
+plt.title(fmnist.classes[fmnist.train_labels()[0]])
 plt.axis('off')
 plt.show()
 ```
 ![FashionMNIST example](https://raw.githubusercontent.com/pczarnik/mnists/main/imgs/fmnist_boot.png)
 
 KMNIST example:
 ```python
 from mnists import KMNIST
 import matplotlib.pyplot as plt
 
 kmnist = KMNIST()
 plt.imshow(
-    kmnist.test_images[:256]
+    kmnist.test_images()[:256]
         .reshape(16, 16, 28, 28)
         .swapaxes(1, 2)
         .reshape(16 * 28, -1),
     cmap='gray')
 plt.axis('off')
 plt.show()
 ```
```

### Comparing `mnists-0.1.0/README.md` & `mnists-0.2.0rc1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -10,55 +10,55 @@
 
 Each dataset stores train/test images as numpy arrays of shape `(n_samples, img_height, img_width)` and train/test labels as numpy arrays of shape `(n_samples,)`.
 
 MNIST example:
 ```python
 >>> from mnists import MNIST
 >>> mnist = MNIST()
->>> type(mnist.train_images)
+>>> type(mnist.train_images())
 <class 'numpy.ndarray'>
->>> mnist.train_images.dtype
+>>> mnist.train_images().dtype
 dtype('uint8')
->>> mnist.train_images.min()
+>>> mnist.train_images().min()
 0
->>> mnist.train_images.max()
+>>> mnist.train_images().max()
 255
->>> mnist.train_images.shape
+>>> mnist.train_images().shape
 (60000, 28, 28)
->>> mnist.train_labels.shape
+>>> mnist.train_labels().shape
 (60000,)
->>> mnist.test_images.shape
+>>> mnist.test_images().shape
 (10000, 28, 28)
->>> mnist.test_labels.shape
+>>> mnist.test_labels().shape
 (10000,)
 >>> mnist.classes[:3]
 ['0 - zero', '1 - one', '2 - two']
 ```
 
 FashionMNIST example:
 ```python
 from mnists import FashionMNIST
 import matplotlib.pyplot as plt
 
 fmnist = FashionMNIST()
-plt.imshow(fmnist.train_images[0], cmap='gray')
-plt.title(fmnist.classes[fmnist.train_labels[0]])
+plt.imshow(fmnist.train_images()[0], cmap='gray')
+plt.title(fmnist.classes[fmnist.train_labels()[0]])
 plt.axis('off')
 plt.show()
 ```
 ![FashionMNIST example](https://raw.githubusercontent.com/pczarnik/mnists/main/imgs/fmnist_boot.png)
 
 KMNIST example:
 ```python
 from mnists import KMNIST
 import matplotlib.pyplot as plt
 
 kmnist = KMNIST()
 plt.imshow(
-    kmnist.test_images[:256]
+    kmnist.test_images()[:256]
         .reshape(16, 16, 28, 28)
         .swapaxes(1, 2)
         .reshape(16 * 28, -1),
     cmap='gray')
 plt.axis('off')
 plt.show()
 ```
```

### Comparing `mnists-0.1.0/mnists/_mnist.py` & `mnists-0.2.0rc1/mnists/_mnist.py`

 * *Files 20% similar despite different names*

```diff
@@ -17,17 +17,19 @@
     MNIST Dataset
     http://yann.lecun.com/exdb/mnist
 
     Attributes
     ----------
     target_dir : str
         Directory where all files exist or will be downloaded.
-    train_images, train_labels, test_images, test_labels : np.ndarray, optional
+    _train_images, _train_labels, _test_images, _test_labels : np.ndarray, optional
         Numpy array representation of train/test images/labels from MNIST dataset.
         May be None if wasn't loaded manually or during initialization.
+        If is not None, corresponding getter, e.g., _train_images -> train_images(),
+        will be available.
     classes : list[str]
         Class names.
     mirrors : list[str]
         List of urls where dataset is hosted.
     resources : dict[str, tuple[str, str]]
        Dictionary of data files with filename and md5 hash.
     """
@@ -89,18 +91,18 @@
             If True, downloads all files to `target_dir`, even if they exist there.
         load : bool, default=True
             If True, loads data from files in `target_dir`.
         """
 
         self.target_dir = self.default_dir if target_dir is None else target_dir
 
-        self.train_images: Optional[np.ndarray] = None
-        self.train_labels: Optional[np.ndarray] = None
-        self.test_images: Optional[np.ndarray] = None
-        self.test_labels: Optional[np.ndarray] = None
+        self._train_images: Optional[np.ndarray] = None
+        self._train_labels: Optional[np.ndarray] = None
+        self._test_images: Optional[np.ndarray] = None
+        self._test_labels: Optional[np.ndarray] = None
 
         if download or force_download:
             self.download(force_download)
 
         if load:
             self.load()
 
@@ -130,19 +132,30 @@
         """
 
         for key, (filename, md5) in self.resources.items():
             filepath = os.path.join(self.target_dir, filename)
 
             if not check_file_integrity(filepath, md5):
                 raise RuntimeError(
-                    "Dataset not found. Use download=True or mnist.download() to download it"
+                    f"Dataset '{key}' not found in '{filepath}' or MD5 "
+                    "checksum is not valid. "
+                    "Use download=True or .download() to download it"
                 )
 
             data = read_idx_file(filepath)
-            setattr(self, key, data)
+            self._add_getter(key, data)
+
+    def _add_getter(self, fn_name: str, data: np.ndarray) -> None:
+        var_name = f"_{fn_name}"
+        setattr(self, var_name, data)
+
+        def getter() -> np.ndarray:
+            return getattr(self, var_name)
+
+        setattr(self, fn_name, getter)
 
     def _download_file(self, filename: str, filepath: str) -> None:
         for mirror in self.mirrors:
             url = urljoin(mirror, filename)
             try:
                 print(f"Downloading {url}")
                 urlretrieve(url, filepath)
@@ -159,17 +172,19 @@
     Fashion-MNIST Dataset
     https://github.com/zalandoresearch/fashion-mnist
 
     Attributes
     ----------
     target_dir : str
         Directory where all files exist or will be downloaded.
-    train_images, train_labels, test_images, test_labels : np.ndarray, optional
+    _train_images, _train_labels, _test_images, _test_labels : np.ndarray, optional
         Numpy array representation of train/test images/labels from FashionMNIST dataset.
         May be None if wasn't loaded manually or during initialization.
+        If is not None, corresponding getter, e.g., _train_images -> train_images(),
+        will be available.
     classes : list[str]
         Class names.
     mirrors : list[str]
         List of urls where dataset is hosted.
     resources : dict[str, tuple[str, str]]
        Dictionary of data files with filename and md5 hash.
     """
@@ -218,17 +233,19 @@
     Kuzushiji-MNIST Dataset
     https://github.com/rois-codh/kmnist
 
     Attributes
     ----------
     target_dir : str
         Directory where all files exist or will be downloaded.
-    train_images, train_labels, test_images, test_labels : np.ndarray, optional
+    _train_images, _train_labels, _test_images, _test_labels : np.ndarray, optional
         Numpy array representation of train/test images/labels from KMNIST dataset.
         May be None if wasn't loaded manually or during initialization.
+        If is not None, corresponding getter, e.g., _train_images -> train_images(),
+        will be available.
     classes : list[str]
         Class names.
     mirrors : list[str]
         List of urls where dataset is hosted.
     resources : dict[str, tuple[str, str]]
        Dictionary of data files with filename and md5 hash.
     """
```

### Comparing `mnists-0.1.0/mnists/utils.py` & `mnists-0.2.0rc1/mnists/utils.py`

 * *Files identical despite different names*

### Comparing `mnists-0.1.0/mnists.egg-info/PKG-INFO` & `mnists-0.2.0rc1/mnists.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mnists
-Version: 0.1.0
+Version: 0.2.0rc1
 Summary: MNISTs: All MNIST-like datasets in one package
 Author-email: Piotr Czarnik <ptr.czarnik@gmail.com>
 Project-URL: Homepage, https://github.com/pczarnik/mnists
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
@@ -31,55 +31,55 @@
 
 Each dataset stores train/test images as numpy arrays of shape `(n_samples, img_height, img_width)` and train/test labels as numpy arrays of shape `(n_samples,)`.
 
 MNIST example:
 ```python
 >>> from mnists import MNIST
 >>> mnist = MNIST()
->>> type(mnist.train_images)
+>>> type(mnist.train_images())
 <class 'numpy.ndarray'>
->>> mnist.train_images.dtype
+>>> mnist.train_images().dtype
 dtype('uint8')
->>> mnist.train_images.min()
+>>> mnist.train_images().min()
 0
->>> mnist.train_images.max()
+>>> mnist.train_images().max()
 255
->>> mnist.train_images.shape
+>>> mnist.train_images().shape
 (60000, 28, 28)
->>> mnist.train_labels.shape
+>>> mnist.train_labels().shape
 (60000,)
->>> mnist.test_images.shape
+>>> mnist.test_images().shape
 (10000, 28, 28)
->>> mnist.test_labels.shape
+>>> mnist.test_labels().shape
 (10000,)
 >>> mnist.classes[:3]
 ['0 - zero', '1 - one', '2 - two']
 ```
 
 FashionMNIST example:
 ```python
 from mnists import FashionMNIST
 import matplotlib.pyplot as plt
 
 fmnist = FashionMNIST()
-plt.imshow(fmnist.train_images[0], cmap='gray')
-plt.title(fmnist.classes[fmnist.train_labels[0]])
+plt.imshow(fmnist.train_images()[0], cmap='gray')
+plt.title(fmnist.classes[fmnist.train_labels()[0]])
 plt.axis('off')
 plt.show()
 ```
 ![FashionMNIST example](https://raw.githubusercontent.com/pczarnik/mnists/main/imgs/fmnist_boot.png)
 
 KMNIST example:
 ```python
 from mnists import KMNIST
 import matplotlib.pyplot as plt
 
 kmnist = KMNIST()
 plt.imshow(
-    kmnist.test_images[:256]
+    kmnist.test_images()[:256]
         .reshape(16, 16, 28, 28)
         .swapaxes(1, 2)
         .reshape(16 * 28, -1),
     cmap='gray')
 plt.axis('off')
 plt.show()
 ```
```

### Comparing `mnists-0.1.0/pyproject.toml` & `mnists-0.2.0rc1/pyproject.toml`

 * *Files identical despite different names*

