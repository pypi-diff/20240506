# Comparing `tmp/jlrpy-1.7.0.tar.gz` & `tmp/jlrpy-1.7.1-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jlrpy-1.7.0.tar", last modified: Wed Mar 20 20:13:24 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

