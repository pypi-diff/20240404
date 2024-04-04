# Comparing `tmp/tfds-nightly-4.9.4.dev202404030043.tar.gz` & `tmp/tfds_nightly-4.9.4.dev202404030044-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tfds-nightly-4.9.4.dev202404030043.tar", last modified: Wed Apr  3 00:44:00 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

