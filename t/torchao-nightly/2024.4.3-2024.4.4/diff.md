# Comparing `tmp/torchao-nightly-2024.4.3.tar.gz` & `tmp/torchao-nightly-2024.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torchao-nightly-2024.4.3.tar", last modified: Wed Apr  3 00:18:54 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

