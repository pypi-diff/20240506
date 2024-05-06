# Comparing `tmp/bio_volumentations-1.1.2.tar.gz` & `tmp/bio_volumentations-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bio_volumentations-1.1.2.tar", last modified: Mon Apr 15 11:34:21 2024, max compression
+gzip compressed data, was "bio_volumentations-1.2.0.tar", last modified: Mon May  6 12:33:42 2024, max compression
```

## Comparing `bio_volumentations-1.1.2.tar` & `bio_volumentations-1.2.0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2024-04-15 11:34:21.970596 bio_volumentations-1.1.2/
--rw-rw-rw-   0        0        0     1120 2024-04-15 07:21:36.000000 bio_volumentations-1.1.2/LICENSE
--rw-rw-rw-   0        0        0    10176 2024-04-15 11:34:21.970596 bio_volumentations-1.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     9108 2024-04-15 11:16:30.000000 bio_volumentations-1.1.2/README.md
-drwxrwxrwx   0        0        0        0 2024-04-15 11:34:21.937233 bio_volumentations-1.1.2/bio_volumentations/
--rw-rw-rw-   0        0        0     4025 2024-04-15 07:21:36.000000 bio_volumentations-1.1.2/bio_volumentations/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-15 11:34:21.953326 bio_volumentations-1.1.2/bio_volumentations/augmentations/
--rw-rw-rw-   0        0        0     3953 2024-04-15 07:21:36.000000 bio_volumentations-1.1.2/bio_volumentations/augmentations/__init__.py
--rw-rw-rw-   0        0        0    25874 2024-04-15 07:21:36.000000 bio_volumentations-1.1.2/bio_volumentations/augmentations/functional.py
--rw-rw-rw-   0        0        0     6343 2024-04-15 07:21:36.000000 bio_volumentations-1.1.2/bio_volumentations/augmentations/spatial_funcional.py
--rw-rw-rw-   0        0        0    63200 2024-04-15 07:21:36.000000 bio_volumentations-1.1.2/bio_volumentations/augmentations/transforms.py
--rw-rw-rw-   0        0        0     7379 2024-04-15 07:21:36.000000 bio_volumentations-1.1.2/bio_volumentations/augmentations/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-15 11:34:21.953326 bio_volumentations-1.1.2/bio_volumentations/conversion/
--rw-rw-rw-   0        0        0     3910 2024-04-15 07:21:36.000000 bio_volumentations-1.1.2/bio_volumentations/conversion/__init__.py
--rw-rw-rw-   0        0        0     4070 2024-04-15 07:21:36.000000 bio_volumentations-1.1.2/bio_volumentations/conversion/functional.py
--rw-rw-rw-   0        0        0     7095 2024-04-15 07:21:36.000000 bio_volumentations-1.1.2/bio_volumentations/conversion/transforms.py
-drwxrwxrwx   0        0        0        0 2024-04-15 11:34:21.970596 bio_volumentations-1.1.2/bio_volumentations/core/
--rw-rw-rw-   0        0        0     3869 2024-04-15 07:21:36.000000 bio_volumentations-1.1.2/bio_volumentations/core/__init__.py
--rw-rw-rw-   0        0        0     6040 2024-04-15 07:21:36.000000 bio_volumentations-1.1.2/bio_volumentations/core/composition.py
--rw-rw-rw-   0        0        0     6382 2024-04-15 07:21:36.000000 bio_volumentations-1.1.2/bio_volumentations/core/transforms_interface.py
--rw-rw-rw-   0        0        0     5558 2024-04-15 07:21:36.000000 bio_volumentations-1.1.2/bio_volumentations/random_utils.py
--rw-rw-rw-   0        0        0     2557 2024-04-15 07:21:36.000000 bio_volumentations-1.1.2/bio_volumentations/typing.py
-drwxrwxrwx   0        0        0        0 2024-04-15 11:34:21.970596 bio_volumentations-1.1.2/bio_volumentations.egg-info/
--rw-rw-rw-   0        0        0    10176 2024-04-15 11:34:21.000000 bio_volumentations-1.1.2/bio_volumentations.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      851 2024-04-15 11:34:21.000000 bio_volumentations-1.1.2/bio_volumentations.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-15 11:34:21.000000 bio_volumentations-1.1.2/bio_volumentations.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2024-04-15 11:34:21.000000 bio_volumentations-1.1.2/bio_volumentations.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2024-04-15 11:34:21.000000 bio_volumentations-1.1.2/bio_volumentations.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2851 2024-04-15 11:34:04.000000 bio_volumentations-1.1.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-15 11:34:21.970596 bio_volumentations-1.1.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-15 11:34:21.970596 bio_volumentations-1.1.2/tests/
--rw-rw-rw-   0        0        0      204 2024-04-15 07:21:36.000000 bio_volumentations-1.1.2/tests/test_random_utils.py
+drwxrwxrwx   0        0        0        0 2024-05-06 12:33:42.696520 bio_volumentations-1.2.0/
+-rw-rw-rw-   0        0        0     1120 2024-04-15 07:21:36.000000 bio_volumentations-1.2.0/LICENSE
+-rw-rw-rw-   0        0        0    14366 2024-05-06 12:33:42.679955 bio_volumentations-1.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0    13281 2024-05-06 09:17:31.000000 bio_volumentations-1.2.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-06 12:33:42.563234 bio_volumentations-1.2.0/bio_volumentations/
+-rw-rw-rw-   0        0        0     4025 2024-04-15 07:21:36.000000 bio_volumentations-1.2.0/bio_volumentations/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-06 12:33:42.629957 bio_volumentations-1.2.0/bio_volumentations/augmentations/
+-rw-rw-rw-   0        0        0     3950 2024-05-06 07:28:42.000000 bio_volumentations-1.2.0/bio_volumentations/augmentations/__init__.py
+-rw-rw-rw-   0        0        0    25893 2024-05-06 07:28:42.000000 bio_volumentations-1.2.0/bio_volumentations/augmentations/functional.py
+-rw-rw-rw-   0        0        0     6617 2024-05-06 07:28:42.000000 bio_volumentations-1.2.0/bio_volumentations/augmentations/spatial_funcional.py
+-rw-rw-rw-   0        0        0    63120 2024-05-06 07:28:42.000000 bio_volumentations-1.2.0/bio_volumentations/augmentations/transforms.py
+-rw-rw-rw-   0        0        0     7358 2024-05-06 07:28:42.000000 bio_volumentations-1.2.0/bio_volumentations/augmentations/utils.py
+-rw-rw-rw-   0        0        0     2557 2024-05-06 07:28:42.000000 bio_volumentations-1.2.0/bio_volumentations/biovol_typing.py
+drwxrwxrwx   0        0        0        0 2024-05-06 12:33:42.646613 bio_volumentations-1.2.0/bio_volumentations/conversion/
+-rw-rw-rw-   0        0        0     3910 2024-04-15 07:21:36.000000 bio_volumentations-1.2.0/bio_volumentations/conversion/__init__.py
+-rw-rw-rw-   0        0        0     4070 2024-04-15 07:21:36.000000 bio_volumentations-1.2.0/bio_volumentations/conversion/functional.py
+-rw-rw-rw-   0        0        0     7095 2024-04-15 07:21:36.000000 bio_volumentations-1.2.0/bio_volumentations/conversion/transforms.py
+drwxrwxrwx   0        0        0        0 2024-05-06 12:33:42.679955 bio_volumentations-1.2.0/bio_volumentations/core/
+-rw-rw-rw-   0        0        0     3869 2024-04-15 07:21:36.000000 bio_volumentations-1.2.0/bio_volumentations/core/__init__.py
+-rw-rw-rw-   0        0        0     6040 2024-04-15 07:21:36.000000 bio_volumentations-1.2.0/bio_volumentations/core/composition.py
+-rw-rw-rw-   0        0        0     6382 2024-04-15 07:21:36.000000 bio_volumentations-1.2.0/bio_volumentations/core/transforms_interface.py
+-rw-rw-rw-   0        0        0     5565 2024-05-06 07:28:42.000000 bio_volumentations-1.2.0/bio_volumentations/random_utils.py
+drwxrwxrwx   0        0        0        0 2024-05-06 12:33:42.679955 bio_volumentations-1.2.0/bio_volumentations.egg-info/
+-rw-rw-rw-   0        0        0    14366 2024-05-06 12:33:42.000000 bio_volumentations-1.2.0/bio_volumentations.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      858 2024-05-06 12:33:42.000000 bio_volumentations-1.2.0/bio_volumentations.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-06 12:33:42.000000 bio_volumentations-1.2.0/bio_volumentations.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2024-05-06 12:33:42.000000 bio_volumentations-1.2.0/bio_volumentations.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2024-05-06 12:33:42.000000 bio_volumentations-1.2.0/bio_volumentations.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2674 2024-05-06 09:17:30.000000 bio_volumentations-1.2.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-06 12:33:42.696640 bio_volumentations-1.2.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-06 12:33:42.679955 bio_volumentations-1.2.0/tests/
+-rw-rw-rw-   0        0        0      196 2024-05-06 07:28:55.000000 bio_volumentations-1.2.0/tests/test_random_utils.py
```

### Comparing `bio_volumentations-1.1.2/LICENSE` & `bio_volumentations-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bio_volumentations-1.1.2/PKG-INFO` & `bio_volumentations-1.2.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: bio-volumentations
-Version: 1.1.2
-Summary: Library for 3D-5D augmentations of volumetric multi-dimensional biomedical images
+Version: 1.2.0
+Summary: Library for 3D-5D augmentations of volumetric multi-dimensional biomedical images and their annotations
 Author: Lucia Hradecká, Filip Lux, Samuel Šuľan
 Author-email: Lucia Hradecká <lucia.d.hradecka@gmail.com>, Filip Lux <lux.filip@gmail.com>
 License: MIT License
