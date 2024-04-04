# Comparing `tmp/simple-notifications-0.1.2.tar.gz` & `tmp/simple_notifications-0.1.3-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simple-notifications-0.1.2.tar", last modified: Sun Aug 13 08:44:32 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

