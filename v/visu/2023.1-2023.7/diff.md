# Comparing `tmp/visu-2023.1.tar.gz` & `tmp/visu-2023.7-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "visu-2023.1.tar", last modified: Fri Feb  3 15:40:51 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

