# Comparing `tmp/pymsis-0.8.0.tar.gz` & `tmp/pymsis-0.9.0-cp312-cp312-win_amd64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymsis-0.8.0.tar", last modified: Tue Oct  3 18:40:22 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

