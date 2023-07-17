# Comparing `tmp/wordx-0.2.5.tar.gz` & `tmp/wordx-0.2.6.tar.gz`

## Comparing `wordx-0.2.5.tar` & `wordx-0.2.6.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wordx-0.2.5/src/wordx/__init__.py
--rw-r--r--   0        0        0     3749 2020-02-02 00:00:00.000000 wordx-0.2.5/src/wordx/fake_zip.py
--rw-r--r--   0        0        0     1650 2020-02-02 00:00:00.000000 wordx-0.2.5/src/wordx/sheet.py
--rw-r--r--   0        0        0     2899 2020-02-02 00:00:00.000000 wordx-0.2.5/src/wordx/utility.py
--rw-r--r--   0        0        0     3953 2020-02-02 00:00:00.000000 wordx-0.2.5/src/wordx/word_file.py
--rw-r--r--   0        0        0    25045 2020-02-02 00:00:00.000000 wordx-0.2.5/tests/1.png
--rw-r--r--   0        0        0     2962 2020-02-02 00:00:00.000000 wordx-0.2.5/tests/1.py
--rw-r--r--   0        0        0   241198 2020-02-02 00:00:00.000000 wordx-0.2.5/tests/123.docx
--rw-r--r--   0        0        0    12116 2020-02-02 00:00:00.000000 wordx-0.2.5/tests/2.docx
--rw-r--r--   0        0        0    12203 2020-02-02 00:00:00.000000 wordx-0.2.5/tests/3.docx
--rw-r--r--   0        0        0    12699 2020-02-02 00:00:00.000000 wordx-0.2.5/tests/footer.docx
--rw-r--r--   0        0        0    12201 2020-02-02 00:00:00.000000 wordx-0.2.5/tests/footer.xml
--rw-r--r--   0        0        0     2920 2020-02-02 00:00:00.000000 wordx-0.2.5/tests/haha.xml
--rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 wordx-0.2.5/tests/test_fake_zip.py
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 wordx-0.2.5/tests/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 wordx-0.2.5/tests/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 wordx-0.2.5/tests/.pytest_cache/README.md
--rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 wordx-0.2.5/tests/.pytest_cache/v/cache/lastfailed
--rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 wordx-0.2.5/tests/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 wordx-0.2.5/tests/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0    14195 2020-02-02 00:00:00.000000 wordx-0.2.5/tests/文档合并/123.docx
--rw-r--r--   0        0        0    14199 2020-02-02 00:00:00.000000 wordx-0.2.5/tests/文档合并/456.docx
--rw-r--r--   0        0        0    12076 2020-02-02 00:00:00.000000 wordx-0.2.5/tests/文档合并/merge.docx
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 wordx-0.2.5/tests/文档合并/merge.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 wordx-0.2.5/LICENSE
--rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 wordx-0.2.5/README.md
--rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 wordx-0.2.5/pyproject.toml
--rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 wordx-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wordx-0.2.6/src/wordx/__init__.py
+-rw-r--r--   0        0        0     3749 2020-02-02 00:00:00.000000 wordx-0.2.6/src/wordx/fake_zip.py
+-rw-r--r--   0        0        0     1650 2020-02-02 00:00:00.000000 wordx-0.2.6/src/wordx/sheet.py
+-rw-r--r--   0        0        0     2915 2020-02-02 00:00:00.000000 wordx-0.2.6/src/wordx/utility.py
+-rw-r--r--   0        0        0     3953 2020-02-02 00:00:00.000000 wordx-0.2.6/src/wordx/word_file.py
+-rw-r--r--   0        0        0    25045 2020-02-02 00:00:00.000000 wordx-0.2.6/tests/1.png
+-rw-r--r--   0        0        0     2962 2020-02-02 00:00:00.000000 wordx-0.2.6/tests/1.py
+-rw-r--r--   0        0        0   241198 2020-02-02 00:00:00.000000 wordx-0.2.6/tests/123.docx
+-rw-r--r--   0        0        0    12116 2020-02-02 00:00:00.000000 wordx-0.2.6/tests/2.docx
+-rw-r--r--   0        0        0    12203 2020-02-02 00:00:00.000000 wordx-0.2.6/tests/3.docx
+-rw-r--r--   0        0        0    12699 2020-02-02 00:00:00.000000 wordx-0.2.6/tests/footer.docx
+-rw-r--r--   0        0        0    12201 2020-02-02 00:00:00.000000 wordx-0.2.6/tests/footer.xml
+-rw-r--r--   0        0        0     2920 2020-02-02 00:00:00.000000 wordx-0.2.6/tests/haha.xml
+-rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 wordx-0.2.6/tests/test_fake_zip.py
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 wordx-0.2.6/tests/.pytest_cache/.gitignore
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 wordx-0.2.6/tests/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 wordx-0.2.6/tests/.pytest_cache/README.md
+-rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 wordx-0.2.6/tests/.pytest_cache/v/cache/lastfailed
+-rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 wordx-0.2.6/tests/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 wordx-0.2.6/tests/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0    14195 2020-02-02 00:00:00.000000 wordx-0.2.6/tests/文档合并/123.docx
+-rw-r--r--   0        0        0    14199 2020-02-02 00:00:00.000000 wordx-0.2.6/tests/文档合并/456.docx
+-rw-r--r--   0        0        0    12076 2020-02-02 00:00:00.000000 wordx-0.2.6/tests/文档合并/merge.docx
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 wordx-0.2.6/tests/文档合并/merge.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 wordx-0.2.6/LICENSE
+-rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 wordx-0.2.6/README.md
+-rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 wordx-0.2.6/pyproject.toml
+-rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 wordx-0.2.6/PKG-INFO
```

### Comparing `wordx-0.2.5/src/wordx/fake_zip.py` & `wordx-0.2.6/src/wordx/fake_zip.py`

 * *Files identical despite different names*

### Comparing `wordx-0.2.5/src/wordx/sheet.py` & `wordx-0.2.6/src/wordx/sheet.py`

 * *Files identical despite different names*

### Comparing `wordx-0.2.5/src/wordx/utility.py` & `wordx-0.2.6/src/wordx/utility.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,14 +55,14 @@
         self.save_relations(xml_file, relations)
         return relation_id
 
     def add_footer_relation(self):
         footer_relation_id = random.randint(1000,9999)
         footer_file = f'footer{footer_relation_id}.xml'
         self.add_relation('document.xml', 'footer', footer_file, footer_relation_id)
