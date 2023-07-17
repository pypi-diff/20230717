# Comparing `tmp/cshogi-0.6.1.tar.gz` & `tmp/cshogi-0.6.2-cp39-cp39-win_amd64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cshogi-0.6.1.tar", last modified: Sun Jul 16 15:49:55 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

