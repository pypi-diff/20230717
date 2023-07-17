# Comparing `tmp/pronounspageviewer-1.0.1-py3-none-any.whl.zip` & `tmp/pronounspageviewer-1.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 4204 bytes, number of entries: 8
--rw-rw-rw-  2.0 fat     1944 b- defN 23-Jun-11 13:51 pronounspageviewer/__init__.py
+Zip file size: 4310 bytes, number of entries: 8
+-rw-rw-rw-  2.0 fat     2411 b- defN 23-Jul-17 17:23 pronounspageviewer/__init__.py
 -rw-rw-rw-  2.0 fat      892 b- defN 23-Jun-11 13:51 pronounspageviewer/__main__.py
--rw-rw-rw-  2.0 fat     1714 b- defN 23-Jun-11 15:02 pronounspageviewer-1.0.1.dist-info/LICENSE.txt
--rw-rw-rw-  2.0 fat      831 b- defN 23-Jun-11 15:02 pronounspageviewer-1.0.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-11 15:02 pronounspageviewer-1.0.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       72 b- defN 23-Jun-11 15:02 pronounspageviewer-1.0.1.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat       19 b- defN 23-Jun-11 15:02 pronounspageviewer-1.0.1.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      723 b- defN 23-Jun-11 15:02 pronounspageviewer-1.0.1.dist-info/RECORD
-8 files, 6287 bytes uncompressed, 2916 bytes compressed:  53.6%
+-rw-rw-rw-  2.0 fat     1714 b- defN 23-Jul-17 17:26 pronounspageviewer-1.0.2.dist-info/LICENSE.txt
+-rw-rw-rw-  2.0 fat      831 b- defN 23-Jul-17 17:26 pronounspageviewer-1.0.2.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-17 17:26 pronounspageviewer-1.0.2.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       72 b- defN 23-Jul-17 17:26 pronounspageviewer-1.0.2.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat       19 b- defN 23-Jul-17 17:26 pronounspageviewer-1.0.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      723 b- defN 23-Jul-17 17:26 pronounspageviewer-1.0.2.dist-info/RECORD
+8 files, 6754 bytes uncompressed, 3022 bytes compressed:  55.3%
```

## zipnote {}

```diff
@@ -1,25 +1,25 @@
 Filename: pronounspageviewer/__init__.py
 Comment: 
 
 Filename: pronounspageviewer/__main__.py
 Comment: 
 
-Filename: pronounspageviewer-1.0.1.dist-info/LICENSE.txt
+Filename: pronounspageviewer-1.0.2.dist-info/LICENSE.txt
 Comment: 
 
-Filename: pronounspageviewer-1.0.1.dist-info/METADATA
+Filename: pronounspageviewer-1.0.2.dist-info/METADATA
 Comment: 
 
-Filename: pronounspageviewer-1.0.1.dist-info/WHEEL
+Filename: pronounspageviewer-1.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: pronounspageviewer-1.0.1.dist-info/entry_points.txt
+Filename: pronounspageviewer-1.0.2.dist-info/entry_points.txt
 Comment: 
 
-Filename: pronounspageviewer-1.0.1.dist-info/top_level.txt
+Filename: pronounspageviewer-1.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: pronounspageviewer-1.0.1.dist-info/RECORD
+Filename: pronounspageviewer-1.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pronounspageviewer/__init__.py

