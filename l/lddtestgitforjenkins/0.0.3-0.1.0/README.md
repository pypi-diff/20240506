# Comparing `tmp/lddtestgitforjenkins-0.0.3.tar.gz` & `tmp/lddtestgitforjenkins-0.1.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lddtestgitforjenkins-0.0.3.tar", last modified: Wed Nov 22 07:59:47 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

