# Comparing `tmp/chiapos-2.0.0b4.tar.gz` & `tmp/chiapos-2.0.0b5-cp39-cp39-win_amd64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chiapos-2.0.0b4.tar", last modified: Wed Jul 12 23:36:44 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

