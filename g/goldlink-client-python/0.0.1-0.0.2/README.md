# Comparing `tmp/goldlink-client-python-0.0.1.tar.gz` & `tmp/goldlink_client_python-0.0.2-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "goldlink-client-python-0.0.1.tar", last modified: Thu May  2 21:48:49 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

