# Comparing `tmp/AppAuthN-0.0.15.tar.gz` & `tmp/AppAuthN-0.0.16-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AppAuthN-0.0.15.tar", last modified: Wed May  1 07:01:55 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

