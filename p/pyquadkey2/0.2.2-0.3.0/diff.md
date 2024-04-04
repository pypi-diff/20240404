# Comparing `tmp/pyquadkey2-0.2.2.tar.gz` & `tmp/pyquadkey2-0.3.0-cp311-cp311-manylinux_2_5_x86_64.manylinux1_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyquadkey2-0.2.2.tar", last modified: Tue Jun 21 00:41:50 2022, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

