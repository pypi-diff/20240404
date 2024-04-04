# Comparing `tmp/sunpy-5.1.1.tar.gz` & `tmp/sunpy-5.1.2-cp39-abi3-manylinux_2_17_x86_64.manylinux2014_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sunpy-5.1.1.tar", last modified: Sat Jan 13 03:20:02 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

