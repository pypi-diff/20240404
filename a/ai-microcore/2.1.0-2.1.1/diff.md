# Comparing `tmp/ai_microcore-2.1.0.tar.gz` & `tmp/ai_microcore-2.1.1-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ai_microcore-2.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```
