# Comparing `tmp/skll-3.2.0.tar.gz` & `tmp/skll-4.0.0.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skll-3.2.0.tar", last modified: Thu Jan 19 17:26:18 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

