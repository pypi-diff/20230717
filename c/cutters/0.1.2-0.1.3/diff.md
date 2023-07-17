# Comparing `tmp/cutters-0.1.2.tar.gz` & `tmp/cutters-0.1.3.tar.gz`

## Comparing `cutters-0.1.2.tar` & `cutters-0.1.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0      358 1970-01-01 00:00:00.000000 cutters-0.1.2/local_dependencies/cutters/Cargo.toml
--rw-r--r--   0     1000      984       46 2022-02-09 12:57:48.000000 cutters-0.1.2/local_dependencies/cutters/.gitignore
--rw-r--r--   0     1000      984     2978 2022-02-11 10:46:22.000000 cutters-0.1.2/local_dependencies/cutters/README.md
--rw-r--r--   0     1000      984      290 2022-02-09 12:57:48.000000 cutters-0.1.2/local_dependencies/cutters/res/baseline.pest
--rw-r--r--   0     1000      984     4340 2022-02-09 19:26:06.000000 cutters-0.1.2/local_dependencies/cutters/res/en.pest
--rw-r--r--   0     1000      984     3667 2022-02-09 19:24:03.000000 cutters-0.1.2/local_dependencies/cutters/res/hr.pest
--rw-r--r--   0     1000      984     1841 2022-02-09 17:49:24.000000 cutters-0.1.2/local_dependencies/cutters/src/lib.rs
--rw-r--r--   0     1000      984     1166 2022-02-09 12:57:48.000000 cutters-0.1.2/local_dependencies/cutters/src/parsers/baseline.rs
--rw-r--r--   0     1000      984     4308 2022-02-09 18:35:27.000000 cutters-0.1.2/local_dependencies/cutters/src/parsers/croatian.rs
--rw-r--r--   0     1000      984     3942 2022-02-09 18:35:23.000000 cutters-0.1.2/local_dependencies/cutters/src/parsers/english.rs
--rw-r--r--   0     1000      984       53 2022-02-09 17:41:01.000000 cutters-0.1.2/local_dependencies/cutters/src/parsers/mod.rs
--rw-r--r--   0        0        0      322 1970-01-01 00:00:00.000000 cutters-0.1.2/Cargo.toml
--rw-r--r--   0     1000      984       46 2022-02-09 12:57:48.000000 cutters-0.1.2/.gitignore
--rw-r--r--   0     1000      984       43 2022-02-10 13:07:58.000000 cutters-0.1.2/MANIFEST.in
--rw-r--r--   0     1000      984     2791 2022-02-11 11:07:24.000000 cutters-0.1.2/README.md
--rw-r--r--   0     1000      984      486 2022-02-11 11:08:19.000000 cutters-0.1.2/pyproject.toml
--rw-r--r--   0     1000      984      728 2022-02-11 11:08:35.000000 cutters-0.1.2/setup.py
--rw-r--r--   0     1000      984     1822 2022-02-09 20:12:39.000000 cutters-0.1.2/src/lib.rs
--rw-r--r--   0     1000      984     5967 2022-02-10 23:17:05.000000 cutters-0.1.2/test.py
--rw-r--r--   0        0        0     3208 1970-01-01 00:00:00.000000 cutters-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      358 1970-01-01 00:00:00.000000 cutters-0.1.3/local_dependencies/cutters/Cargo.toml
+-rw-r--r--   0     1000      984       46 2022-02-09 12:57:48.000000 cutters-0.1.3/local_dependencies/cutters/.gitignore
+-rw-r--r--   0     1000      984     2978 2022-02-11 10:46:22.000000 cutters-0.1.3/local_dependencies/cutters/README.md
+-rw-r--r--   0     1000      984      290 2022-02-09 12:57:48.000000 cutters-0.1.3/local_dependencies/cutters/res/baseline.pest
+-rw-r--r--   0     1000      984     4656 2022-03-01 17:38:08.000000 cutters-0.1.3/local_dependencies/cutters/res/en.pest
+-rw-r--r--   0     1000      984     3983 2022-03-01 17:38:04.000000 cutters-0.1.3/local_dependencies/cutters/res/hr.pest
+-rw-r--r--   0     1000      984     1841 2022-02-09 17:49:24.000000 cutters-0.1.3/local_dependencies/cutters/src/lib.rs
+-rw-r--r--   0     1000      984     1166 2022-02-09 12:57:48.000000 cutters-0.1.3/local_dependencies/cutters/src/parsers/baseline.rs
+-rw-r--r--   0     1000      984     4988 2022-03-01 17:31:55.000000 cutters-0.1.3/local_dependencies/cutters/src/parsers/croatian.rs
+-rw-r--r--   0     1000      984     4405 2022-03-01 17:31:49.000000 cutters-0.1.3/local_dependencies/cutters/src/parsers/english.rs
+-rw-r--r--   0     1000      984       53 2022-02-09 17:41:01.000000 cutters-0.1.3/local_dependencies/cutters/src/parsers/mod.rs
+-rw-r--r--   0        0        0      322 1970-01-01 00:00:00.000000 cutters-0.1.3/Cargo.toml
+-rw-r--r--   0     1000      984       46 2022-02-09 12:57:48.000000 cutters-0.1.3/.gitignore
+-rw-r--r--   0     1000      984       43 2022-02-10 13:07:58.000000 cutters-0.1.3/MANIFEST.in
+-rw-r--r--   0     1000      984     2791 2022-02-11 11:07:24.000000 cutters-0.1.3/README.md
+-rw-r--r--   0     1000      984      502 2022-03-01 17:33:21.000000 cutters-0.1.3/pyproject.toml
+-rw-r--r--   0     1000      984      728 2022-03-01 17:33:31.000000 cutters-0.1.3/setup.py
+-rw-r--r--   0     1000      984     1822 2022-03-01 17:19:52.000000 cutters-0.1.3/src/lib.rs
+-rw-r--r--   0     1000      984      665 2022-03-01 17:40:15.000000 cutters-0.1.3/test.py
+-rw-r--r--   0        0        0     3274 1970-01-01 00:00:00.000000 cutters-0.1.3/PKG-INFO
```

### Comparing `cutters-0.1.2/local_dependencies/cutters/README.md` & `cutters-0.1.3/local_dependencies/cutters/README.md`

 * *Files identical despite different names*

### Comparing `cutters-0.1.2/local_dependencies/cutters/res/en.pest` & `cutters-0.1.3/local_dependencies/cutters/res/en.pest`

 * *Files 23% similar despite different names*

```diff
@@ -42,45 +42,56 @@
     )
 }
 number = _{
     NUMBER+ |
     roman_numeral
 }
 
