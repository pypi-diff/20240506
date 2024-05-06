# Comparing `tmp/Test19991021-3.4.0.tar.gz` & `tmp/Test19991021-3.5.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Test19991021-3.4.0.tar", last modified: Sat May  4 14:39:57 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

