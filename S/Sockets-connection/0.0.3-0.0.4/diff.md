# Comparing `tmp/Sockets_connection-0.0.3.tar.gz` & `tmp/Sockets_connection-0.0.4-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Sockets_connection-0.0.3.tar", last modified: Mon Jul 17 13:18:30 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

