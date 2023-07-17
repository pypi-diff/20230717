# Comparing `tmp/lark-1.1.5.tar.gz` & `tmp/lark-1.1.6-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lark-1.1.5.tar", last modified: Tue Dec  6 12:50:11 2022, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

