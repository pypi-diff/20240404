# Comparing `tmp/pyserilog-0.1.1a4.tar.gz` & `tmp/pyserilog-0.2.0a1-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyserilog-0.1.1a4.tar", last modified: Sat Mar 30 07:05:49 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

