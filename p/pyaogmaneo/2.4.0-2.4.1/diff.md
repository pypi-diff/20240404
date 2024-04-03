# Comparing `tmp/pyaogmaneo-2.4.0.tar.gz` & `tmp/pyaogmaneo-2.4.1-cp312-cp312-musllinux_1_1_aarch64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyaogmaneo-2.4.0.tar", last modified: Tue Apr  2 17:13:30 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

