# Comparing `tmp/pytexexam-3.0.tar.gz` & `tmp/pytexexam-3.0.1-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytexexam-3.0.tar", last modified: Mon Feb 12 07:49:35 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

