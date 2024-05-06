# Comparing `tmp/document_image_utils-0.1.4.tar.gz` & `tmp/document_image_utils-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "document_image_utils-0.1.4.tar", max compression
+gzip compressed data, was "document_image_utils-0.1.5.tar", max compression
```

## Comparing `document_image_utils-0.1.4.tar` & `document_image_utils-0.1.5.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0        0 2024-03-12 20:00:48.000000 document_image_utils-0.1.4/document_image_utils/__init__.py
--rw-r--r--   0        0        0    11476 2024-02-13 16:43:52.000000 document_image_utils-0.1.4/document_image_utils/box.py
--rw-r--r--   0        0        0    14320 2024-03-15 18:34:58.000000 document_image_utils-0.1.4/document_image_utils/image.py
--rw-r--r--   0        0        0      505 2024-03-15 18:35:14.000000 document_image_utils-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      879 2024-03-15 17:34:42.000000 document_image_utils-0.1.4/README.md
--rw-r--r--   0        0        0     1351 1970-01-01 00:00:00.000000 document_image_utils-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-03-12 20:00:48.000000 document_image_utils-0.1.5/document_image_utils/__init__.py
+-rw-r--r--   0        0        0    11476 2024-02-13 16:43:52.000000 document_image_utils-0.1.5/document_image_utils/box.py
+-rw-r--r--   0        0        0    14334 2024-05-06 15:28:38.146124 document_image_utils-0.1.5/document_image_utils/image.py
+-rw-r--r--   0        0        0      505 2024-05-06 15:58:10.894337 document_image_utils-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      879 2024-03-15 17:34:42.000000 document_image_utils-0.1.5/README.md
+-rw-r--r--   0        0        0     1351 1970-01-01 00:00:00.000000 document_image_utils-0.1.5/PKG-INFO
```

### Comparing `document_image_utils-0.1.4/document_image_utils/box.py` & `document_image_utils-0.1.5/document_image_utils/box.py`

 * *Files identical despite different names*

### Comparing `document_image_utils-0.1.4/document_image_utils/image.py` & `document_image_utils-0.1.5/document_image_utils/image.py`

 * *Files 1% similar despite different names*

```diff
@@ -376,15 +376,15 @@
     angle = math.degrees(math.atan((right_most_point[1] - left_most_point[1]) / (right_most_point[0] - left_most_point[0])))
 
     print('angle',angle)
 
     rotation_angle = 90 - abs(angle)
     if direction == 'counter_clockwise':
         rotation_angle = -rotation_angle
-    img = ndimage.rotate(og_img, rotation_angle)
+    img = ndimage.rotate(og_img, rotation_angle,reshape=False)
 
 
     ## test images
     if debug:
         cv2.imwrite(test_path + '_rotated.png', img)
 
         # draw points from set
```

### Comparing `document_image_utils-0.1.4/README.md` & `document_image_utils-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `document_image_utils-0.1.4/PKG-INFO` & `document_image_utils-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: document_image_utils
-Version: 0.1.4
+Version: 0.1.5
 Summary: Toolkit for document image processing
 Author: Gonçalo Afonso
 Author-email: brazafonso2001@gmail.com
 Requires-Python: >=3.10.11,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

