# Comparing `tmp/secure_sedge-1.7.2.tar.gz` & `tmp/secure_sedge-1.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "secure_sedge-1.7.2.tar", last modified: Mon Jul 17 07:07:39 2023, max compression
+gzip compressed data, was "secure_sedge-1.7.4.tar", last modified: Mon Jul 17 18:20:09 2023, max compression
```

## Comparing `secure_sedge-1.7.2.tar` & `secure_sedge-1.7.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-07-17 07:07:39.518595 secure_sedge-1.7.2/
--rwxr-xr-x   0 2ps       (1000) 2ps       (1000)       86 2022-07-30 10:57:45.000000 secure_sedge-1.7.2/MANIFEST.in
--rw-r--r--   0 2ps       (1000) 2ps       (1000)     5717 2023-07-17 07:07:39.518595 secure_sedge-1.7.2/PKG-INFO
-drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-07-17 07:07:39.518595 secure_sedge-1.7.2/docs/
--rwxr-xr-x   0 2ps       (1000) 2ps       (1000)     5165 2023-01-24 17:30:51.000000 secure_sedge-1.7.2/docs/index.rst
-drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-07-17 07:07:39.518595 secure_sedge-1.7.2/secure_sedge.egg-info/
--rw-r--r--   0 2ps       (1000) 2ps       (1000)     5717 2023-07-17 07:07:39.000000 secure_sedge-1.7.2/secure_sedge.egg-info/PKG-INFO
--rw-r--r--   0 2ps       (1000) 2ps       (1000)      364 2023-07-17 07:07:39.000000 secure_sedge-1.7.2/secure_sedge.egg-info/SOURCES.txt
--rw-r--r--   0 2ps       (1000) 2ps       (1000)        1 2023-07-17 07:07:39.000000 secure_sedge-1.7.2/secure_sedge.egg-info/dependency_links.txt
--rw-r--r--   0 2ps       (1000) 2ps       (1000)       49 2023-07-17 07:07:39.000000 secure_sedge-1.7.2/secure_sedge.egg-info/entry_points.txt
--rw-r--r--   0 2ps       (1000) 2ps       (1000)      111 2023-07-17 07:07:39.000000 secure_sedge-1.7.2/secure_sedge.egg-info/requires.txt
--rw-r--r--   0 2ps       (1000) 2ps       (1000)        6 2023-07-17 07:07:39.000000 secure_sedge-1.7.2/secure_sedge.egg-info/top_level.txt
-drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-07-17 07:07:39.518595 secure_sedge-1.7.2/sedge/
--rwxr-xr-x   0 2ps       (1000) 2ps       (1000)     4461 2023-02-21 19:50:49.000000 secure_sedge-1.7.2/sedge/README.md
--rwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2021-08-03 07:09:12.000000 secure_sedge-1.7.2/sedge/__init__.py
--rwxr-xr-x   0 2ps       (1000) 2ps       (1000)    19655 2023-07-17 07:05:30.000000 secure_sedge-1.7.2/sedge/installers.py
--rwxr-xr-x   0 2ps       (1000) 2ps       (1000)     1207 2023-07-17 07:07:38.000000 secure_sedge-1.7.2/sedge/main.py
--rwxr-xr-x   0 2ps       (1000) 2ps       (1000)    29492 2023-04-06 05:19:53.000000 secure_sedge-1.7.2/sedge/sewer.py
--rwxr-xr-x   0 2ps       (1000) 2ps       (1000)        6 2023-07-17 07:07:38.000000 secure_sedge-1.7.2/sedge/version.txt
--rwxr-xr-x   0 2ps       (1000) 2ps       (1000)       84 2023-07-17 07:07:39.518595 secure_sedge-1.7.2/setup.cfg
--rwxr-xr-x   0 2ps       (1000) 2ps       (1000)     2616 2023-07-17 07:07:38.000000 secure_sedge-1.7.2/setup.py
+drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-07-17 18:20:09.904861 secure_sedge-1.7.4/
+-rwxr-xr-x   0 2ps       (1000) 2ps       (1000)       86 2022-07-30 10:57:45.000000 secure_sedge-1.7.4/MANIFEST.in
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)     5717 2023-07-17 18:20:09.904861 secure_sedge-1.7.4/PKG-INFO
+drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-07-17 18:20:09.904861 secure_sedge-1.7.4/docs/
+-rwxr-xr-x   0 2ps       (1000) 2ps       (1000)     5165 2023-01-24 17:30:51.000000 secure_sedge-1.7.4/docs/index.rst
+drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-07-17 18:20:09.904861 secure_sedge-1.7.4/secure_sedge.egg-info/
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)     5717 2023-07-17 18:20:09.000000 secure_sedge-1.7.4/secure_sedge.egg-info/PKG-INFO
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)      364 2023-07-17 18:20:09.000000 secure_sedge-1.7.4/secure_sedge.egg-info/SOURCES.txt
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)        1 2023-07-17 18:20:09.000000 secure_sedge-1.7.4/secure_sedge.egg-info/dependency_links.txt
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)       49 2023-07-17 18:20:09.000000 secure_sedge-1.7.4/secure_sedge.egg-info/entry_points.txt
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)      111 2023-07-17 18:20:09.000000 secure_sedge-1.7.4/secure_sedge.egg-info/requires.txt
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)        6 2023-07-17 18:20:09.000000 secure_sedge-1.7.4/secure_sedge.egg-info/top_level.txt
+drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-07-17 18:20:09.904861 secure_sedge-1.7.4/sedge/
+-rwxr-xr-x   0 2ps       (1000) 2ps       (1000)     4461 2023-02-21 19:50:49.000000 secure_sedge-1.7.4/sedge/README.md
+-rwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2021-08-03 07:09:12.000000 secure_sedge-1.7.4/sedge/__init__.py
+-rwxr-xr-x   0 2ps       (1000) 2ps       (1000)    20119 2023-07-17 18:11:51.000000 secure_sedge-1.7.4/sedge/installers.py
+-rwxr-xr-x   0 2ps       (1000) 2ps       (1000)     1207 2023-07-17 18:20:09.000000 secure_sedge-1.7.4/sedge/main.py
+-rwxr-xr-x   0 2ps       (1000) 2ps       (1000)    29492 2023-04-06 05:19:53.000000 secure_sedge-1.7.4/sedge/sewer.py
+-rwxr-xr-x   0 2ps       (1000) 2ps       (1000)        6 2023-07-17 18:20:09.000000 secure_sedge-1.7.4/sedge/version.txt
+-rwxr-xr-x   0 2ps       (1000) 2ps       (1000)       84 2023-07-17 18:20:09.904861 secure_sedge-1.7.4/setup.cfg
+-rwxr-xr-x   0 2ps       (1000) 2ps       (1000)     2616 2023-07-17 18:20:09.000000 secure_sedge-1.7.4/setup.py
```

### Comparing `secure_sedge-1.7.2/PKG-INFO` & `secure_sedge-1.7.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: secure_sedge
-Version: 1.7.2
+Version: 1.7.4
 Summary: a helpful set of convocations to create certs
 Home-page: https://bitbucket.org/dbuy/secure_sedge
 Author: 2ps
 Author-email: p.shingavi@yahoo.com
 License: BSD
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `secure_sedge-1.7.2/docs/index.rst` & `secure_sedge-1.7.4/docs/index.rst`

 * *Files identical despite different names*

