# Comparing `tmp/sentecon-0.1.7-py3-none-any.whl.zip` & `tmp/sentecon-0.1.8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,17 @@
-Zip file size: 2191414 bytes, number of entries: 15
+Zip file size: 2191413 bytes, number of entries: 15
 -rw-rw-r--  2.0 unx       26 b- defN 23-Jul-07 03:28 sentecon/__init__.py
--rw-rw-r--  2.0 unx     5230 b- defN 23-Jul-17 19:44 sentecon/core.py
+-rw-rw-r--  2.0 unx     5235 b- defN 23-Jul-17 21:16 sentecon/core.py
 -rw-rw-r--  2.0 unx   936473 b- defN 23-Jul-07 03:30 sentecon/data/EmpathVocab_centroids_Empath_all-MiniLM-L6-v2.csv
 -rw-rw-r--  2.0 unx  1886798 b- defN 23-Jul-07 03:30 sentecon/data/EmpathVocab_centroids_Empath_all-mpnet-base-v2.csv
 -rw-rw-r--  2.0 unx   351609 b- defN 23-Jul-07 03:30 sentecon/data/LIWCVocab_centroids_LIWC_all-MiniLM-L6-v2.csv
 -rw-rw-r--  2.0 unx   506131 b- defN 23-Jul-07 03:30 sentecon/data/LIWCVocab_centroids_LIWC_all-distilroberta-v1.csv
 -rw-rw-r--  2.0 unx   710224 b- defN 23-Jul-07 03:30 sentecon/data/LIWCVocab_centroids_LIWC_all-mpnet-base-v2.csv
 -rw-rw-r--  2.0 unx   462534 b- defN 23-Jul-07 03:30 sentecon/data/LIWCVocab_centroids_LIWC_bert-base-uncased.csv
 -rw-rw-r--  2.0 unx   482765 b- defN 23-Jul-07 03:30 sentecon/data/LIWCVocab_centroids_LIWC_roberta-base.csv
 -rw-rw-r--  2.0 unx   219530 b- defN 23-Jul-07 03:28 sentecon/data/empath_vocab.csv
 -rwxrwxr-x  2.0 unx    47458 b- defN 23-Jul-07 03:28 sentecon/data/liwc_vocab.csv
--rw-rw-r--  2.0 unx      411 b- defN 23-Jul-17 19:44 sentecon-0.1.7.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jul-17 19:44 sentecon-0.1.7.dist-info/WHEEL
--rw-rw-r--  2.0 unx        9 b- defN 23-Jul-17 19:44 sentecon-0.1.7.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1461 b- defN 23-Jul-17 19:44 sentecon-0.1.7.dist-info/RECORD
-15 files, 5610751 bytes uncompressed, 2188952 bytes compressed:  61.0%
+-rw-rw-r--  2.0 unx      411 b- defN 23-Jul-17 21:18 sentecon-0.1.8.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jul-17 21:18 sentecon-0.1.8.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        9 b- defN 23-Jul-17 21:18 sentecon-0.1.8.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1461 b- defN 23-Jul-17 21:18 sentecon-0.1.8.dist-info/RECORD
+15 files, 5610756 bytes uncompressed, 2188951 bytes compressed:  61.0%
```

## zipnote {}

```diff
@@ -27,20 +27,20 @@
 
 Filename: sentecon/data/empath_vocab.csv
 Comment: 
 
 Filename: sentecon/data/liwc_vocab.csv
 Comment: 
 
-Filename: sentecon-0.1.7.dist-info/METADATA
+Filename: sentecon-0.1.8.dist-info/METADATA
 Comment: 
 
-Filename: sentecon-0.1.7.dist-info/WHEEL
+Filename: sentecon-0.1.8.dist-info/WHEEL
 Comment: 
 
-Filename: sentecon-0.1.7.dist-info/top_level.txt
+Filename: sentecon-0.1.8.dist-info/top_level.txt
 Comment: 
 
-Filename: sentecon-0.1.7.dist-info/RECORD
+Filename: sentecon-0.1.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## sentecon/core.py

