# Comparing `tmp/qtreemesh-0.0.1.tar.gz` & `tmp/qtreemesh-0.1.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qtreemesh-0.0.1.tar", last modified: Thu Jul  6 16:22:37 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

