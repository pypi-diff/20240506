# Comparing `tmp/PennyLane_Lightning-0.35.1.tar.gz` & `tmp/PennyLane_Lightning-0.36.0-cp310-cp310-macosx_11_0_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PennyLane_Lightning-0.35.1.tar", last modified: Mon Mar 11 20:44:05 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