+ignoreable = _{
+    ("(" ~ (!")" ~ ANY)* ~ ")") |
+    ("[" ~ (!"]" ~ ANY)* ~ "]") |
+    ("{" ~ (!"}" ~ ANY)* ~ "}")
+}
+
 possible_sentence_start = _{ WHITE_SPACE* ~ (UPPERCASE_LETTER | TITLECASE_LETTER | QUOTATION_MARK | NUMBER) }
 complete_ending = _{ (WHITE_SPACE* ~ SENTENCE_TERMINAL+)+ }
 
 quoted_internal_sentence = _{
     &(NEWLINE+) |
     (WHITE_SPACE+ ~ ending_abbreviation+ ~ &possible_sentence_start) | // abbreviation at the end of a sentence
     ((number ~ WHITE_SPACE* ~ "." ~ WHITE_SPACE* ~ number) ~ &possible_sentence_start ~ !number) |
     ((number ~ WHITE_SPACE* ~ "." ~ WHITE_SPACE* ~ number) ~ !(WHITE_SPACE* ~ (UPPERCASE_LETTER | TITLECASE_LETTER)) ~ quoted_internal_sentence) |
-    ((contraction | (WHITE_SPACE+ ~ abbreviation+) | (!(SENTENCE_TERMINAL | QUOTATION_MARK) ~ ANY ) | (SENTENCE_TERMINAL ~ !possible_sentence_start)) ~ quoted_internal_sentence) |
+    ((ignoreable | contraction | (WHITE_SPACE+ ~ abbreviation+) | (!(SENTENCE_TERMINAL | QUOTATION_MARK) ~ ANY ) | (SENTENCE_TERMINAL ~ !possible_sentence_start)) ~ quoted_internal_sentence) |
     (complete_ending) |
     &QUOTATION_MARK
 }
 
 quote_sentence = { &possible_sentence_start ~ !QUOTATION_MARK ~ WHITE_SPACE* ~ abbreviation* ~ quoted_internal_sentence }
 
 quote = {
     (WHITE_SPACE* ~ quote_sentence ~ (!NEWLINE ~ WHITE_SPACE)*)+
 }
 
 quote_wrapper = _{
     (QUOTATION_MARK ~ quote ~ (&(NEWLINE+) | QUOTATION_MARK))
 }
 
