# Comparing `tmp/mypy-boto3-b2bi-1.34.74.tar.gz` & `tmp/mypy_boto3_b2bi-1.34.78-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-b2bi-1.34.74.tar", last modified: Fri Mar 29 19:18:22 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

