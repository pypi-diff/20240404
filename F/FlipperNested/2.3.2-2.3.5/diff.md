# Comparing `tmp/FlipperNested-2.3.2.tar.gz` & `tmp/FlipperNested-2.3.5-cp311-cp311-win_amd64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FlipperNested-2.3.2.tar", last modified: Thu Oct  5 08:52:33 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