+quoted_phrase = _{
+    (QUOTATION_MARK ~ !possible_sentence_start ~ (!QUOTATION_MARK~ ANY)* ~ (&(NEWLINE+) | QUOTATION_MARK))
+}
+
 internal_sentence = _{
     &(NEWLINE+) |
     (WHITE_SPACE+ ~ ending_abbreviation+ ~ &possible_sentence_start) |
     (contraction ~ internal_sentence) |
+    (quoted_phrase ~ internal_sentence) |
     ((number ~ WHITE_SPACE* ~ "." ~ WHITE_SPACE* ~ number) ~ ((&possible_sentence_start ~ !number) | &EOI)) |
     ((number ~ WHITE_SPACE* ~ "." ~ WHITE_SPACE* ~ number) ~ !(WHITE_SPACE* ~ (UPPERCASE_LETTER | TITLECASE_LETTER)) ~ internal_sentence) |
     (quote_wrapper ~ (&possible_sentence_start | internal_sentence | &EOI)) |
-    (((WHITE_SPACE+ ~ abbreviation+) | (!SENTENCE_TERMINAL ~ ANY ) | (SENTENCE_TERMINAL ~ !possible_sentence_start)) ~ internal_sentence) |
+    ((ignoreable | (WHITE_SPACE+ ~ abbreviation+) | (!SENTENCE_TERMINAL ~ ANY ) | (SENTENCE_TERMINAL ~ !possible_sentence_start)) ~ internal_sentence) |
     (complete_ending) |
     (!WHITE_SPACE ~ ANY)+
 }
 
 sentence = { &possible_sentence_start ~ WHITE_SPACE* ~ abbreviation* ~ internal_sentence }
 
 sentence_list = _{ (WHITE_SPACE* ~ (sentence | ANY) ~ WHITE_SPACE*)* }
```

### Comparing `cutters-0.1.2/local_dependencies/cutters/res/hr.pest` & `cutters-0.1.3/local_dependencies/cutters/res/hr.pest`

 * *Files 2% similar despite different names*

```diff
@@ -31,44 +31,55 @@
     )
 }
 number = _{
     NUMBER+ |
     roman_numeral
 }
 
+ignoreable = _{
+    ("(" ~ (!")" ~ ANY)* ~ ")") |
+    ("[" ~ (!"]" ~ ANY)* ~ "]") |
+    ("{" ~ (!"}" ~ ANY)* ~ "}")
+}
+
 possible_sentence_start = _{ WHITE_SPACE* ~ (UPPERCASE_LETTER | TITLECASE_LETTER | QUOTATION_MARK | NUMBER) }
 complete_ending = _{ (WHITE_SPACE* ~ SENTENCE_TERMINAL+)+ }
 
 quoted_internal_sentence = _{
     &(NEWLINE+) |
     (WHITE_SPACE+ ~ ending_abbreviation ~ &possible_sentence_start) | // abbreviation at the end of a sentence
     ((number ~ WHITE_SPACE* ~ "." ~ WHITE_SPACE*)+ ~ &possible_sentence_start ~ !number) |
     ((number ~ WHITE_SPACE* ~ "." ~ WHITE_SPACE*)+ ~ !(WHITE_SPACE* ~ (UPPERCASE_LETTER | TITLECASE_LETTER)) ~ quoted_internal_sentence) |
-    (((WHITE_SPACE+ ~ abbreviation+) | (!(SENTENCE_TERMINAL | QUOTATION_MARK) ~ ANY ) | (SENTENCE_TERMINAL ~ !possible_sentence_start)) ~ quoted_internal_sentence) |
+    ((ignoreable | (WHITE_SPACE+ ~ abbreviation+) | (!(SENTENCE_TERMINAL | QUOTATION_MARK) ~ ANY ) | (SENTENCE_TERMINAL ~ !possible_sentence_start)) ~ quoted_internal_sentence) |
     (complete_ending) |
     &QUOTATION_MARK
 }
 
 quote_sentence = { &possible_sentence_start ~ !QUOTATION_MARK ~ WHITE_SPACE* ~ abbreviation* ~ quoted_internal_sentence }
 
 quote = {
     (WHITE_SPACE* ~ quote_sentence ~ (!NEWLINE ~ WHITE_SPACE)*)+
 }
 
 quote_wrapper = _{
     (QUOTATION_MARK ~ quote ~ (&(NEWLINE+) | QUOTATION_MARK))
 }
 
