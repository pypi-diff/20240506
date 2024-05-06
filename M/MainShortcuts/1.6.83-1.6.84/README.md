# Comparing `tmp/mainshortcuts-1.6.83.tar.gz` & `tmp/mainshortcuts-1.6.84-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mainshortcuts-1.6.83.tar", max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

