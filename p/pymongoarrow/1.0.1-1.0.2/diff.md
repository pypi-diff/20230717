# Comparing `tmp/pymongoarrow-1.0.1.tar.gz` & `tmp/pymongoarrow-1.0.2-cp39-cp39-win_amd64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymongoarrow-1.0.1.tar", last modified: Thu Jun 22 20:58:51 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

