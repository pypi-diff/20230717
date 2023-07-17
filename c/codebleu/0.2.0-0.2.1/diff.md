# Comparing `tmp/codebleu-0.2.0.tar.gz` & `tmp/codebleu-0.2.1-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codebleu-0.2.0.tar", last modified: Wed Jul 12 12:42:20 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

