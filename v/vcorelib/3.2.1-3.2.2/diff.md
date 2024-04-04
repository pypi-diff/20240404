# Comparing `tmp/vcorelib-3.2.1.tar.gz` & `tmp/vcorelib-3.2.2-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vcorelib-3.2.1.tar", last modified: Thu Apr  4 03:28:57 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

