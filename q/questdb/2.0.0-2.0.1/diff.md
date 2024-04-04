# Comparing `tmp/questdb-2.0.0.tar.gz` & `tmp/questdb-2.0.1-cp311-cp311-manylinux_2_17_i686.manylinux2014_i686.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "questdb-2.0.0.tar", last modified: Tue Mar 19 15:04:43 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

