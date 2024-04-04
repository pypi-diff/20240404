# Comparing `tmp/tablib-3.6.0.tar.gz` & `tmp/tablib-3.6.1-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tablib-3.6.0.tar", last modified: Sat Mar 23 11:06:04 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