-Project-URL: Homepage, https://gitlab.fi.muni.cz/cbia/bio-volumentations/-/tree/v1-1-0?ref_type=heads
-Project-URL: Documentation, https://biovolumentations.readthedocs.io/v1-1-2/
-Project-URL: Repository, https://gitlab.fi.muni.cz/cbia/bio-volumentations/-/tree/v1-1-0?ref_type=heads
+Project-URL: Homepage, https://gitlab.fi.muni.cz/cbia/bio-volumentations/-/tree/1.2.0?ref_type=tags
+Project-URL: Documentation, https://biovolumentations.readthedocs.io/1.2.0/
+Project-URL: Repository, https://gitlab.fi.muni.cz/cbia/bio-volumentations/-/tree/1.2.0?ref_type=tags
 Keywords: image,augmentation,3D,volumetric,biomedical,bioimage,preprocessing,transformation
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.1
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -19,192 +19,262 @@
 Requires-Dist: scipy
 Requires-Dist: scikit-image
 Requires-Dist: matplotlib
 Requires-Dist: SimpleITK
 
 # Bio-Volumentations
 
-`Bio-Volumentations` is an image augmentation and preprocessing package for 3D, 4D, and 5D biomedical images.
+`Bio-Volumentations` is an image augmentation and preprocessing package for 3D (volumetric), 
+4D (time-lapse volumetric or multi-channel volumetric), and 5D (time-lapse multi-channel volumetric) 
+biomedical images and their annotations.
 
-It offers a range of image transformations implemented efficiently for time-lapse multi-channel volumetric image data.
+The library offers a wide range of efficiently implemented image transformations.
 This includes both preprocessing transformations (such as intensity normalisation, padding, and type casting) 
 and augmentation transformations (such as affine transform, noise addition and removal, and contrast manipulation).
 
-The `Bio-Volumentations` library is a suitable tool for data manipulation in machine learning applications. 
+The `Bio-Volumentations` library is a suitable tool for image manipulation in machine learning applications. 
 It can be used with any major Python deep learning library, including PyTorch, PyTorch Lightning, TensorFlow, and Keras.
 
-This library builds upon wide-spread libraries such as Albumentations (see the Contributions section below) 
-in terms of design and user interface. Therefore, it can easily be adopted by developers.
+This library builds upon wide-spread libraries such as Albumentations and TorchIO (see the Contributions section below). 
+Therefore, it can easily be adopted by developers.
 
 # Installation
 
 Install the package from pip using:
 ```python
 pip install bio-volumentations
 ```