### Comparing `secure_sedge-1.7.2/secure_sedge.egg-info/PKG-INFO` & `secure_sedge-1.7.4/secure_sedge.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: secure-sedge
-Version: 1.7.2
+Version: 1.7.4
 Summary: a helpful set of convocations to create certs
 Home-page: https://bitbucket.org/dbuy/secure_sedge
 Author: 2ps
 Author-email: p.shingavi@yahoo.com
 License: BSD
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `secure_sedge-1.7.2/sedge/README.md` & `secure_sedge-1.7.4/sedge/README.md`

 * *Files identical despite different names*

### Comparing `secure_sedge-1.7.2/sedge/installers.py` & `secure_sedge-1.7.4/sedge/installers.py`

 * *Files 1% similar despite different names*

```diff
@@ -410,44 +410,61 @@
             {'}'}
         {'}'}
         """
     )
     ctx.run(c)
 
 
-@task
-def trust_keystore(ctx, keystore_filename, input_bundle='/etc/ssl/certs/ca-bundle.crt', password=None):
-    """
-    builds a trust keystore from the specified cert bundle
-
-    password may be specified via the SEDGE_KEYSTORE_PASSWORD command
-    """
+def trusted_cert_entries(certs, seen):
     from cryptography import x509
-    from cryptography.hazmat.backends import default_backend
     from cryptography.hazmat.primitives import serialization
     from jks.jks import TrustedCertEntry
-    from jks.jks import KeyStore
-    password = password or os.environ.get('SEDGE_KEYSTORE_PASSWORD')
-    with open(input_bundle, 'rb') as f:
-        data = f.read()
-    certs = x509.load_pem_x509_certificates(data)
-    print(f'found {len(certs)} certs in {input_bundle}')
-    seen = dict()
     entries = []
     for cert in certs:
-        print(type(cert))
         alias = cert.subject.rfc4514_string()
         i = 0
         original_alias = alias
         while alias in seen:
             i += 1
             alias = f'{original_alias}{i:02d}'
         der = cert.public_bytes(serialization.Encoding.DER)
         seen[alias] = cert
         entries.append(TrustedCertEntry.new(alias, der))
+    return entries
+
+
+@task
+def trust_keystore(
+        ctx, keystore_filename, bucket, cert_object,
+        ca_bundle='/etc/ssl/certs/ca-bundle.crt', password=None,
+        profile=None, region=None):
+    """
+    builds a trust keystore from the specified cert bundle and sedge cert
+
+    password may be specified via the SEDGE_KEYSTORE_PASSWORD command
+    """
+    from cryptography import x509
+    from jks.jks import KeyStore
+    from boto3 import Session
+    session = Session(profile_name=profile, region_name=region)
+    password = password or os.environ.get('SEDGE_KEYSTORE_PASSWORD')
+    seen = dict()
+    entries = []
+    with open(ca_bundle, 'rb') as f:
+        data = f.read()
+    certs = x509.load_pem_x509_certificates(data)
+    print(f'found {len(certs)} certs in {ca_bundle}')
+    entries = trusted_cert_entries(certs, seen)
+
+    s3 = session.resource('s3')
+    s3_cert = s3.Object(bucket, cert_object)
+    response = s3_cert.get()
+    data = response['Body'].read()
+    certs = x509.load_pem_x509_certificates(data)
+    entries += trusted_cert_entries(certs[1:], seen)
     k = KeyStore.new('jks', entries)
     k.save(keystore_filename, password)
 
 
 @task
 def keystore(ctx, keystore_filename, name, bucket, cert_object, key_object,
              password=None, private_key_password=None, profile=None, region=None):
@@ -478,15 +495,14 @@
     response = s3_cert.get()
     data = response['Body'].read()
     certs = x509.load_pem_x509_certificates(data)
     print(f'found {len(certs)} certs in s3://{bucket}/{cert_object}')
     seen = dict()
     cert_chain = []
     for cert in certs:
-        print(type(cert))
         alias = cert.subject.rfc4514_string()
         i = 0
         original_alias = alias
         while alias in seen:
             i += 1
             alias = f'{original_alias}{i:02d}'
         der = cert.public_bytes(serialization.Encoding.DER)
```

