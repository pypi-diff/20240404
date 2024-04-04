# Comparing `tmp/flytekitplugins-openai-1.12.0b3.tar.gz` & `tmp/flytekitplugins_openai-1.12.0b4-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flytekitplugins-openai-1.12.0b3.tar", last modified: Tue Apr  2 21:31:35 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