```diff
@@ -37,15 +37,15 @@
             parse, self.category_names = liwc.load_token_parser(liwc_path)
             if liwc_subset:
                 self.category_names = self.category_names[21:]
 
         if self.num_centroids > 1:
             self.category_headers = []
             for cluster in range(self.num_centroids):
-                self.category_headers += ['{}_c{}'.format(category, cluster) for category in category_names]
+                self.category_headers += ['{}_c{}'.format(category, cluster) for category in self.category_names]
         else:
             self.category_headers = self.category_names
         
         # corpus_df = pd.read_pickle(os.path.join(self.data_dir, '{}Vocab_corpus_{}_{}.pkl'.format(
         #     self.lexicon, self.lexicon, self.lm)))
         # corpus_df.dropna(inplace=True)
```

## Comparing `sentecon-0.1.7.dist-info/RECORD` & `sentecon-0.1.8.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 sentecon/__init__.py,sha256=VAmQxF81BPXmuwPF4qUIePCac6mznS_VTnBrogeMWug,26
-sentecon/core.py,sha256=A6EQhh-8gB_Z61tEXenTL3e2v1MTr86_wow-_WVJgdI,5230
+sentecon/core.py,sha256=cEX-B_pxfAiCQOAK-eRHyF9dGmzHZ9WkPLFLiH5SKpM,5235
 sentecon/data/EmpathVocab_centroids_Empath_all-MiniLM-L6-v2.csv,sha256=yP_q_UgMfGIFzVz2TLAe9D6R8YoeuvJWdOOC3jrgWMY,936473
 sentecon/data/EmpathVocab_centroids_Empath_all-mpnet-base-v2.csv,sha256=XP5YlpHr1Hg8AgQu7fLDMCPrcMWuNAHT_Y547pybwbg,1886798
 sentecon/data/LIWCVocab_centroids_LIWC_all-MiniLM-L6-v2.csv,sha256=qb8MFG2KkRC47Bt2_q4vpRgkT9AdXm-hBoxz43tK5kI,351609
 sentecon/data/LIWCVocab_centroids_LIWC_all-distilroberta-v1.csv,sha256=UGjtZid4Fpp2BxWH2cC5KI9ADoEPXTPOwaQ8eiFU6YM,506131
 sentecon/data/LIWCVocab_centroids_LIWC_all-mpnet-base-v2.csv,sha256=e_qbnOh6dTMMmipIXs7Jg6iT2DNxgbjiKKzg7D82Tp4,710224
 sentecon/data/LIWCVocab_centroids_LIWC_bert-base-uncased.csv,sha256=VVQlcQ8Lpr-XkwEs1AF6V0KYR9fTlh6YNLEzO85PjkU,462534
 sentecon/data/LIWCVocab_centroids_LIWC_roberta-base.csv,sha256=HUb8L6dI-nowDqudrIGHZM_mPxszjA4zZYCsiq39w_M,482765
 sentecon/data/empath_vocab.csv,sha256=R7EKMzoH3NJ5eHwXUTNyqWpniGtvzBV-hPdordKoiVg,219530
 sentecon/data/liwc_vocab.csv,sha256=WrNmXGN9dlnSJ-qWqFKdhfAOagBqMKBXAGpeS08WAi8,47458
-sentecon-0.1.7.dist-info/METADATA,sha256=E-bQziPgsuCuYyHV2Q4jA8XLQZs6UH0LCrBhEYuomL0,411
-sentecon-0.1.7.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-sentecon-0.1.7.dist-info/top_level.txt,sha256=Lf9c710FobR6j8uX0IZwgeajaYIIpToqmrX5LlRN5zY,9
-sentecon-0.1.7.dist-info/RECORD,,
+sentecon-0.1.8.dist-info/METADATA,sha256=nWPvtYi-vz3T5w-mh74sD18q2s9bX_iTg4etnOoyji4,411
+sentecon-0.1.8.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+sentecon-0.1.8.dist-info/top_level.txt,sha256=Lf9c710FobR6j8uX0IZwgeajaYIIpToqmrX5LlRN5zY,9
+sentecon-0.1.8.dist-info/RECORD,,
```

