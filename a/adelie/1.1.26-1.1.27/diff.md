# Comparing `tmp/adelie-1.1.26.tar.gz` & `tmp/adelie-1.1.27-cp312-cp312-macosx_14_0_arm64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adelie-1.1.26.tar", last modified: Tue Apr  2 14:40:02 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