+quoted_phrase = _{
+    (QUOTATION_MARK ~ !possible_sentence_start ~ (!QUOTATION_MARK~ ANY)* ~ (&(NEWLINE+) | QUOTATION_MARK))
+}
+
 internal_sentence = _{
     &(NEWLINE+) |
     (WHITE_SPACE+ ~ ending_abbreviation+ ~ &possible_sentence_start) |
+    (quoted_phrase ~ internal_sentence) |
     (quote_wrapper ~ (&possible_sentence_start | internal_sentence | &EOI)) |
     ((number ~ WHITE_SPACE* ~ "." ~ WHITE_SPACE*)+ ~ ((&possible_sentence_start ~ !number) | &EOI)) |
     ((number ~ WHITE_SPACE* ~ "." ~ WHITE_SPACE*)+ ~ !(WHITE_SPACE* ~ (UPPERCASE_LETTER | TITLECASE_LETTER)) ~ internal_sentence) |
-    (((WHITE_SPACE+ ~ abbreviation+) | (!SENTENCE_TERMINAL ~ ANY ) | (SENTENCE_TERMINAL ~ !possible_sentence_start)) ~ internal_sentence) |
+    ((ignoreable | (WHITE_SPACE+ ~ abbreviation+) | (!SENTENCE_TERMINAL ~ ANY ) | (SENTENCE_TERMINAL ~ !possible_sentence_start)) ~ internal_sentence) |
     (complete_ending) |
     (!WHITE_SPACE ~ ANY)+
 }
 
 sentence = { &possible_sentence_start ~ WHITE_SPACE* ~ abbreviation* ~ internal_sentence }
 
 sentence_list = _{ (WHITE_SPACE* ~ (sentence | ANY) ~ WHITE_SPACE*)* }
```

### Comparing `cutters-0.1.2/local_dependencies/cutters/src/lib.rs` & `cutters-0.1.3/local_dependencies/cutters/src/lib.rs`

 * *Files identical despite different names*

### Comparing `cutters-0.1.2/local_dependencies/cutters/src/parsers/baseline.rs` & `cutters-0.1.3/local_dependencies/cutters/src/parsers/baseline.rs`

 * *Files identical despite different names*

### Comparing `cutters-0.1.2/local_dependencies/cutters/src/parsers/croatian.rs` & `cutters-0.1.3/local_dependencies/cutters/src/parsers/croatian.rs`

 * *Files 7% similar despite different names*

```diff
@@ -53,14 +53,29 @@
 
         for (sentence, query_sentence) in sentences.iter().zip(query_sentences) {
             assert!(query_sentence == sentence.str);
         }
     }
 
     #[test]
