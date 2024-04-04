# Comparing `tmp/honeyhive-0.1.89.tar.gz` & `tmp/honeyhive-0.1.90-py2.py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "honeyhive-0.1.89.tar", last modified: Sun Mar 17 03:39:20 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

