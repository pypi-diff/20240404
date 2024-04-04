# Comparing `tmp/PAGETools-0.5.2.tar.gz` & `tmp/PAGETools-0.5.2a1-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PAGETools-0.5.2.tar", last modified: Thu Apr  4 09:39:39 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