+    fn brackets() {
+        let query_sentences = vec![
+            r#"Novi standard temelji se na smjernicama iz novog Priručnika za sastavljače i korisnike statističkih pokazatelja o inozemnoj zaduženosti (engl. External Debt Statistics - Guide for Compilers and Users), a prihvatile su ga zemlje potpisnice Posebnog standarda o statističkom izvješčivanju (engl. Special Data Dissemination Standard - SDDS)."#,
+        ];
+
+        let text = query_sentences.join(" ");
+
+        let sentences = cut(&text);
+
+        for (sentence, query_sentence) in sentences.iter().zip(query_sentences) {
+            assert!(query_sentence == sentence.str);
+        }
+    }
+
+    #[test]
     fn quotes() {
         let query_quotes = vec![
             vec![vec![
                 r#"Sve sretne obitelji nalik su jedna na drugu, svaka nesretna obitelj nesretna je na svoj način."#,
             ]],
             vec![vec![r#"Hvala."#, r#"Ja također."#]],
             vec![vec![r#"Pazi!"#]],
```

### Comparing `cutters-0.1.2/local_dependencies/cutters/src/parsers/english.rs` & `cutters-0.1.3/local_dependencies/cutters/src/parsers/english.rs`

 * *Files 5% similar despite different names*

```diff
@@ -53,14 +53,29 @@
 
         for (sentence, query_sentence) in sentences.iter().zip(query_sentences) {
             assert!(query_sentence == sentence.str);
         }
     }
 
     #[test]
+    fn brackets() {
+        let query_sentences = vec![
+            r#"European Union (hrv. Europska Unija) is a political and economic union of 27 member states that are located primarily in Europe."#,
+        ];
+
+        let text = query_sentences.join(" ");
+
+        let sentences = cut(&text);
+
+        for (sentence, query_sentence) in sentences.iter().zip(query_sentences) {
+            assert!(query_sentence == sentence.str);
+        }
+    }
+
+    #[test]
     fn quotes() {
         let query_quotes = vec![
             vec![vec![
                 r#"Sve sretne obitelji nalik su jedna na drugu, svaka nesretna obitelj nesretna je na svoj način."#,
             ]],
             vec![vec![r#"Hvala."#, r#"Ja također."#]],
             vec![vec![r#"Pazi!"#]],
```

### Comparing `cutters-0.1.2/README.md` & `cutters-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `cutters-0.1.2/setup.py` & `cutters-0.1.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 from setuptools_rust import Binding, RustExtension
 
 setup(
     name="cutters",
-    version="0.1.2",
+    version="0.1.3",
     description="A rule based sentence segmentation library.",
     long_description=open("README.md", "r", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     author="cyanic-selkie",
     author_email="cyanic-selkie@protonmail.com",
     url="https://github.com/cyanic-selkie/cutters",
     license="MIT",
```

### Comparing `cutters-0.1.2/src/lib.rs` & `cutters-0.1.3/src/lib.rs`

 * *Files identical despite different names*

### Comparing `cutters-0.1.2/PKG-INFO` & `cutters-0.1.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: cutters
-Version: 0.1.2
+Version: 0.1.3
 Classifier: Natural Language :: Croatian
 Classifier: Natural Language :: English
 Classifier: Topic :: Text Processing
 Summary: A rule based sentence segmentation library.
 Author: cyanic-selkie <cyanic-selkie@protonmail.com>
 Author-email: cyanic-selkie <cyanic-selkie@protonmail.com>
 License: MIT
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
+Project-URL: Repository, https://github.com/cyanic-selkie/cutters
 
 <div align="center">
     <h1>cutters</h1>
     <p>
     A rule based sentence segmentation library.<br>
     <i>Python bindings for the <a href="https://crates.io/crates/cutters">cutters</a> library written in Rust.</i>
     </p>
```

#### html2text {}

```diff
@@ -1,14 +1,15 @@
-Metadata-Version: 2.1 Name: cutters Version: 0.1.2 Classifier: Natural Language
+Metadata-Version: 2.1 Name: cutters Version: 0.1.3 Classifier: Natural Language
 :: Croatian Classifier: Natural Language :: English Classifier: Topic :: Text
 Processing Summary: A rule based sentence segmentation library. Author: cyanic-
 selkie
 protonmail.com> Author-email: cyanic-selkie
 protonmail.com> License: MIT Description-Content-Type: text/markdown;
-charset=UTF-8; variant=GFM
+charset=UTF-8; variant=GFM Project-URL: Repository, https://github.com/cyanic-
+selkie/cutters
                              ****** cutters ******
                   A rule based sentence segmentation library.
            Python bindings for the cutters library written in Rust.
                         [Release] [License] [Downloads]
                     ð§ This library is experimental. ð§
 ## Features - Full UTF-8 support. - Robust parsing. - Language specific rules
 (each defined by its own [PEG](https://en.wikipedia.org/wiki/
```

