# Comparing `tmp/chombopy-0.2.1.tar.gz` & `tmp/chombopy-1.0.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/chombopy-0.2.1.tar", last modified: Mon May  4 18:01:03 2020, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

