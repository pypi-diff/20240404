# Comparing `tmp/botocore-a-la-carte-artifact-1.34.76.tar.gz` & `tmp/botocore_a_la_carte_artifact-1.34.77-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botocore-a-la-carte-artifact-1.34.76.tar", last modified: Wed Apr  3 00:59:02 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

