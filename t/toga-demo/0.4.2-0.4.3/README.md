# Comparing `tmp/toga-demo-0.4.2.tar.gz` & `tmp/toga_demo-0.4.3-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "toga-demo-0.4.2.tar", last modified: Tue Feb  6 05:53:57 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