-        return footer_relation_id, footer_file
+        return f'rId{footer_relation_id}', footer_file
 
     def add_header_relation(self):
         header_relation_id = random.randint(1000,9999)
         header_file = f'header{header_relation_id}.xml'
         self.add_relation('document.xml', 'header', header_file, header_relation_id)
-        return header_relation_id, header_file
+        return f'rId{header_relation_id}', header_file
```

### Comparing `wordx-0.2.5/src/wordx/word_file.py` & `wordx-0.2.6/src/wordx/word_file.py`

 * *Files identical despite different names*

### Comparing `wordx-0.2.5/tests/1.png` & `wordx-0.2.6/tests/1.png`

 * *Files identical despite different names*

### Comparing `wordx-0.2.5/tests/1.py` & `wordx-0.2.6/tests/1.py`

 * *Files identical despite different names*

### Comparing `wordx-0.2.5/tests/123.docx` & `wordx-0.2.6/tests/123.docx`

 * *Files identical despite different names*

### Comparing `wordx-0.2.5/tests/2.docx` & `wordx-0.2.6/tests/2.docx`

 * *Files identical despite different names*

### Comparing `wordx-0.2.5/tests/3.docx` & `wordx-0.2.6/tests/3.docx`

 * *Files identical despite different names*

### Comparing `wordx-0.2.5/tests/footer.docx` & `wordx-0.2.6/tests/footer.docx`

 * *Files identical despite different names*

### Comparing `wordx-0.2.5/tests/footer.xml` & `wordx-0.2.6/tests/footer.xml`

 * *Files identical despite different names*

### Comparing `wordx-0.2.5/tests/haha.xml` & `wordx-0.2.6/tests/haha.xml`

 * *Files identical despite different names*

### Comparing `wordx-0.2.5/tests/test_fake_zip.py` & `wordx-0.2.6/tests/test_fake_zip.py`

 * *Files identical despite different names*

### Comparing `wordx-0.2.5/tests/文档合并/123.docx` & `wordx-0.2.6/tests/文档合并/123.docx`

 * *Files identical despite different names*

### Comparing `wordx-0.2.5/tests/文档合并/456.docx` & `wordx-0.2.6/tests/文档合并/456.docx`

 * *Files identical despite different names*

### Comparing `wordx-0.2.5/tests/文档合并/merge.docx` & `wordx-0.2.6/tests/文档合并/merge.docx`

 * *Files identical despite different names*

### Comparing `wordx-0.2.5/LICENSE` & `wordx-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `wordx-0.2.5/pyproject.toml` & `wordx-0.2.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "wordx"
-version = "0.2.5"
+version = "0.2.6"
 authors = [
   { name="inspirare6", email="inspirare6@163.com" },
 ]
 description = "generate word documents in a sexy way"
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
```

### Comparing `wordx-0.2.5/PKG-INFO` & `wordx-0.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wordx
-Version: 0.2.5
+Version: 0.2.6
 Summary: generate word documents in a sexy way
 Project-URL: Homepage, https://github.com/inspirare6/wordx
 Project-URL: Bug Tracker, https://github.com/inspirare6/wordx/issues
 Author-email: inspirare6 <inspirare6@163.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