+
+See [the project's PyPi page](https://pypi.org/project/bio-volumentations/) for more details.
+
 ## Requirements
 
-NumPy       https://numpy.org/ <br> 
-SciPy       https://scipy.org/ <br>
-Scikit-image https://scikit-image.org/ <br>
-Matplotlib  https://matplotlib.org/ <br>
-SimpleITK   https://simpleitk.org/ <br>
+- [NumPy](https://numpy.org/)
+- [SciPy](https://scipy.org/)
+- [Scikit-image](https://scikit-image.org/)
+- [Matplotlib](https://matplotlib.org/)
+- [SimpleITK](https://simpleitk.org/)
 
 
 # Usage
 
 ### Importing
 
 Import the library to your project using:
 ```python
 import bio_volumentations as biovol
 ```
 
 ### How to Use Bio-Volumentations?
 
-The Bio-Volumentations library processes 3D, 4D, and 5D images. Each image must be 
-represented as `numpy.ndarray`s and must conform  to the following conventions:
+The `Bio-Volumentations` library processes 3D, 4D, and 5D images. Each image must be 
+represented as a `numpy.ndarray` and must conform to the following conventions:
 
 - The order of dimensions is [C, Z, Y, X, T], where C is the channel dimension, 
    T is the time dimension, and Z, Y, and X are the spatial dimensions.
-- The three spatial dimensions (Z, Y, X) are compulsory.
+- The three spatial dimensions (Z, Y, X) must be present. To transform a 2D image, please create a dummy Z dimension first. 
 - The channel (C) dimension is optional. If it is not present, the library will automatically
-   create a dummy dimension in its place and output an image of shape (1, Z, Y, X).
+   create a dummy dimension in its place, so the output image shape will be [1, Z, Y, X].
 - The time (T) dimension is optional and can only be present if the channel (C) dimension is 
-   also present.
+   also present in the input data. To process single-channel time-lapse images, please create a dummy C dimension first.
+
+Thus, an input image is interpreted in the following ways based on its shape:
+
+1. [Z, Y, X] ... a single-channel volumetric image;
+2. [C, Z, Y, X] ... a multi-channel volumetric image;
+3. [C, Z, Y, X, T] ... a single-channel as well as multi-channel volumetric image sequence.
+
+The shape of the output image is either [C, Z, Y, X] (cases 1 & 2) or [C, Z, Y, X, T] (case 3).
 
-Thus, the input images can have these shapes:
+The images are type-casted to a floating-point datatype before transformations, irrespective of their actual datatype.
 
-- [Z, Y, X] (a single-channel volumetric image)
-- [C, Z, Y, X] (a multi-channel volumetric image)
-- [C, Z, Y, X, T] (a single-channel as well as multi-channel volumetric image sequence)
+For the specification of image annotation conventions, please see below.
 
-**It is strongly recommended to use `Compose` to create and use transformation pipelines.** 
+**It is strongly recommended to use `Compose` to create and use transformation pipelines.** <br>
 The `Compose` class automatically checks and adjusts image format, datatype, stacks
 individual transforms to a pipeline, and outputs the image as a contiguous array. 
-Optionally, it can also convert the transformed image to a desired format.
+Optionally, it can also convert the transformed image to a desired format. <br>
+If you call transformations outside of `Compose`, we cannot guarantee the all assumptions are checked and enforced, 
+so you might encounter unexpected behaviour.
 
-More at the [documentation pages](https://www.google.com).
-
-Below, there are several examples of how to use this library.
+Below, there are several examples of how to use this library. You are also welcome to check 
+[our documentation pages](https://biovolumentations.readthedocs.io/1.2.0/).
 
 ### Example: Transforming a Single Image
 
+To create the transformation pipeline, you just need to instantiate all desired transformations
+(with the desired parameter values)
+and then feed a list of these transformations into a new `Compose` object. 
+
+Optionally, you can specify a datatype conversion transformation that will be applied after the last transformation
+in the list, e.g. from the default `numpy.ndarray` to a `torch.Tensor`. You can also specify the probability
+of actually applying the whole pipeline as a number between 0 and 1. The default probability is 1 (always apply).
+See the [docs](https://biovolumentations.readthedocs.io/1.2.0/) for more details.
+
+The `Compose` object is callable. The data is passed as a keyword argument, and the call returns a dictionary 
+with the same keywords and corresponding transformed images. This might look like an overkill for a single image, 
+but will come handy when transforming images with annotations. The default key for the image is `image`.
+
+
 ```python
 import numpy as np
 from bio_volumentations import Compose, RandomGamma, RandomRotate90, GaussianBlur
 
-# Create the transformation using Compose from a list of transformations
+# Create the transformation pipeline using Compose
 aug = Compose([
         RandomGamma(gamma_limit = (0.8, 1,2), p = 0.8),
         RandomRotate90(axes = [1, 2, 3], p = 1),
         GaussianBlur(sigma = 1.2, p = 0.8)
       ])
 
-# Generate an image 
+# Generate an image - shape [C, Z, Y, X]
 img = np.random.rand(1, 128, 256, 256)
 
 # Transform the image
-# Notice that the image must be passed as a keyword argument to the transformation pipeline
+# Please note that the image must be passed as a keyword argument to the transformation pipeline
 # and extracted from the outputted dictionary.
 data = {'image': img}
 aug_data = aug(**data)
 transformed_img = aug_data['image']
 ```
 
 ### Example: Transforming Image Tuples
 
 Sometimes, it is necessary to consistently transform a tuple of corresponding images.
-To that end, Bio-Volumentations define several target types:
+To that end, `Bio-Volumentations` define several target types:
 
-- `image` for the image data;
-- `mask` for integer-valued label images; and
-- `float_mask` for real-valued label images.
+- `image` for the image data (any datatype allowed, gets converted to floating-point by default);
+- `mask` for integer-valued label images (expected integer datatype); and
+- `float_mask` for real-valued label images (expected floating-point datatype).
 
 The `mask` and `float_mask` target types are expected to have the same shape as the `image`
 target except for the channel (C) dimension which must not be included. 
-For example, for images of shape (150, 300, 300), (1, 150, 300, 300), or
-(4, 150, 300, 300), the corresponding `mask` must be of shape (150, 300, 300).
-If one wants to use a multichannel `mask` or `float_mask`, one has to split it into
+For example, for images of shape [150, 300, 300], [1, 150, 300, 300], and
+[4, 150, 300, 300], the corresponding `mask` and `float_mask` must be of shape [150, 300, 300].
+If you want to use a multichannel `mask` or `float_mask`, you have to split it into
 a set of single-channel `mask`s or `float_mask`s, respectively, and input them
 as stand-alone targets (see below).
 
 If a `Random...` transform receives multiple targets on its input in a single call,
-the same random numbers are used to transform all of these targets.
+the same transformation parameters are used to transform all of these targets.
+For example, `RandomAffineTransform` applies the same geometric transformation to all target types in a single call.
+
+Some transformations, such as `RandomGaussianNoise` or `RandomGamma`, are only defined for the `image` target 
+and leave the `mask` and `float_mask` targets unchanged. Please consult the 
+[documentation of the individual transforms](https://biovolumentations.readthedocs.io/1.2.0/) for more details.
 
-However, some transformations might behave slightly differently for the individual
-target types. For example, `RandomCrop` works in the same way for all target types, while
-`RandomGaussianNoise` only affects the `image` target and leaves the `mask` and
-`float_mask` targets unchanged. Please consult the documentation of respective transforms
-for more details.
+The image tuples are fed to the `Compose` object call as keyword arguments and extracted from the outputted dictionary
+using the same keys. The default key values are `image`, `mask`, and `float_mask`.
 
 ```python
 import numpy as np
 from bio_volumentations import Compose, RandomGamma, RandomRotate90, GaussianBlur
 
-# Create the transformation using Compose from a list of transformations
+# Create the transformation using Compose
 aug = Compose([
         RandomGamma(gamma_limit = (0.8, 1,2), p = 0.8),
         RandomRotate90(axes = [1, 2, 3], p = 1),
         GaussianBlur(sigma = 1.2, p = 0.8)
       ])
 
 # Generate image and a corresponding labeled image
 img = np.random.rand(1, 128, 256, 256)
 lbl = np.random.randint(0, 1, size=(128, 256, 256), dtype=np.uint8)
 
 # Transform the images
-# Notice that the images must be passed as keyword arguments to the transformation pipeline
+# Please note that the images must be passed as keyword arguments to the transformation pipeline
 # and extracted from the outputted dictionary.
 data = {'image': img, 'mask': lbl}
 aug_data = aug(**data)
 transformed_img, transformed_lbl = aug_data['image'], aug_data['mask']
 ```
 
 
 ### Example: Transforming Multiple Images of the Same Target Type
 
-Although there are only three target types, one input arbitrary number of images to any
-transformation. To achieve this, one has to define the value of the `targets` argument
+Although there are only three target types, you can input an arbitrary number of images to any
+transformation. To achieve this, you have to define the value of the `targets` argument
 when creating a `Compose` object.
 
-`targets` must be a list with 3 items: a list with names of `image`-type targets, 
-a list with names of `mask`-type targets, and 
-a list with names of `float_mask`-type targets. The specified names will then be used 
-to input the images to the transformation call as well as during extracting the
-transformed images from the outputted dictionary. Please see the code below 
-for a practical example.
+The value of `targets` must be a list with exactly 3 items: a list with keys of `image`-type targets, 
+a list with keys of `mask`-type targets, and 
+a list with keys of `float_mask`-type targets. 
+The specified keys will then be used to input the images to the transformation call as well as to extract the
+transformed images from the outputted dictionary. 
+
+The keys can be any valid dictionary keys; most importantly, they must be unique across all target types.
+You don't need to feed an image for each target to the transformation call: in our example below, we have four targets
+(two `image`, one `mask`, and one `float_mask`), but we only transform three images.
+
+You cannot define your own target types; that would require re-implementing all existing transforms.
 
 ```python
 import numpy as np
 from bio_volumentations import Compose, RandomGamma, RandomRotate90, GaussianBlur
 
-# Create the transformation using Compose from a list of transformations and define targets
+# Create the transformation using Compose: do not forget to define targets
 aug = Compose([
         RandomGamma( gamma_limit = (0.8, 1,2), p = 0.8),
         RandomRotate90(axes = [1, 2, 3], p = 1),
         GaussianBlur(sigma = 1.2, p = 0.8)
     ], 
     targets= [ ['image' , 'image1'] , ['mask'], ['float_mask'] ])
 
-# Generate the image data
+# Generate the image data: two images and a single int-valued mask
 img = np.random.rand(1, 128, 256, 256)
 img1 = np.random.rand(1, 128, 256, 256)
 lbl = np.random.randint(0, 1, size=(128, 256, 256), dtype=np.uint8)
 
 # Transform the images
-# Notice that the images must be passed as keyword arguments to the transformation pipeline
+# Please note that the images must be passed as keyword arguments to the transformation pipeline
 # and extracted from the outputted dictionary.
 data = {'image': img, 'image1': img1, 'mask': lbl}
 aug_data = aug(**data)
 transformed_img = aug_data['image']
 transformed_img1 = aug_data['image1']
 transformed_lbl = aug_data['mask']
 ```
 
+### Example: Adding a Custom Transformation
+
+Each transformation inherits from the `Transform` class. You can thus easily implement your own 
+transformations and use them with this library. You can check our implementations to see how this can be done.
+For example, `Flip` can be implemented as follows:
+
+```python
+import numpy as np
+from typing import List
+from bio_volumentations import DualTransform
+
+class Flip(DualTransform):
+    def __init__(self, axes: List[int] = None, always_apply=False, p=1):
+        super().__init__(always_apply, p)
+        self.axes = axes
+
+    # Transform the image
+    def apply(self, img, **params):
+        return np.flip(img, params["axes"])
+
+    # Transform the int-valued mask
+    def apply_to_mask(self, mask, **params):
+       # The mask has no channels
+        return np.flip(mask, axis=[item - 1 for item in params["axes"]])
+    
+    # Transform the float-valued mask
+    # By default, float_mask uses the implementation of mask, unless it is overridden (see the implementation of DualTransform).
+    #def apply_to_float_mask(self, float_mask, **params):
+    #    return self.apply_to_mask(float_mask, **params)
+
+    # Get transformation parameters. Useful especially for RandomXXX transforms to ensure consistent transformation of image tuples.
+    def get_params(self, **data):
+        axes = self.axes if self.axes is not None else [1, 2, 3]
+        return {"axes": axes}
+```
+
+
 # Implemented Transforms
 
 ### A List of Implemented Transformations
 
 Point transformations:
 ```python
 GaussianNoise 
@@ -243,26 +313,25 @@
 # Contributions
 
 Authors of the Bio-Volumentations library: Samuel Šuľan, Lucia Hradecká, Filip Lux.
 - Lucia Hradecká: lucia.d.hradecka@gmail.com   
 - Filip Lux: lux.filip@gmail.com     
 
 The Bio-Volumentations library is based on the following image augmentation libraries:
-- Albumentations:           https://github.com/albumentations-team/albumentations       
-- 3D Conversion:            https://github.com/ashawkey/volumentations                  
-- Continued Development:    https://github.com/ZFTurbo/volumentations                   
-- Enhancements:             https://github.com/qubvel/volumentations                    
-- Further Enhancements:     https://github.com/muellerdo/volumentations     
-
-We would thus like to thank their authors, namely:
-- The Albumentations team: https://github.com/albumentations-team                    
-- Pavel Iakubovskii: https://github.com/qubvel                                 
-- ZFTurbo: https://github.com/ZFTurbo                                
-- ashawkey: https://github.com/ashawkey                               
-- Dominik Müller: https://github.com/muellerdo         
+- [Albumentations](https://github.com/albumentations-team/albumentations)  
+- [Volumentations](https://github.com/ashawkey/volumentations)                  
+- [Volumentations: Continued Development](https://github.com/ZFTurbo/volumentations)                   
+- [Volumentations: Enhancements](https://github.com/qubvel/volumentations)        
+- [Volumentations: Further Enhancements](https://github.com/muellerdo/volumentations)
+- [TorchIO](https://github.com/fepegar/torchio)
+
+We would thus like to thank their authors, namely [the Albumentations team](https://github.com/albumentations-team), 
+[Pavel Iakubovskii](https://github.com/qubvel), [ZFTurbo](https://github.com/ZFTurbo), 
+[ashawkey](https://github.com/ashawkey), [Dominik Müller](https://github.com/muellerdo), and 
+[TorchIO contributors](https://github.com/fepegar/torchio?tab=readme-ov-file#contributors).         
 
 
 # Citation
 
 TBA
```

### Comparing `bio_volumentations-1.1.2/README.md` & `bio_volumentations-1.2.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,187 +1,257 @@
 # Bio-Volumentations
 
-`Bio-Volumentations` is an image augmentation and preprocessing package for 3D, 4D, and 5D biomedical images.
+`Bio-Volumentations` is an image augmentation and preprocessing package for 3D (volumetric), 
+4D (time-lapse volumetric or multi-channel volumetric), and 5D (time-lapse multi-channel volumetric) 
+biomedical images and their annotations.
 
-It offers a range of image transformations implemented efficiently for time-lapse multi-channel volumetric image data.
+The library offers a wide range of efficiently implemented image transformations.
 This includes both preprocessing transformations (such as intensity normalisation, padding, and type casting) 
 and augmentation transformations (such as affine transform, noise addition and removal, and contrast manipulation).
 
-The `Bio-Volumentations` library is a suitable tool for data manipulation in machine learning applications. 
+The `Bio-Volumentations` library is a suitable tool for image manipulation in machine learning applications. 
 It can be used with any major Python deep learning library, including PyTorch, PyTorch Lightning, TensorFlow, and Keras.
 
-This library builds upon wide-spread libraries such as Albumentations (see the Contributions section below) 
-in terms of design and user interface. Therefore, it can easily be adopted by developers.
+This library builds upon wide-spread libraries such as Albumentations and TorchIO (see the Contributions section below). 
+Therefore, it can easily be adopted by developers.
 
 # Installation
 
 Install the package from pip using:
 ```python
 pip install bio-volumentations
 ```
+
+See [the project's PyPi page](https://pypi.org/project/bio-volumentations/) for more details.
+
 ## Requirements
 
-NumPy       https://numpy.org/ <br> 
-SciPy       https://scipy.org/ <br>
-Scikit-image https://scikit-image.org/ <br>
-Matplotlib  https://matplotlib.org/ <br>
-SimpleITK   https://simpleitk.org/ <br>
+- [NumPy](https://numpy.org/)
+- [SciPy](https://scipy.org/)
+- [Scikit-image](https://scikit-image.org/)
+- [Matplotlib](https://matplotlib.org/)
+- [SimpleITK](https://simpleitk.org/)
 
 
 # Usage
 
 ### Importing
 
 Import the library to your project using:
 ```python
 import bio_volumentations as biovol
 ```
 
 ### How to Use Bio-Volumentations?
 
-The Bio-Volumentations library processes 3D, 4D, and 5D images. Each image must be 
-represented as `numpy.ndarray`s and must conform  to the following conventions:
+The `Bio-Volumentations` library processes 3D, 4D, and 5D images. Each image must be 
+represented as a `numpy.ndarray` and must conform to the following conventions:
 
 - The order of dimensions is [C, Z, Y, X, T], where C is the channel dimension, 
    T is the time dimension, and Z, Y, and X are the spatial dimensions.
-- The three spatial dimensions (Z, Y, X) are compulsory.
+- The three spatial dimensions (Z, Y, X) must be present. To transform a 2D image, please create a dummy Z dimension first. 
 - The channel (C) dimension is optional. If it is not present, the library will automatically
-   create a dummy dimension in its place and output an image of shape (1, Z, Y, X).
+   create a dummy dimension in its place, so the output image shape will be [1, Z, Y, X].
 - The time (T) dimension is optional and can only be present if the channel (C) dimension is 
-   also present.
+   also present in the input data. To process single-channel time-lapse images, please create a dummy C dimension first.
+
+Thus, an input image is interpreted in the following ways based on its shape:
+
+1. [Z, Y, X] ... a single-channel volumetric image;
+2. [C, Z, Y, X] ... a multi-channel volumetric image;
+3. [C, Z, Y, X, T] ... a single-channel as well as multi-channel volumetric image sequence.
+
+The shape of the output image is either [C, Z, Y, X] (cases 1 & 2) or [C, Z, Y, X, T] (case 3).
 
-Thus, the input images can have these shapes:
+The images are type-casted to a floating-point datatype before transformations, irrespective of their actual datatype.
 
-- [Z, Y, X] (a single-channel volumetric image)
-- [C, Z, Y, X] (a multi-channel volumetric image)
-- [C, Z, Y, X, T] (a single-channel as well as multi-channel volumetric image sequence)
+For the specification of image annotation conventions, please see below.
 
-**It is strongly recommended to use `Compose` to create and use transformation pipelines.** 
+**It is strongly recommended to use `Compose` to create and use transformation pipelines.** <br>
 The `Compose` class automatically checks and adjusts image format, datatype, stacks
 individual transforms to a pipeline, and outputs the image as a contiguous array. 
-Optionally, it can also convert the transformed image to a desired format.
+Optionally, it can also convert the transformed image to a desired format. <br>
+If you call transformations outside of `Compose`, we cannot guarantee the all assumptions are checked and enforced, 
+so you might encounter unexpected behaviour.
 
-More at the [documentation pages](https://www.google.com).
-
-Below, there are several examples of how to use this library.
+Below, there are several examples of how to use this library. You are also welcome to check 
+[our documentation pages](https://biovolumentations.readthedocs.io/1.2.0/).
 
 ### Example: Transforming a Single Image
 
+To create the transformation pipeline, you just need to instantiate all desired transformations
+(with the desired parameter values)
+and then feed a list of these transformations into a new `Compose` object. 
+
+Optionally, you can specify a datatype conversion transformation that will be applied after the last transformation
+in the list, e.g. from the default `numpy.ndarray` to a `torch.Tensor`. You can also specify the probability
+of actually applying the whole pipeline as a number between 0 and 1. The default probability is 1 (always apply).
+See the [docs](https://biovolumentations.readthedocs.io/1.2.0/) for more details.
+
+The `Compose` object is callable. The data is passed as a keyword argument, and the call returns a dictionary 
+with the same keywords and corresponding transformed images. This might look like an overkill for a single image, 
+but will come handy when transforming images with annotations. The default key for the image is `image`.
+
+
 ```python
 import numpy as np
 from bio_volumentations import Compose, RandomGamma, RandomRotate90, GaussianBlur
 
-# Create the transformation using Compose from a list of transformations
+# Create the transformation pipeline using Compose
 aug = Compose([
         RandomGamma(gamma_limit = (0.8, 1,2), p = 0.8),
         RandomRotate90(axes = [1, 2, 3], p = 1),
         GaussianBlur(sigma = 1.2, p = 0.8)
       ])
 
-# Generate an image 
+# Generate an image - shape [C, Z, Y, X]
 img = np.random.rand(1, 128, 256, 256)
 
 # Transform the image
-# Notice that the image must be passed as a keyword argument to the transformation pipeline
+# Please note that the image must be passed as a keyword argument to the transformation pipeline
 # and extracted from the outputted dictionary.
 data = {'image': img}
 aug_data = aug(**data)
 transformed_img = aug_data['image']
 ```
 
 ### Example: Transforming Image Tuples
 
 Sometimes, it is necessary to consistently transform a tuple of corresponding images.
-To that end, Bio-Volumentations define several target types:
+To that end, `Bio-Volumentations` define several target types:
 
-- `image` for the image data;
-- `mask` for integer-valued label images; and
-- `float_mask` for real-valued label images.
+- `image` for the image data (any datatype allowed, gets converted to floating-point by default);
+- `mask` for integer-valued label images (expected integer datatype); and
+- `float_mask` for real-valued label images (expected floating-point datatype).
 
 The `mask` and `float_mask` target types are expected to have the same shape as the `image`
 target except for the channel (C) dimension which must not be included. 
-For example, for images of shape (150, 300, 300), (1, 150, 300, 300), or
-(4, 150, 300, 300), the corresponding `mask` must be of shape (150, 300, 300).
-If one wants to use a multichannel `mask` or `float_mask`, one has to split it into
+For example, for images of shape [150, 300, 300], [1, 150, 300, 300], and
+[4, 150, 300, 300], the corresponding `mask` and `float_mask` must be of shape [150, 300, 300].
+If you want to use a multichannel `mask` or `float_mask`, you have to split it into
 a set of single-channel `mask`s or `float_mask`s, respectively, and input them
 as stand-alone targets (see below).
 
 If a `Random...` transform receives multiple targets on its input in a single call,
-the same random numbers are used to transform all of these targets.
+the same transformation parameters are used to transform all of these targets.
+For example, `RandomAffineTransform` applies the same geometric transformation to all target types in a single call.
+
+Some transformations, such as `RandomGaussianNoise` or `RandomGamma`, are only defined for the `image` target 
+and leave the `mask` and `float_mask` targets unchanged. Please consult the 
+[documentation of the individual transforms](https://biovolumentations.readthedocs.io/1.2.0/) for more details.
 
-However, some transformations might behave slightly differently for the individual
-target types. For example, `RandomCrop` works in the same way for all target types, while
-`RandomGaussianNoise` only affects the `image` target and leaves the `mask` and
-`float_mask` targets unchanged. Please consult the documentation of respective transforms
-for more details.
+The image tuples are fed to the `Compose` object call as keyword arguments and extracted from the outputted dictionary
+using the same keys. The default key values are `image`, `mask`, and `float_mask`.
 
 ```python
 import numpy as np
 from bio_volumentations import Compose, RandomGamma, RandomRotate90, GaussianBlur
 
-# Create the transformation using Compose from a list of transformations
+# Create the transformation using Compose
 aug = Compose([
         RandomGamma(gamma_limit = (0.8, 1,2), p = 0.8),
         RandomRotate90(axes = [1, 2, 3], p = 1),
         GaussianBlur(sigma = 1.2, p = 0.8)
       ])
 
 # Generate image and a corresponding labeled image
 img = np.random.rand(1, 128, 256, 256)
 lbl = np.random.randint(0, 1, size=(128, 256, 256), dtype=np.uint8)
 
 # Transform the images
-# Notice that the images must be passed as keyword arguments to the transformation pipeline
+# Please note that the images must be passed as keyword arguments to the transformation pipeline
 # and extracted from the outputted dictionary.
 data = {'image': img, 'mask': lbl}
 aug_data = aug(**data)
 transformed_img, transformed_lbl = aug_data['image'], aug_data['mask']
 ```
 
 
 ### Example: Transforming Multiple Images of the Same Target Type
 
-Although there are only three target types, one input arbitrary number of images to any
-transformation. To achieve this, one has to define the value of the `targets` argument
+Although there are only three target types, you can input an arbitrary number of images to any
+transformation. To achieve this, you have to define the value of the `targets` argument
 when creating a `Compose` object.
 
-`targets` must be a list with 3 items: a list with names of `image`-type targets, 
-a list with names of `mask`-type targets, and 
-a list with names of `float_mask`-type targets. The specified names will then be used 
-to input the images to the transformation call as well as during extracting the
-transformed images from the outputted dictionary. Please see the code below 
-for a practical example.
+The value of `targets` must be a list with exactly 3 items: a list with keys of `image`-type targets, 
+a list with keys of `mask`-type targets, and 
+a list with keys of `float_mask`-type targets. 
+The specified keys will then be used to input the images to the transformation call as well as to extract the
+transformed images from the outputted dictionary. 
+
+The keys can be any valid dictionary keys; most importantly, they must be unique across all target types.
+You don't need to feed an image for each target to the transformation call: in our example below, we have four targets
+(two `image`, one `mask`, and one `float_mask`), but we only transform three images.
+
+You cannot define your own target types; that would require re-implementing all existing transforms.
 
 ```python
 import numpy as np
 from bio_volumentations import Compose, RandomGamma, RandomRotate90, GaussianBlur
 
-# Create the transformation using Compose from a list of transformations and define targets
+# Create the transformation using Compose: do not forget to define targets
 aug = Compose([
         RandomGamma( gamma_limit = (0.8, 1,2), p = 0.8),
         RandomRotate90(axes = [1, 2, 3], p = 1),
         GaussianBlur(sigma = 1.2, p = 0.8)
     ], 
     targets= [ ['image' , 'image1'] , ['mask'], ['float_mask'] ])
 
-# Generate the image data
+# Generate the image data: two images and a single int-valued mask
 img = np.random.rand(1, 128, 256, 256)
 img1 = np.random.rand(1, 128, 256, 256)
 lbl = np.random.randint(0, 1, size=(128, 256, 256), dtype=np.uint8)
 
 # Transform the images
-# Notice that the images must be passed as keyword arguments to the transformation pipeline
+# Please note that the images must be passed as keyword arguments to the transformation pipeline
 # and extracted from the outputted dictionary.
 data = {'image': img, 'image1': img1, 'mask': lbl}
 aug_data = aug(**data)
 transformed_img = aug_data['image']
 transformed_img1 = aug_data['image1']
 transformed_lbl = aug_data['mask']
 ```
 
+### Example: Adding a Custom Transformation
+
+Each transformation inherits from the `Transform` class. You can thus easily implement your own 
+transformations and use them with this library. You can check our implementations to see how this can be done.
+For example, `Flip` can be implemented as follows:
+
+```python
+import numpy as np
+from typing import List
+from bio_volumentations import DualTransform
+
+class Flip(DualTransform):
+    def __init__(self, axes: List[int] = None, always_apply=False, p=1):
+        super().__init__(always_apply, p)
+        self.axes = axes
+
+    # Transform the image
+    def apply(self, img, **params):
+        return np.flip(img, params["axes"])
+
+    # Transform the int-valued mask
+    def apply_to_mask(self, mask, **params):
+       # The mask has no channels
+        return np.flip(mask, axis=[item - 1 for item in params["axes"]])
+    
+    # Transform the float-valued mask
+    # By default, float_mask uses the implementation of mask, unless it is overridden (see the implementation of DualTransform).
+    #def apply_to_float_mask(self, float_mask, **params):
+    #    return self.apply_to_mask(float_mask, **params)
+
+    # Get transformation parameters. Useful especially for RandomXXX transforms to ensure consistent transformation of image tuples.
+    def get_params(self, **data):
+        axes = self.axes if self.axes is not None else [1, 2, 3]
+        return {"axes": axes}
+```
+
+
 # Implemented Transforms
 
 ### A List of Implemented Transformations
 
 Point transformations:
 ```python
 GaussianNoise 
@@ -220,26 +290,25 @@
 # Contributions
 
 Authors of the Bio-Volumentations library: Samuel Šuľan, Lucia Hradecká, Filip Lux.
 - Lucia Hradecká: lucia.d.hradecka@gmail.com   
 - Filip Lux: lux.filip@gmail.com     
 
 The Bio-Volumentations library is based on the following image augmentation libraries:
-- Albumentations:           https://github.com/albumentations-team/albumentations       
-- 3D Conversion:            https://github.com/ashawkey/volumentations                  
-- Continued Development:    https://github.com/ZFTurbo/volumentations                   
-- Enhancements:             https://github.com/qubvel/volumentations                    
-- Further Enhancements:     https://github.com/muellerdo/volumentations     
-
-We would thus like to thank their authors, namely:
-- The Albumentations team: https://github.com/albumentations-team                    
-- Pavel Iakubovskii: https://github.com/qubvel                                 
-- ZFTurbo: https://github.com/ZFTurbo                                
-- ashawkey: https://github.com/ashawkey                               
-- Dominik Müller: https://github.com/muellerdo         
+- [Albumentations](https://github.com/albumentations-team/albumentations)  
+- [Volumentations](https://github.com/ashawkey/volumentations)                  
+- [Volumentations: Continued Development](https://github.com/ZFTurbo/volumentations)                   
+- [Volumentations: Enhancements](https://github.com/qubvel/volumentations)        
+- [Volumentations: Further Enhancements](https://github.com/muellerdo/volumentations)
+- [TorchIO](https://github.com/fepegar/torchio)
+
+We would thus like to thank their authors, namely [the Albumentations team](https://github.com/albumentations-team), 
+[Pavel Iakubovskii](https://github.com/qubvel), [ZFTurbo](https://github.com/ZFTurbo), 
+[ashawkey](https://github.com/ashawkey), [Dominik Müller](https://github.com/muellerdo), and 
+[TorchIO contributors](https://github.com/fepegar/torchio?tab=readme-ov-file#contributors).         
 
 
 # Citation
 
 TBA
```

### Comparing `bio_volumentations-1.1.2/bio_volumentations/__init__.py` & `bio_volumentations-1.2.0/bio_volumentations/__init__.py`

 * *Files identical despite different names*

### Comparing `bio_volumentations-1.1.2/bio_volumentations/augmentations/__init__.py` & `bio_volumentations-1.2.0/bio_volumentations/augmentations/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -34,9 +34,10 @@
 #  FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE                  #
 #  AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER                       #
 #  LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,                #
 #  OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE                #
 #  SOFTWARE.                                                                                    #
 # ============================================================================================= #
 
-from ..augmentations.functional import *
-from ..augmentations.transforms import *
+# TODO: can be removed?
+#from .functional import *
+#from .transforms import *
```

### Comparing `bio_volumentations-1.1.2/bio_volumentations/augmentations/functional.py` & `bio_volumentations-1.2.0/bio_volumentations/augmentations/functional.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,19 +38,18 @@
 #  SOFTWARE.                                                                                    #
 # ============================================================================================= #
 
 import numpy as np
 from functools import wraps
 import skimage.transform as skt
 from skimage.exposure import equalize_hist
-from scipy.ndimage import zoom
-from scipy.ndimage import gaussian_filter
+from scipy.ndimage import zoom, gaussian_filter
 from warnings import warn
 
-from ..typing import TypeTripletFloat
+from ..biovol_typing import TypeTripletFloat
 from .spatial_funcional import get_affine_transform, apply_sitk_transform
 
 
 MAX_VALUES_BY_DTYPE = {
     np.dtype("uint8"): 255,
     np.dtype("uint16"): 65535,
     np.dtype("uint32"): 4294967295,
@@ -285,21 +284,21 @@
     for i in range(img.shape[0]):
         img[i] = normalize_channel(img[i], mean[i], std[i])
     return img
 
 
 def gaussian_noise(img, mean, sigma):
     img = img.astype("float32")
-    noise = np.random.normal(mean, sigma, img.shape)
+    noise = np.random.normal(mean, sigma, img.shape).astype(np.float32)
     return img + noise
 
 
 def poisson_noise(img, intensity):
     img = img.astype("float32")
-    noise = np.random.poisson(img) * intensity
+    noise = np.random.poisson(img).astype(np.float32) * intensity
     return img + noise
 
 
 # TODO parameter
 # Anti-aliasing - gaussian filter to smooth. using automatically when downsampling, except when integer
 # and interpolation is 0. (so mask)
 # float mask - how, for now no gaussian filter.
```

### Comparing `bio_volumentations-1.1.2/bio_volumentations/augmentations/spatial_funcional.py` & `bio_volumentations-1.2.0/bio_volumentations/augmentations/spatial_funcional.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 #  AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER                       #
 #  LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,                #
 #  OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE                #
 #  SOFTWARE.                                                                                    #
 # ============================================================================================= #
 
 import numpy as np
-from ..typing import TypeTripletFloat
+from ..biovol_typing import TypeTripletFloat
 from typing import Sequence, Optional
 import SimpleITK as sitk
 
 from .utils import get_image_center, ras_to_lps, np_to_sitk, sitk_to_np
 
 DEBUG = False
 
@@ -128,31 +128,41 @@
         image: np.array,
         sitk_transform: sitk.Euler3DTransform,
         interpolation: str,
         default_value: float,
         spacing: TypeTripletFloat = (1., 1., 1.)
 ) -> np.array:
 
-    assert len(image.shape) == 4, f'image.shape: {image.shape}'
+    assert len(image.shape) >= 4, f'image.shape: {image.shape}'
 
+    # resolve the image shape
     ch = image.shape[0]
-    image_expanded = np.expand_dims(image, 4)
+    fr = 1 if len(image.shape) == 4 else image.shape[4]
+
+    if len(image.shape) == 4:
+        image_expanded = np.expand_dims(image, 4)
+        expanded = True
+    else:
+        image_expanded = image
+        expanded = False
 
     # convert numpy array to sitk image
     sitk_image = np_to_sitk(image_expanded)
     sitk_image.SetSpacing(spacing)
 
     # apply transform
     floating = reference = sitk_image
     interpolator = sitk.ResampleImageFilter()
     interpolator.SetInterpolator(getattr(sitk, interpolation))
     interpolator.SetReferenceImage(reference)
     interpolator.SetDefaultPixelValue(float(default_value))
     interpolator.SetTransform(sitk_transform)
 
     resampled = interpolator.Execute(floating)
-    np_array = sitk_to_np(resampled, channels=ch, frames=1).squeeze(4)
+    np_array = sitk_to_np(resampled, channels=ch, frames=fr)
+    if expanded:
+        np_array = np_array.squeeze(4)
 
     assert image.shape == np_array.shape, f"image.shape: {image.shape} np_array.shape:, {np_array.shape}"
 
     # np_array = np_array.transpose()  # ITK to NumPy convention
     return np_array
```

### Comparing `bio_volumentations-1.1.2/bio_volumentations/augmentations/transforms.py` & `bio_volumentations-1.2.0/bio_volumentations/augmentations/transforms.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 
 import random
 import numpy as np
 from ..core.transforms_interface import DualTransform, ImageOnlyTransform
 from ..augmentations import functional as F
 from ..random_utils import uniform, sample_range_uniform
 from typing import List, Sequence, Tuple, Union
-from ..typing import TypeSextetFloat, TypeTripletFloat, TypePairFloat
+from ..biovol_typing import TypeSextetFloat, TypeTripletFloat, TypePairFloat
 from .utils import parse_limits, parse_coefs, to_tuple
 
 
 # TODO potential upgrade : different sigmas for different channels
 class GaussianNoise(ImageOnlyTransform):
     """Adds Gaussian noise to the image. The noise is drawn from normal distribution with given parameters.
 
@@ -278,28 +278,28 @@
                         interpolation=self.interpolation,
                         border_mode=self.border_mode,
                         value=self.ival,
                         spacing=self.spacing)
 
     def apply_to_mask(self, mask, **params):
         interpolation = 0   # refers to 'sitkNearestNeighbor'
-        return F.affine(mask,
+        return F.affine(np.expand_dims(mask, 0),
                         scales=self.scale,
                         interpolation=interpolation,
                         border_mode=self.mask_mode,
                         value=self.mval,
-                        spacing=self.spacing)
+                        spacing=self.spacing)[0]
 
     def apply_to_float_mask(self, mask, **params):
-        return F.affine(mask,
+        return F.affine(np.expand_dims(mask, 0),
                         scales=self.scale,
                         interpolation=self.interpolation,
                         border_mode=self.mask_mode,
                         value=self.mval,
-                        spacing=self.spacing)
+                        spacing=self.spacing)[0]
 
     def __repr__(self):
         return f'Scale({self.scale}, {self.interpolation}, {self.border_mode}, {self.ival}, {self.mval},' \
                f'{self.always_apply}, {self.p})'
 
 
 # TODO cannot rescale T dimension
@@ -404,28 +404,28 @@
                         interpolation=self.interpolation,
                         border_mode=self.border_mode,
                         value=self.ival,
                         spacing=self.spacing)
 
     def apply_to_mask(self, mask, **params):
         interpolation = 0   # refers to 'sitkNearestNeighbor'
-        return F.affine(mask,
+        return F.affine(np.expand_dims(mask, 0),
                         scales=params["scale"],
                         interpolation=interpolation,
                         border_mode=self.mask_mode,
                         value=self.mval,
-                        spacing=self.spacing)
+                        spacing=self.spacing)[0]
 
     def apply_to_float_mask(self, mask, **params):
-        return F.affine(mask,
+        return F.affine(np.expand_dims(mask, 0),
                         scales=params["scale"],
                         interpolation=self.interpolation,
                         border_mode=self.mask_mode,
                         value=self.mval,
-                        spacing=self.spacing)
+                        spacing=self.spacing)[0]
 
     def __repr__(self):
         return f'RandomScale({self.scaling_limit}, {self.interpolation}, {self.always_apply}, {self.p})'
 
 
 class RandomRotate90(DualTransform):
     """Rotation of input by 0, 90, 180, or 270 degrees around the specified spatial axes.
@@ -553,34 +553,29 @@
                 Defaults to ``0.5``.
 
         Targets:
             image, mask, float_mask
     """
     def __init__(self, axes_to_choose: Union[None, List[Tuple[int]]] = None, always_apply=False, p=0.5):
         super().__init__(always_apply, p)
+
+        # TODO: check if axis are valid
         self.axes = axes_to_choose
 
     def apply(self, img, **params):
         return np.flip(img, params["axes"])
 
     def apply_to_mask(self, mask, **params):
         # Mask has no dimension channel
         return np.flip(mask, axis=[item - 1 for item in params["axes"]])
 
     def get_params(self, **data):
         
-        if self.axes is None or len(self.axes) == 0:
-            # Pick random combination of axes to flip
-            # TODO include possibility to pick empty combination = no flipping
-            combinations = [(1,), (2,), (3,), (1, 2),
-                            (1, 3), (2, 3), (1, 2, 3)]
-            axes = random.choice(combinations)
-        else:
-            # Pick a random choice from input
-            axes = random.choice(self.axes)
+        to_choose = [1, 2, 3] if self.axes is None else self.axes
+        axes = random.sample(to_choose, random.randint(0, len(to_choose)))
         return {"axes": axes}
 
     def __repr__(self):
         return f'Flip({self.axes}, {self.always_apply}, {self.p})'
 
 
 class CenterCrop(DualTransform):
@@ -795,16 +790,16 @@
             p (float, optional): Chance of applying this transformation in composition. 
             
                 Defaults to ``0.5``.
 
         Targets:
             image, mask, float_mask
     """
-    def __init__(self, angle_limit: Union[float, TypePairFloat, TypeSextetFloat] = (15, 15, 15),
-                 translation_limit: Union[float, TypePairFloat, TypeSextetFloat] = (0, 0, 0),
+    def __init__(self, angle_limit: Union[float, TypePairFloat, TypeSextetFloat] = (15., 15., 15.),
+                 translation_limit: Union[float, TypePairFloat, TypeSextetFloat] = (0., 0., 0.),
                  scaling_limit: Union[float, TypePairFloat, TypeSextetFloat] = (0.2, 0.2, 0.2),
                  spacing: Union[float, TypeTripletFloat] = None,
                  change_to_isotropic: bool = False,
                  interpolation: int = 1,
                  border_mode: str = 'constant', ival: float = 0, mval: float = 0,
                  ignore_index: Union[float, None] = None, always_apply: bool = False, p: float = 0.5):
         super().__init__(always_apply, p)
@@ -831,32 +826,32 @@
                         interpolation=self.interpolation,
                         border_mode=self.border_mode,
                         value=self.ival,
                         spacing=self.spacing)
 
     def apply_to_mask(self, mask, **params):
         interpolation = 0   # refers to 'sitkNearestNeighbor'
-        return F.affine(mask,
+        return F.affine(np.expand_dims(mask, 0),
                         scales=params["scale"],
                         degrees=params["angles"],
                         translation=params["translation"],
                         interpolation=interpolation,
                         border_mode=self.mask_mode,
                         value=self.mval,
-                        spacing=self.spacing)
+                        spacing=self.spacing)[0]
 
     def apply_to_float_mask(self, mask, **params):
-        return F.affine(mask,
+        return F.affine(np.expand_dims(mask, 0),
                         scales=params["scale"],
                         degrees=params["angles"],
                         translation=params["translation"],
                         interpolation=self.interpolation,
                         border_mode=self.mask_mode,
                         value=self.mval,
-                        spacing=self.spacing)
+                        spacing=self.spacing)[0]
 
     def get_params(self, **data):
 
         # set parameters of the transform
         scales = sample_range_uniform(self.scaling_limit)
         angles = sample_range_uniform(self.angle_limit)
         translation = sample_range_uniform(self.translation_limit)
@@ -955,32 +950,32 @@
                         interpolation=self.interpolation,
                         border_mode=self.border_mode,
                         value=self.ival,
                         spacing=self.spacing)
 
     def apply_to_mask(self, mask, **params):
         interpolation = 0   # refers to 'sitkNearestNeighbor'
-        return F.affine(mask,
+        return F.affine(np.expand_dims(mask, 0),
                         scales=self.scale,
                         degrees=self.angles,
                         translation=self.translation,
                         interpolation=interpolation,
                         border_mode=self.mask_mode,
                         value=self.mval,
-                        spacing=self.spacing)
+                        spacing=self.spacing)[0]
 
     def apply_to_float_mask(self, mask, **params):
-        return F.affine(mask,
+        return F.affine(np.expand_dims(mask, 0),
                         scales=self.scale,
                         degrees=self.angles,
                         translation=self.translation,
                         interpolation=self.interpolation,
                         border_mode=self.mask_mode,
                         value=self.mval,
-                        spacing=self.spacing)
+                        spacing=self.spacing)[0]
 
 
 # TODO create checks (mean, std, got good shape, and etc.), what if given list but only one channel, and reverse.
 class NormalizeMeanStd(ImageOnlyTransform):
     """Normalize image values to have mean 0 and standard deviation 1, given channel-wise means and standard deviations.
 
         For a single-channel image, the normalization is applied by the formula: :math:`img = (img - mean) / std`.
```

### Comparing `bio_volumentations-1.1.2/bio_volumentations/augmentations/utils.py` & `bio_volumentations-1.2.0/bio_volumentations/augmentations/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 #  AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER                       #
 #  LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,                #
 #  OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE                #
 #  SOFTWARE.                                                                                    #
 # ============================================================================================= #
 
 from typing import Sequence, Union
-from ..typing import TypeSextetFloat, TypeTripletFloat, TypePairFloat
+from ..biovol_typing import TypeSextetFloat, TypeTripletFloat, TypePairFloat
 import numpy as np
 import SimpleITK as sitk
 
 from collections.abc import Iterable
 
 
 def parse_limits(input_limit: Union[float, TypePairFloat, TypeTripletFloat, TypeSextetFloat],
@@ -37,15 +37,15 @@
     # input_limit = None
     # returns (ie, ie, ie, ie, ie, ie)
     if input_limit is None:
         return tuple((identity_element, ) * 6)
 
     # input_limit = x : float
     # returns (ie-x, ie+x, ie-x, ie+x, ie-x, ie+x)
-    elif len(input_limit) == 1:
+    elif (type(input_limit) is float) or (type(input_limit) is int):
         return tuple((identity_element - input_limit, identity_element + input_limit) * 3)
 
     # input_limit = (a, b) : TypePairFloat
     # returns (a, b, a, b, a, b)
     elif len(input_limit) == 2:
         a, b = input_limit
         return a, b, a, b, a, b
@@ -91,18 +91,16 @@
 def get_image_center(image: np.array,
                      spacing: TypeTripletFloat = (1., 1., 1.),
                      lps: bool = False) -> TypeTripletFloat:
 
     shape = np.array(image.shape)
     if len(shape) == 3:
         center = (shape - 1) / 2
-    elif len(shape) == 4:
-        center = (shape[1:4] - 1) / 2
     else:
-        center = np.array((0, 0, 0))
+        center = (shape[1:4] - 1) / 2
 
     if lps:
         center = ras_to_lps(center)
 
     return center * np.array(spacing)
```

### Comparing `bio_volumentations-1.1.2/bio_volumentations/conversion/__init__.py` & `bio_volumentations-1.2.0/bio_volumentations/conversion/__init__.py`

 * *Files identical despite different names*

### Comparing `bio_volumentations-1.1.2/bio_volumentations/conversion/functional.py` & `bio_volumentations-1.2.0/bio_volumentations/conversion/functional.py`

 * *Files identical despite different names*

### Comparing `bio_volumentations-1.1.2/bio_volumentations/conversion/transforms.py` & `bio_volumentations-1.2.0/bio_volumentations/conversion/transforms.py`

 * *Files identical despite different names*

### Comparing `bio_volumentations-1.1.2/bio_volumentations/core/__init__.py` & `bio_volumentations-1.2.0/bio_volumentations/core/__init__.py`

 * *Files identical despite different names*

### Comparing `bio_volumentations-1.1.2/bio_volumentations/core/composition.py` & `bio_volumentations-1.2.0/bio_volumentations/core/composition.py`

 * *Files identical despite different names*

### Comparing `bio_volumentations-1.1.2/bio_volumentations/core/transforms_interface.py` & `bio_volumentations-1.2.0/bio_volumentations/core/transforms_interface.py`

 * *Files identical despite different names*

### Comparing `bio_volumentations-1.1.2/bio_volumentations/random_utils.py` & `bio_volumentations-1.2.0/bio_volumentations/random_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 #  LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,                #
 #  OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE                #
 #  SOFTWARE.                                                                                    #
 # ============================================================================================= #
 
 import numpy as np
 from typing import Optional, Sequence, Union, Type, Any
-from .typing import TypeSextetFloat, TypeTripletFloat
+from .biovol_typing import TypeSextetFloat, TypeTripletFloat
 import random as random
 
 NumType = Union[int, float, np.ndarray]
 IntNumType = Union[int, np.ndarray]
 Size = Union[int, Sequence[int]]
```

### Comparing `bio_volumentations-1.1.2/bio_volumentations/typing.py` & `bio_volumentations-1.2.0/bio_volumentations/biovol_typing.py`

 * *Files identical despite different names*

### Comparing `bio_volumentations-1.1.2/bio_volumentations.egg-info/PKG-INFO` & `bio_volumentations-1.2.0/bio_volumentations.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: bio-volumentations
-Version: 1.1.2
-Summary: Library for 3D-5D augmentations of volumetric multi-dimensional biomedical images
+Version: 1.2.0
+Summary: Library for 3D-5D augmentations of volumetric multi-dimensional biomedical images and their annotations
 Author: Lucia Hradecká, Filip Lux, Samuel Šuľan
 Author-email: Lucia Hradecká <lucia.d.hradecka@gmail.com>, Filip Lux <lux.filip@gmail.com>
 License: MIT License
-Project-URL: Homepage, https://gitlab.fi.muni.cz/cbia/bio-volumentations/-/tree/v1-1-0?ref_type=heads
-Project-URL: Documentation, https://biovolumentations.readthedocs.io/v1-1-2/
-Project-URL: Repository, https://gitlab.fi.muni.cz/cbia/bio-volumentations/-/tree/v1-1-0?ref_type=heads
+Project-URL: Homepage, https://gitlab.fi.muni.cz/cbia/bio-volumentations/-/tree/1.2.0?ref_type=tags
+Project-URL: Documentation, https://biovolumentations.readthedocs.io/1.2.0/
+Project-URL: Repository, https://gitlab.fi.muni.cz/cbia/bio-volumentations/-/tree/1.2.0?ref_type=tags
 Keywords: image,augmentation,3D,volumetric,biomedical,bioimage,preprocessing,transformation
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.1
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -19,192 +19,262 @@
 Requires-Dist: scipy
 Requires-Dist: scikit-image
 Requires-Dist: matplotlib
 Requires-Dist: SimpleITK
 
 # Bio-Volumentations
 
-`Bio-Volumentations` is an image augmentation and preprocessing package for 3D, 4D, and 5D biomedical images.
+`Bio-Volumentations` is an image augmentation and preprocessing package for 3D (volumetric), 
+4D (time-lapse volumetric or multi-channel volumetric), and 5D (time-lapse multi-channel volumetric) 
+biomedical images and their annotations.
 
-It offers a range of image transformations implemented efficiently for time-lapse multi-channel volumetric image data.
+The library offers a wide range of efficiently implemented image transformations.
 This includes both preprocessing transformations (such as intensity normalisation, padding, and type casting) 
 and augmentation transformations (such as affine transform, noise addition and removal, and contrast manipulation).
 
-The `Bio-Volumentations` library is a suitable tool for data manipulation in machine learning applications. 
+The `Bio-Volumentations` library is a suitable tool for image manipulation in machine learning applications. 
 It can be used with any major Python deep learning library, including PyTorch, PyTorch Lightning, TensorFlow, and Keras.
 
-This library builds upon wide-spread libraries such as Albumentations (see the Contributions section below) 
-in terms of design and user interface. Therefore, it can easily be adopted by developers.
+This library builds upon wide-spread libraries such as Albumentations and TorchIO (see the Contributions section below). 
+Therefore, it can easily be adopted by developers.
 
 # Installation
 
 Install the package from pip using:
 ```python
 pip install bio-volumentations
 ```
+
+See [the project's PyPi page](https://pypi.org/project/bio-volumentations/) for more details.
+
 ## Requirements
 
-NumPy       https://numpy.org/ <br> 
-SciPy       https://scipy.org/ <br>
-Scikit-image https://scikit-image.org/ <br>
-Matplotlib  https://matplotlib.org/ <br>
-SimpleITK   https://simpleitk.org/ <br>
+- [NumPy](https://numpy.org/)
+- [SciPy](https://scipy.org/)
+- [Scikit-image](https://scikit-image.org/)
+- [Matplotlib](https://matplotlib.org/)
+- [SimpleITK](https://simpleitk.org/)
 
 
 # Usage
 
 ### Importing
 
 Import the library to your project using:
 ```python
 import bio_volumentations as biovol
 ```
 
 ### How to Use Bio-Volumentations?
 
-The Bio-Volumentations library processes 3D, 4D, and 5D images. Each image must be 
-represented as `numpy.ndarray`s and must conform  to the following conventions:
+The `Bio-Volumentations` library processes 3D, 4D, and 5D images. Each image must be 
+represented as a `numpy.ndarray` and must conform to the following conventions:
 
 - The order of dimensions is [C, Z, Y, X, T], where C is the channel dimension, 
    T is the time dimension, and Z, Y, and X are the spatial dimensions.
-- The three spatial dimensions (Z, Y, X) are compulsory.
+- The three spatial dimensions (Z, Y, X) must be present. To transform a 2D image, please create a dummy Z dimension first. 
 - The channel (C) dimension is optional. If it is not present, the library will automatically
-   create a dummy dimension in its place and output an image of shape (1, Z, Y, X).
+   create a dummy dimension in its place, so the output image shape will be [1, Z, Y, X].
 - The time (T) dimension is optional and can only be present if the channel (C) dimension is 
-   also present.
+   also present in the input data. To process single-channel time-lapse images, please create a dummy C dimension first.
+
+Thus, an input image is interpreted in the following ways based on its shape:
+
+1. [Z, Y, X] ... a single-channel volumetric image;
+2. [C, Z, Y, X] ... a multi-channel volumetric image;
+3. [C, Z, Y, X, T] ... a single-channel as well as multi-channel volumetric image sequence.
+
+The shape of the output image is either [C, Z, Y, X] (cases 1 & 2) or [C, Z, Y, X, T] (case 3).
 
-Thus, the input images can have these shapes:
+The images are type-casted to a floating-point datatype before transformations, irrespective of their actual datatype.
 
-- [Z, Y, X] (a single-channel volumetric image)
-- [C, Z, Y, X] (a multi-channel volumetric image)
-- [C, Z, Y, X, T] (a single-channel as well as multi-channel volumetric image sequence)
+For the specification of image annotation conventions, please see below.
 
-**It is strongly recommended to use `Compose` to create and use transformation pipelines.** 
+**It is strongly recommended to use `Compose` to create and use transformation pipelines.** <br>
 The `Compose` class automatically checks and adjusts image format, datatype, stacks
 individual transforms to a pipeline, and outputs the image as a contiguous array. 
-Optionally, it can also convert the transformed image to a desired format.
+Optionally, it can also convert the transformed image to a desired format. <br>
+If you call transformations outside of `Compose`, we cannot guarantee the all assumptions are checked and enforced, 
+so you might encounter unexpected behaviour.
 
-More at the [documentation pages](https://www.google.com).
-
-Below, there are several examples of how to use this library.
+Below, there are several examples of how to use this library. You are also welcome to check 
+[our documentation pages](https://biovolumentations.readthedocs.io/1.2.0/).
 
 ### Example: Transforming a Single Image
 
+To create the transformation pipeline, you just need to instantiate all desired transformations
+(with the desired parameter values)
+and then feed a list of these transformations into a new `Compose` object. 
+
+Optionally, you can specify a datatype conversion transformation that will be applied after the last transformation
+in the list, e.g. from the default `numpy.ndarray` to a `torch.Tensor`. You can also specify the probability
+of actually applying the whole pipeline as a number between 0 and 1. The default probability is 1 (always apply).
+See the [docs](https://biovolumentations.readthedocs.io/1.2.0/) for more details.
+
+The `Compose` object is callable. The data is passed as a keyword argument, and the call returns a dictionary 
+with the same keywords and corresponding transformed images. This might look like an overkill for a single image, 
+but will come handy when transforming images with annotations. The default key for the image is `image`.
+
+
 ```python
 import numpy as np
 from bio_volumentations import Compose, RandomGamma, RandomRotate90, GaussianBlur
 
-# Create the transformation using Compose from a list of transformations
+# Create the transformation pipeline using Compose
 aug = Compose([
         RandomGamma(gamma_limit = (0.8, 1,2), p = 0.8),
         RandomRotate90(axes = [1, 2, 3], p = 1),
         GaussianBlur(sigma = 1.2, p = 0.8)
       ])
 
-# Generate an image 
+# Generate an image - shape [C, Z, Y, X]
 img = np.random.rand(1, 128, 256, 256)
 
 # Transform the image
-# Notice that the image must be passed as a keyword argument to the transformation pipeline
+# Please note that the image must be passed as a keyword argument to the transformation pipeline
 # and extracted from the outputted dictionary.
 data = {'image': img}
 aug_data = aug(**data)
 transformed_img = aug_data['image']
 ```
 
 ### Example: Transforming Image Tuples
 
 Sometimes, it is necessary to consistently transform a tuple of corresponding images.
-To that end, Bio-Volumentations define several target types:
+To that end, `Bio-Volumentations` define several target types:
 
-- `image` for the image data;
-- `mask` for integer-valued label images; and
-- `float_mask` for real-valued label images.
+- `image` for the image data (any datatype allowed, gets converted to floating-point by default);
+- `mask` for integer-valued label images (expected integer datatype); and
+- `float_mask` for real-valued label images (expected floating-point datatype).
 
 The `mask` and `float_mask` target types are expected to have the same shape as the `image`
 target except for the channel (C) dimension which must not be included. 
-For example, for images of shape (150, 300, 300), (1, 150, 300, 300), or
-(4, 150, 300, 300), the corresponding `mask` must be of shape (150, 300, 300).
-If one wants to use a multichannel `mask` or `float_mask`, one has to split it into
+For example, for images of shape [150, 300, 300], [1, 150, 300, 300], and
+[4, 150, 300, 300], the corresponding `mask` and `float_mask` must be of shape [150, 300, 300].
+If you want to use a multichannel `mask` or `float_mask`, you have to split it into
 a set of single-channel `mask`s or `float_mask`s, respectively, and input them
 as stand-alone targets (see below).
 
 If a `Random...` transform receives multiple targets on its input in a single call,
-the same random numbers are used to transform all of these targets.
+the same transformation parameters are used to transform all of these targets.
+For example, `RandomAffineTransform` applies the same geometric transformation to all target types in a single call.
+
+Some transformations, such as `RandomGaussianNoise` or `RandomGamma`, are only defined for the `image` target 
+and leave the `mask` and `float_mask` targets unchanged. Please consult the 
+[documentation of the individual transforms](https://biovolumentations.readthedocs.io/1.2.0/) for more details.
 
-However, some transformations might behave slightly differently for the individual
-target types. For example, `RandomCrop` works in the same way for all target types, while
-`RandomGaussianNoise` only affects the `image` target and leaves the `mask` and
-`float_mask` targets unchanged. Please consult the documentation of respective transforms
-for more details.
+The image tuples are fed to the `Compose` object call as keyword arguments and extracted from the outputted dictionary
+using the same keys. The default key values are `image`, `mask`, and `float_mask`.
 
 ```python
 import numpy as np
 from bio_volumentations import Compose, RandomGamma, RandomRotate90, GaussianBlur
 
-# Create the transformation using Compose from a list of transformations
+# Create the transformation using Compose
 aug = Compose([
         RandomGamma(gamma_limit = (0.8, 1,2), p = 0.8),
         RandomRotate90(axes = [1, 2, 3], p = 1),
         GaussianBlur(sigma = 1.2, p = 0.8)
       ])
 
 # Generate image and a corresponding labeled image
 img = np.random.rand(1, 128, 256, 256)
 lbl = np.random.randint(0, 1, size=(128, 256, 256), dtype=np.uint8)
 
 # Transform the images
-# Notice that the images must be passed as keyword arguments to the transformation pipeline
+# Please note that the images must be passed as keyword arguments to the transformation pipeline
 # and extracted from the outputted dictionary.
 data = {'image': img, 'mask': lbl}
 aug_data = aug(**data)
 transformed_img, transformed_lbl = aug_data['image'], aug_data['mask']
 ```
 
 
 ### Example: Transforming Multiple Images of the Same Target Type
 
-Although there are only three target types, one input arbitrary number of images to any
-transformation. To achieve this, one has to define the value of the `targets` argument
+Although there are only three target types, you can input an arbitrary number of images to any
+transformation. To achieve this, you have to define the value of the `targets` argument
 when creating a `Compose` object.
 
-`targets` must be a list with 3 items: a list with names of `image`-type targets, 
-a list with names of `mask`-type targets, and 
-a list with names of `float_mask`-type targets. The specified names will then be used 
-to input the images to the transformation call as well as during extracting the
-transformed images from the outputted dictionary. Please see the code below 
-for a practical example.
+The value of `targets` must be a list with exactly 3 items: a list with keys of `image`-type targets, 
+a list with keys of `mask`-type targets, and 
+a list with keys of `float_mask`-type targets. 
+The specified keys will then be used to input the images to the transformation call as well as to extract the
+transformed images from the outputted dictionary. 
+
+The keys can be any valid dictionary keys; most importantly, they must be unique across all target types.
+You don't need to feed an image for each target to the transformation call: in our example below, we have four targets
+(two `image`, one `mask`, and one `float_mask`), but we only transform three images.
+
+You cannot define your own target types; that would require re-implementing all existing transforms.
 
 ```python
 import numpy as np
 from bio_volumentations import Compose, RandomGamma, RandomRotate90, GaussianBlur
 
-# Create the transformation using Compose from a list of transformations and define targets
+# Create the transformation using Compose: do not forget to define targets
 aug = Compose([
         RandomGamma( gamma_limit = (0.8, 1,2), p = 0.8),
         RandomRotate90(axes = [1, 2, 3], p = 1),
         GaussianBlur(sigma = 1.2, p = 0.8)
     ], 
     targets= [ ['image' , 'image1'] , ['mask'], ['float_mask'] ])
 
-# Generate the image data
+# Generate the image data: two images and a single int-valued mask
 img = np.random.rand(1, 128, 256, 256)
 img1 = np.random.rand(1, 128, 256, 256)
 lbl = np.random.randint(0, 1, size=(128, 256, 256), dtype=np.uint8)
 
 # Transform the images
-# Notice that the images must be passed as keyword arguments to the transformation pipeline
+# Please note that the images must be passed as keyword arguments to the transformation pipeline
 # and extracted from the outputted dictionary.
 data = {'image': img, 'image1': img1, 'mask': lbl}
 aug_data = aug(**data)
 transformed_img = aug_data['image']
 transformed_img1 = aug_data['image1']
 transformed_lbl = aug_data['mask']
 ```
 
+### Example: Adding a Custom Transformation
+
+Each transformation inherits from the `Transform` class. You can thus easily implement your own 
+transformations and use them with this library. You can check our implementations to see how this can be done.
+For example, `Flip` can be implemented as follows:
+
+```python
+import numpy as np
+from typing import List
+from bio_volumentations import DualTransform
+
+class Flip(DualTransform):
+    def __init__(self, axes: List[int] = None, always_apply=False, p=1):
+        super().__init__(always_apply, p)
+        self.axes = axes
+
+    # Transform the image
+    def apply(self, img, **params):
+        return np.flip(img, params["axes"])
+
+    # Transform the int-valued mask
+    def apply_to_mask(self, mask, **params):
+       # The mask has no channels
+        return np.flip(mask, axis=[item - 1 for item in params["axes"]])
+    
+    # Transform the float-valued mask
+    # By default, float_mask uses the implementation of mask, unless it is overridden (see the implementation of DualTransform).
+    #def apply_to_float_mask(self, float_mask, **params):
+    #    return self.apply_to_mask(float_mask, **params)
+
+    # Get transformation parameters. Useful especially for RandomXXX transforms to ensure consistent transformation of image tuples.
+    def get_params(self, **data):
+        axes = self.axes if self.axes is not None else [1, 2, 3]
+        return {"axes": axes}
+```
+
+
 # Implemented Transforms
 
 ### A List of Implemented Transformations
 
 Point transformations:
 ```python
 GaussianNoise 
@@ -243,26 +313,25 @@
 # Contributions
 
 Authors of the Bio-Volumentations library: Samuel Šuľan, Lucia Hradecká, Filip Lux.
 - Lucia Hradecká: lucia.d.hradecka@gmail.com   
 - Filip Lux: lux.filip@gmail.com     
 
 The Bio-Volumentations library is based on the following image augmentation libraries:
-- Albumentations:           https://github.com/albumentations-team/albumentations       
-- 3D Conversion:            https://github.com/ashawkey/volumentations                  
-- Continued Development:    https://github.com/ZFTurbo/volumentations                   
-- Enhancements:             https://github.com/qubvel/volumentations                    
-- Further Enhancements:     https://github.com/muellerdo/volumentations     
-
-We would thus like to thank their authors, namely:
-- The Albumentations team: https://github.com/albumentations-team                    
-- Pavel Iakubovskii: https://github.com/qubvel                                 
-- ZFTurbo: https://github.com/ZFTurbo                                
-- ashawkey: https://github.com/ashawkey                               
-- Dominik Müller: https://github.com/muellerdo         
+- [Albumentations](https://github.com/albumentations-team/albumentations)  
+- [Volumentations](https://github.com/ashawkey/volumentations)                  
+- [Volumentations: Continued Development](https://github.com/ZFTurbo/volumentations)                   
+- [Volumentations: Enhancements](https://github.com/qubvel/volumentations)        
+- [Volumentations: Further Enhancements](https://github.com/muellerdo/volumentations)
+- [TorchIO](https://github.com/fepegar/torchio)
+
+We would thus like to thank their authors, namely [the Albumentations team](https://github.com/albumentations-team), 
+[Pavel Iakubovskii](https://github.com/qubvel), [ZFTurbo](https://github.com/ZFTurbo), 
+[ashawkey](https://github.com/ashawkey), [Dominik Müller](https://github.com/muellerdo), and 
+[TorchIO contributors](https://github.com/fepegar/torchio?tab=readme-ov-file#contributors).         
 
 
 # Citation
 
 TBA
```

### Comparing `bio_volumentations-1.1.2/bio_volumentations.egg-info/SOURCES.txt` & `bio_volumentations-1.2.0/bio_volumentations.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 LICENSE
 README.md
 pyproject.toml
 bio_volumentations/__init__.py
+bio_volumentations/biovol_typing.py
 bio_volumentations/random_utils.py
-bio_volumentations/typing.py
 bio_volumentations.egg-info/PKG-INFO
 bio_volumentations.egg-info/SOURCES.txt
 bio_volumentations.egg-info/dependency_links.txt
 bio_volumentations.egg-info/requires.txt
 bio_volumentations.egg-info/top_level.txt
 bio_volumentations/augmentations/__init__.py
 bio_volumentations/augmentations/functional.py
```

### Comparing `bio_volumentations-1.1.2/pyproject.toml` & `bio_volumentations-1.2.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 
 [project]
 # Put the name of your project on PyPI.
 name = "bio-volumentations"
 
 # Put the version of your project. This field is required, although it is often marked as dynamic:
-version = "1.1.2"
+version = "1.2.0"
 #dynamic = ["version"]
 # https://stackoverflow.com/questions/21064581/how-to-overwrite-pypi-package-when-doing-upload-from-command-line
 
 # If your project has dependencies, list them like this:
 dependencies = [
   "numpy",
   "scipy",
@@ -35,15 +35,15 @@
   {name = "Filip Lux", email = "lux.filip@gmail.com"},
   {name = "Samuel Šuľan"},
 ]
 # Optionally, can also include the maintainers field
 
 # A one-line description of your project, to show as the “headline” of your project page on PyPI
 # and other places such as lists of search results:
-description = "Library for 3D-5D augmentations of volumetric multi-dimensional biomedical images"
+description = "Library for 3D-5D augmentations of volumetric multi-dimensional biomedical images and their annotations"
 
 # A longer description - can use readme.md
 readme = "README.md"
 
 # Lincense - two possibilities
 #license = {file = "LICENSE"}
 license = {text = "MIT License"}
@@ -58,18 +58,10 @@
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 # A list of URLs associated with your project, displayed on the left sidebar of your PyPI project page.
 [project.urls]
-Homepage = "https://gitlab.fi.muni.cz/cbia/bio-volumentations/-/tree/v1-1-0?ref_type=heads"
-Documentation = "https://biovolumentations.readthedocs.io/v1-1-2/"
-Repository = "https://gitlab.fi.muni.cz/cbia/bio-volumentations/-/tree/v1-1-0?ref_type=heads"
-
-# MISSING FROM SETUP.PY
-# entry_points={
-#        'console_scripts': [
-#            'bioVolumentation=bio_volumentations:__init__'
-#        ]
-#    }
-# packages=setuptools.find_packages()
+Homepage = "https://gitlab.fi.muni.cz/cbia/bio-volumentations/-/tree/1.2.0?ref_type=tags"
+Documentation = "https://biovolumentations.readthedocs.io/1.2.0/"
+Repository = "https://gitlab.fi.muni.cz/cbia/bio-volumentations/-/tree/1.2.0?ref_type=tags"
```

