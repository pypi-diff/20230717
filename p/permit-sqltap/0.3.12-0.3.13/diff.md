# Comparing `tmp/permit-sqltap-0.3.12.tar.gz` & `tmp/permit_sqltap-0.3.13-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "permit-sqltap-0.3.12.tar", last modified: Thu Mar 16 10:01:54 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

