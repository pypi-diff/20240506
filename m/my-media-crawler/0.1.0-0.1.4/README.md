# Comparing `tmp/my_media_crawler-0.1.0.tar.gz` & `tmp/my_media_crawler-0.1.4-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "my_media_crawler-0.1.0.tar", last modified: Sat May  4 01:52:19 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

