# Comparing `tmp/python-gemini-api-2.4.1.tar.gz` & `tmp/python_gemini_api-2.4.2-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-gemini-api-2.4.1.tar", last modified: Fri Mar 29 00:27:50 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