### Comparing `secure_sedge-1.7.2/sedge/main.py` & `secure_sedge-1.7.4/sedge/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,8 +39,8 @@
             'handlers': [ 'console-brief', ],
             'propagate': False,
         }
     }
 ))
 ns = Collection.from_module(sewer)
 ns.add_collection(installers.installers_collection, 'install')
-program = Program(version='1.7.2', namespace=ns)
+program = Program(version='1.7.4', namespace=ns)
```

### Comparing `secure_sedge-1.7.2/sedge/sewer.py` & `secure_sedge-1.7.4/sedge/sewer.py`

 * *Files identical despite different names*

### Comparing `secure_sedge-1.7.2/setup.py` & `secure_sedge-1.7.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 except ImportError:
     from pkg_resources import resource_string
     readme_text = resource_string('sedge', 'README.md')
     readme_text = readme_text.decode('utf-8')
 
 # Version info -- read without importing
 _locals = {}
-version = '1.7.2'
+version = '1.7.4'
 
 
 # PyYAML ships a split Python 2/3 codebase. Unfortunately, some pip versions
 # attempt to interpret both halves of PyYAML, yielding SyntaxErrors. Thus, we
 # exclude whichever appears inappropriate for the installing interpreter.
 exclude = ['*.yaml2', 'tests']
```