```diff
@@ -7,45 +7,61 @@
         'close': 'Only if we\'re close',
     }
 
     def __init__(self, profile_data: dict):
         self.data = profile_data
         self.opinions = dict(self.base_opinions)
         for opinion in self.data.get('opinions', {}):
-            self.opinions[opinion] = self.data['opinions'][opinion].get('description')
+            self.opinions[opinion] = self.data['opinions'][opinion].get(
+                'description')
 
     def _print_opinion_list(self, heading: str, items: list, indent: str = ''):
         print(indent + heading)
         for item in items:
-            print(indent, item.get('value'), self.opinions.get(item.get('opinion')), sep='\t')
+            print(indent, item.get('value'), self.opinions.get(
+                item.get('opinion')), sep='\t')
 
     def _print_list(self, heading: str, key: str):
         print(heading + ':', ', '.join(self.data.get(key, [])))
 
     def _print_words(self):
         print('Words')
         for category in self.data.get('words', []):
-            self._print_opinion_list(category.get('header'), category.get('values', []), '\t')
+            self._print_opinion_list(category.get(
+                'header'), category.get('values', []), '\t')
+
+    def _print_custom_flags(self):
+        flags = self.data.get('customFlags', [])
+        if len(flags) == 0:
+            return
+        print('Custom flags')
+        for flag in flags:
+            if flag.get('description'):
+                print(f"\t{flag['name']}\t{flag['description']}")
+            else:
+                print('\t' + flag['name'])
 
     def print(self):
         if 'description' in self.data:
             print(self.data['description'])
         if 'age' in self.data:
             print('Age:', self.data['age'])
-        # Links
+        if 'links' in self.data:
+            self._print_list('Links', 'links')
         if 'flags' in self.data:
             self._print_list('Flags', 'flags')
         if 'customFlags' in self.data:
-            self._print_list('Custom flags', 'customFlags')
+            self._print_custom_flags()
         print()
         if 'names' in self.data:
             self._print_opinion_list('Names', self.data['names'])
         if 'pronouns' in self.data:
             self._print_opinion_list('Pronouns', self.data['pronouns'])
         if 'words' in self.data:
             self._print_words()
 
+
 def print_page(page: dict):
     print('Username:', page.get('username', '<no username>'))
     for profile in page.get('profiles', {}):
         print('Profile', profile)
         Profile(page['profiles'].get(profile, {})).print()
```

## Comparing `pronounspageviewer-1.0.1.dist-info/LICENSE.txt` & `pronounspageviewer-1.0.2.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `pronounspageviewer-1.0.1.dist-info/METADATA` & `pronounspageviewer-1.0.2.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pronounspageviewer
-Version: 1.0.1
+Version: 1.0.2
 Summary: View a Pronouns.page from its JSON file
 Author: Joe Greaves
 Project-URL: Homepage, https://github.com/Grvs44/Pronouns.page-Viewer
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
```

## Comparing `pronounspageviewer-1.0.1.dist-info/RECORD` & `pronounspageviewer-1.0.2.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-pronounspageviewer/__init__.py,sha256=Rzi7Ln_rYeRA0e-88Z2WkfxYxPjaxmTRagR9SCZD0N4,1944
+pronounspageviewer/__init__.py,sha256=ErvkP-VVMwbCNjulhZbqea8LH_IoY9PtdJFWscn2NTs,2411
 pronounspageviewer/__main__.py,sha256=X7T5YON5jkpwyg1go6l0YniaAq9GOfkcMVMK4rAQhNU,892
-pronounspageviewer-1.0.1.dist-info/LICENSE.txt,sha256=42KznO94fKWkiywx3MOxyp7ByNDs0OC_Q6LBuyrMhUM,1714
-pronounspageviewer-1.0.1.dist-info/METADATA,sha256=3_qXP3NcsUyDGNbB9HQEIN-JJyvy9uU6yP4SgrIY5mI,831
-pronounspageviewer-1.0.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-pronounspageviewer-1.0.1.dist-info/entry_points.txt,sha256=fA_p_TU4iwkpbnjzko5pmmeXVECj7N3Q7gCCI63R-so,72
-pronounspageviewer-1.0.1.dist-info/top_level.txt,sha256=3tyjVlGFhTUGWb3WyTwPwAusl-MGokJHH0QDVKjhCBM,19
-pronounspageviewer-1.0.1.dist-info/RECORD,,
+pronounspageviewer-1.0.2.dist-info/LICENSE.txt,sha256=42KznO94fKWkiywx3MOxyp7ByNDs0OC_Q6LBuyrMhUM,1714
+pronounspageviewer-1.0.2.dist-info/METADATA,sha256=M569q6Gi8tapFum5mkfCd0xMcW2bBhg778EqqhkK2rc,831
+pronounspageviewer-1.0.2.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+pronounspageviewer-1.0.2.dist-info/entry_points.txt,sha256=fA_p_TU4iwkpbnjzko5pmmeXVECj7N3Q7gCCI63R-so,72
+pronounspageviewer-1.0.2.dist-info/top_level.txt,sha256=3tyjVlGFhTUGWb3WyTwPwAusl-MGokJHH0QDVKjhCBM,19
+pronounspageviewer-1.0.2.dist-info/RECORD,,
```

