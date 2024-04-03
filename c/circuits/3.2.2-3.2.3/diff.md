# Comparing `tmp/circuits-3.2.2.tar.gz` & `tmp/circuits-3.2.3-py2.py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/circuits-3.2.2.tar", last modified: Tue Oct 19 16:25:00 2021, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

