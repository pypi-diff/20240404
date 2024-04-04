# Comparing `tmp/trc-data-reader-0.2.0.tar.gz` & `tmp/trc_data_reader-0.3.2-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trc-data-reader-0.2.0.tar", last modified: Thu Nov 25 15:07:28 2021, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

