# Comparing `tmp/gamsapi-46.3.0.tar.gz` & `tmp/gamsapi-46.4.0-cp39-cp39-manylinux_2_17_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gamsapi-46.3.0.tar", last modified: Tue Mar 19 09:29:31 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

