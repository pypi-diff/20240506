# Comparing `tmp/myqueue-24.1.0.tar.gz` & `tmp/myqueue-24.5.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "myqueue-24.1.0.tar", last modified: Tue Jan  2 13:19:09 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

