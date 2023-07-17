# Comparing `tmp/px_recount-3.11.0rc2.tar.gz` & `tmp/px_recount-3.11.0rc3.tar.gz`

## Comparing `px_recount-3.11.0rc2.tar` & `px_recount-3.11.0rc3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      477 1970-01-01 00:00:00.000000 px_recount-3.11.0rc2/Cargo.toml
--rw-r--r--   0     1001      123      685 2023-07-16 22:48:51.000000 px_recount-3.11.0rc2/.gitignore
--rw-r--r--   0     1001      123    30523 2023-07-16 22:48:51.000000 px_recount-3.11.0rc2/Cargo.lock
--rw-r--r--   0     1001      123      557 2023-07-16 22:48:51.000000 px_recount-3.11.0rc2/pyproject.toml
--rw-r--r--   0     1001      123     7758 2023-07-16 22:48:51.000000 px_recount-3.11.0rc2/src/main.rs
--rw-r--r--   0        0        0      619 1970-01-01 00:00:00.000000 px_recount-3.11.0rc2/PKG-INFO
+-rw-r--r--   0        0        0      477 1970-01-01 00:00:00.000000 px_recount-3.11.0rc3/Cargo.toml
+-rw-r--r--   0     1001      123      685 2023-07-17 00:54:40.000000 px_recount-3.11.0rc3/.gitignore
+-rw-r--r--   0     1001      123    30523 2023-07-17 00:54:45.000000 px_recount-3.11.0rc3/Cargo.lock
+-rw-r--r--   0     1001      123      557 2023-07-17 00:54:40.000000 px_recount-3.11.0rc3/pyproject.toml
+-rw-r--r--   0     1001      123     7686 2023-07-17 00:54:40.000000 px_recount-3.11.0rc3/src/main.rs
+-rw-r--r--   0        0        0      619 1970-01-01 00:00:00.000000 px_recount-3.11.0rc3/PKG-INFO
```

### Comparing `px_recount-3.11.0rc2/.gitignore` & `px_recount-3.11.0rc3/.gitignore`

 * *Files identical despite different names*

### Comparing `px_recount-3.11.0rc2/Cargo.lock` & `px_recount-3.11.0rc3/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -704,15 +704,15 @@
 checksum = "78803b62cbf1f46fde80d7c0e803111524b9877184cfe7c3033659490ac7a7da"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "px-recount"
-version = "3.11.0-rc2"
+version = "3.11.0-rc3"
 dependencies = [
  "anyhow",
  "dicom",
  "redis 0.23.0",
  "redis-derive",
  "time 0.3.23",
 ]
```

### Comparing `px_recount-3.11.0rc2/pyproject.toml` & `px_recount-3.11.0rc3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `px_recount-3.11.0rc2/src/main.rs` & `px_recount-3.11.0rc3/src/main.rs`

 * *Files 0% similar despite different names*

```diff
@@ -122,33 +122,31 @@
         series_key_of(dcm).with_context(|| format!("Could not read DICOM tags of {:?}", &dcm))?;
 
     let mut client = redis::Client::open(get_redis_url()?)?;
 
     let is_last = redis::transaction(&mut client, &[&series_key], |con, pipe| {
         let data: ReData = con.hgetall(&series_key)?;
         let new_count = data.fileCounter + 1;
+        pipe.hset(&series_key, "fileCounter", new_count)
+            .ignore()
+            .hset(&series_key, "lastUpdate", now_iso8901())
+            .ignore();
         let status = if new_count == data.NumberOfSeriesRelatedInstances {
             // pipe.del(&series_key).ignore();
             FileStatus::Last
-        } else {
-            pipe.hset(&series_key, "fileCounter", new_count)
-                .ignore()
-                .hset(&series_key, "lastUpdate", now_iso8901())
-                .ignore();
-            if new_count > data.NumberOfSeriesRelatedInstances {
-                let error = format!(
-                    "Received too many files for series. \
+        } else if new_count > data.NumberOfSeriesRelatedInstances {
+            let error = format!(
+                "Received too many files for series. \
                     !!!SOMETHING IS VERY WRONG!!! \
                     key={} {:?}",
-                    &series_key, &data
-                );
-                FileStatus::Exception(error)
-            } else {
-                FileStatus::NotLast
-            }
+                &series_key, &data
+            );
+            FileStatus::Exception(error)
+        } else {
+            FileStatus::NotLast
         };
         pipe.query(con).map(|_: Option<()>| Some(status))
     })
     .with_context(|| format!("Redis transaction failed on key: {}", &series_key))?;
     is_last.into_result()
 }
```

### Comparing `px_recount-3.11.0rc2/PKG-INFO` & `px_recount-3.11.0rc3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: px-recount
-Version: 3.11.0rc2
+Version: 3.11.0rc3
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
```

