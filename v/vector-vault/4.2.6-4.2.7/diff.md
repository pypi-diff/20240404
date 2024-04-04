# Comparing `tmp/vector_vault-4.2.6.tar.gz` & `tmp/vector_vault-4.2.7-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vector_vault-4.2.6.tar", last modified: Thu Apr  4 04:46:02 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

