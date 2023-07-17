# Comparing `tmp/parse_emails-0.1.8.tar.gz` & `tmp/parse_emails-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "parse_emails-0.1.8.tar", max compression
+gzip compressed data, was "parse_emails-0.1.9.tar", max compression
```

## Comparing `parse_emails-0.1.8.tar` & `parse_emails-0.1.9.tar`

### file list

```diff
@@ -1,55 +1,55 @@
--rw-r--r--   0        0        0     1064 2023-04-03 09:39:47.521417 parse_emails-0.1.8/LICENSE
--rw-r--r--   0        0        0     2328 2023-04-03 09:39:47.521417 parse_emails-0.1.8/README.md
--rw-r--r--   0        0        0       50 2023-04-03 09:39:47.521417 parse_emails-0.1.8/parse_emails/__init__.py
--rw-r--r--   0        0        0     2290 2023-04-03 09:39:47.521417 parse_emails-0.1.8/parse_emails/common.py
--rw-r--r--   0        0        0    49697 2023-04-03 09:39:47.521417 parse_emails-0.1.8/parse_emails/constants.py
--rw-r--r--   0        0        0    20567 2023-04-03 09:39:47.521417 parse_emails-0.1.8/parse_emails/handle_eml.py
--rw-r--r--   0        0        0    39800 2023-04-03 09:39:47.521417 parse_emails-0.1.8/parse_emails/handle_msg.py
--rw-r--r--   0        0        0    10548 2023-04-03 09:39:47.521417 parse_emails-0.1.8/parse_emails/parse_emails.py
--rw-r--r--   0        0        0        0 2023-04-03 09:39:47.521417 parse_emails-0.1.8/parse_emails/tests/__init__.py
--rw-r--r--   0        0        0    29461 2023-04-03 09:39:47.521417 parse_emails-0.1.8/parse_emails/tests/parse_emails_test.py
--rw-r--r--   0        0        0    69301 2023-04-03 09:39:47.525417 parse_emails-0.1.8/parse_emails/tests/test_data/DONT_OPEN-MALICIOUS.eml
--rw-r--r--   0        0        0    69303 2023-04-03 09:39:47.525417 parse_emails-0.1.8/parse_emails/tests/test_data/DONT_OPEN-MALICIOUS_base64_headers.eml
--rw-r--r--   0        0        0 14960583 2023-04-03 09:39:47.613417 parse_emails-0.1.8/parse_emails/tests/test_data/Fwd_test-inner_attachment_eml.eml
--rw-r--r--   0        0        0     6500 2023-04-03 09:39:47.613417 parse_emails-0.1.8/parse_emails/tests/test_data/ParseEmailFiles-test-emls.eml
--rw-r--r--   0        0        0    23552 2023-04-03 09:39:47.613417 parse_emails-0.1.8/parse_emails/tests/test_data/Phishing_TEST.msg
--rw-r--r--   0        0        0      180 2023-04-03 09:39:47.613417 parse_emails-0.1.8/parse_emails/tests/test_data/chinese_big5_encoding.eml
--rw-r--r--   0        0        0      286 2023-04-03 09:39:47.613417 parse_emails-0.1.8/parse_emails/tests/test_data/chinese_gb2312_encoding.eml
--rw-r--r--   0        0        0      187 2023-04-03 09:39:47.613417 parse_emails-0.1.8/parse_emails/tests/test_data/chinese_gbk_encoding.eml
--rw-r--r--   0        0        0      188 2023-04-03 09:39:47.613417 parse_emails-0.1.8/parse_emails/tests/test_data/chinese_iso_2022_jp_encoding.eml
--rw-r--r--   0        0        0     2361 2023-04-03 09:39:47.613417 parse_emails-0.1.8/parse_emails/tests/test_data/email_with_signed_attachment.eml
--rw-r--r--   0        0        0     2234 2023-04-03 09:39:47.613417 parse_emails-0.1.8/parse_emails/tests/test_data/email_with_special_char_bytes.eml
--rw-r--r--   0        0        0     1803 2023-04-03 09:39:47.613417 parse_emails-0.1.8/parse_emails/tests/test_data/eml_contains_base64_eml.eml
--rw-r--r--   0        0        0     1793 2023-04-03 09:39:47.613417 parse_emails-0.1.8/parse_emails/tests/test_data/eml_contains_base64_eml2.eml
--rw-r--r--   0        0        0     2822 2023-04-03 09:39:47.613417 parse_emails-0.1.8/parse_emails/tests/test_data/eml_contains_emptytxt_htm_file.eml
--rw-r--r--   0        0        0      869 2023-04-03 09:39:47.613417 parse_emails-0.1.8/parse_emails/tests/test_data/eml_contains_htm_attachment.eml
--rw-r--r--   0        0        0   495444 2023-04-03 09:39:47.617417 parse_emails-0.1.8/parse_emails/tests/test_data/eml_contains_image_as_cid.eml
--rw-r--r--   0        0        0     1794 2023-04-03 09:39:47.617417 parse_emails-0.1.8/parse_emails/tests/test_data/eml_with_special_utf_8_chars.eml
--rw-r--r--   0        0        0     7010 2023-04-03 09:39:47.617417 parse_emails-0.1.8/parse_emails/tests/test_data/file_with_a_long_subject_and_special_characters.eml
--rw-r--r--   0        0        0    19456 2023-04-03 09:39:47.617417 parse_emails-0.1.8/parse_emails/tests/test_data/html_attachment.msg
--rw-r--r--   0        0        0   359231 2023-04-03 09:39:47.617417 parse_emails-0.1.8/parse_emails/tests/test_data/image.jpg
--rw-r--r--   0        0        0      700 2023-04-03 09:39:47.617417 parse_emails-0.1.8/parse_emails/tests/test_data/invalid_message_id.eml
--rw-r--r--   0        0        0    13312 2023-04-03 09:39:47.617417 parse_emails-0.1.8/parse_emails/tests/test_data/msg_contains_eml.msg
--rw-r--r--   0        0        0  4063744 2023-04-03 09:39:47.633417 parse_emails-0.1.8/parse_emails/tests/test_data/msg_with_rtf_compressed.msg
--rw-r--r--   0        0        0     2445 2023-04-03 09:39:47.633417 parse_emails-0.1.8/parse_emails/tests/test_data/multipart_alternative_format.p7m
--rw-r--r--   0        0        0    44092 2023-04-03 09:39:47.633417 parse_emails-0.1.8/parse_emails/tests/test_data/multipart_mixed_format.p7m
--rw-r--r--   0        0        0    44094 2023-04-03 09:39:47.633417 parse_emails-0.1.8/parse_emails/tests/test_data/multipart_related_format.p7m
--rw-r--r--   0        0        0   402039 2023-04-03 09:39:47.637417 parse_emails-0.1.8/parse_emails/tests/test_data/multipart_related_format_old.p7m
--rw-r--r--   0        0        0    11782 2023-04-03 09:39:47.637417 parse_emails-0.1.8/parse_emails/tests/test_data/multiple_to_cc.eml
--rw-r--r--   0        0        0    11822 2023-04-03 09:39:47.637417 parse_emails-0.1.8/parse_emails/tests/test_data/multiple_to_cc_from_Cyrillic_characters.eml
--rw-r--r--   0        0        0     4967 2023-04-03 09:39:47.637417 parse_emails-0.1.8/parse_emails/tests/test_data/new-line-in-parts.eml
--rw-r--r--   0        0        0        0 2023-04-03 09:39:47.637417 parse_emails-0.1.8/parse_emails/tests/test_data/no_content.eml
--rw-r--r--   0        0        0      148 2023-04-03 09:39:47.637417 parse_emails-0.1.8/parse_emails/tests/test_data/no_content_type.eml
--rw-r--r--   0        0        0    17408 2023-04-03 09:39:47.637417 parse_emails-0.1.8/parse_emails/tests/test_data/smime-p7s.msg
--rw-r--r--   0        0        0     7333 2023-04-03 09:39:47.637417 parse_emails-0.1.8/parse_emails/tests/test_data/smime.p7m
--rw-r--r--   0        0        0     6804 2023-04-03 09:39:47.637417 parse_emails-0.1.8/parse_emails/tests/test_data/smime2.p7m
--rw-r--r--   0        0        0     7391 2023-04-03 09:39:47.637417 parse_emails-0.1.8/parse_emails/tests/test_data/smime_mime_entity_ascii_crlf.p7m
--rw-r--r--   0        0        0      688 2023-04-03 09:39:47.637417 parse_emails-0.1.8/parse_emails/tests/test_data/smtp_email_type.eml
--rw-r--r--   0        0        0      751 2023-04-03 09:39:47.637417 parse_emails-0.1.8/parse_emails/tests/test_data/smtp_envelope_headers.eml
--rw-r--r--   0        0        0     9754 2023-04-03 09:39:47.637417 parse_emails-0.1.8/parse_emails/tests/test_data/test-eml-text-html.eml
--rw-r--r--   0        0        0      965 2023-04-03 09:39:47.637417 parse_emails-0.1.8/parse_emails/tests/test_data/utf_8_email.eml
--rw-r--r--   0        0        0      969 2023-04-03 09:39:47.637417 parse_emails-0.1.8/parse_emails/tests/test_data/utf_8_with_bom.eml
--rw-r--r--   0        0        0    42496 2023-04-03 09:39:47.637417 parse_emails-0.1.8/parse_emails/tests/test_data/utf_subject.msg
--rw-r--r--   0        0        0     1007 2023-04-03 09:39:47.637417 parse_emails-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     3167 1970-01-01 00:00:00.000000 parse_emails-0.1.8/setup.py
--rw-r--r--   0        0        0     3374 1970-01-01 00:00:00.000000 parse_emails-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-05-15 15:20:36.556240 parse_emails-0.1.9/LICENSE
+-rw-r--r--   0        0        0     2328 2023-05-15 15:20:36.556240 parse_emails-0.1.9/README.md
+-rw-r--r--   0        0        0       50 2023-05-15 15:20:36.560240 parse_emails-0.1.9/parse_emails/__init__.py
+-rw-r--r--   0        0        0     2290 2023-05-15 15:20:36.560240 parse_emails-0.1.9/parse_emails/common.py
+-rw-r--r--   0        0        0    49697 2023-05-15 15:20:36.560240 parse_emails-0.1.9/parse_emails/constants.py
+-rw-r--r--   0        0        0    20567 2023-05-15 15:20:36.560240 parse_emails-0.1.9/parse_emails/handle_eml.py
+-rw-r--r--   0        0        0    39800 2023-05-15 15:20:36.560240 parse_emails-0.1.9/parse_emails/handle_msg.py
+-rw-r--r--   0        0        0    10790 2023-05-15 15:20:36.560240 parse_emails-0.1.9/parse_emails/parse_emails.py
+-rw-r--r--   0        0        0        0 2023-05-15 15:20:36.560240 parse_emails-0.1.9/parse_emails/tests/__init__.py
+-rw-r--r--   0        0        0    29889 2023-05-15 15:20:36.560240 parse_emails-0.1.9/parse_emails/tests/parse_emails_test.py
+-rw-r--r--   0        0        0    69301 2023-05-15 15:20:36.560240 parse_emails-0.1.9/parse_emails/tests/test_data/DONT_OPEN-MALICIOUS.eml
+-rw-r--r--   0        0        0    69303 2023-05-15 15:20:36.560240 parse_emails-0.1.9/parse_emails/tests/test_data/DONT_OPEN-MALICIOUS_base64_headers.eml
+-rw-r--r--   0        0        0 14960583 2023-05-15 15:20:36.644240 parse_emails-0.1.9/parse_emails/tests/test_data/Fwd_test-inner_attachment_eml.eml
+-rw-r--r--   0        0        0     6500 2023-05-15 15:20:36.644240 parse_emails-0.1.9/parse_emails/tests/test_data/ParseEmailFiles-test-emls.eml
+-rw-r--r--   0        0        0    23552 2023-05-15 15:20:36.644240 parse_emails-0.1.9/parse_emails/tests/test_data/Phishing_TEST.msg
+-rw-r--r--   0        0        0      180 2023-05-15 15:20:36.644240 parse_emails-0.1.9/parse_emails/tests/test_data/chinese_big5_encoding.eml
+-rw-r--r--   0        0        0      286 2023-05-15 15:20:36.644240 parse_emails-0.1.9/parse_emails/tests/test_data/chinese_gb2312_encoding.eml
+-rw-r--r--   0        0        0      187 2023-05-15 15:20:36.644240 parse_emails-0.1.9/parse_emails/tests/test_data/chinese_gbk_encoding.eml
+-rw-r--r--   0        0        0      188 2023-05-15 15:20:36.644240 parse_emails-0.1.9/parse_emails/tests/test_data/chinese_iso_2022_jp_encoding.eml
+-rw-r--r--   0        0        0     2361 2023-05-15 15:20:36.644240 parse_emails-0.1.9/parse_emails/tests/test_data/email_with_signed_attachment.eml
+-rw-r--r--   0        0        0     2234 2023-05-15 15:20:36.644240 parse_emails-0.1.9/parse_emails/tests/test_data/email_with_special_char_bytes.eml
+-rw-r--r--   0        0        0     1803 2023-05-15 15:20:36.644240 parse_emails-0.1.9/parse_emails/tests/test_data/eml_contains_base64_eml.eml
+-rw-r--r--   0        0        0     1793 2023-05-15 15:20:36.644240 parse_emails-0.1.9/parse_emails/tests/test_data/eml_contains_base64_eml2.eml
+-rw-r--r--   0        0        0     2822 2023-05-15 15:20:36.644240 parse_emails-0.1.9/parse_emails/tests/test_data/eml_contains_emptytxt_htm_file.eml
+-rw-r--r--   0        0        0      869 2023-05-15 15:20:36.644240 parse_emails-0.1.9/parse_emails/tests/test_data/eml_contains_htm_attachment.eml
+-rw-r--r--   0        0        0   495444 2023-05-15 15:20:36.648239 parse_emails-0.1.9/parse_emails/tests/test_data/eml_contains_image_as_cid.eml
+-rw-r--r--   0        0        0      936 2023-05-15 15:20:36.648239 parse_emails-0.1.9/parse_emails/tests/test_data/eml_non_ascii.eml
+-rw-r--r--   0        0        0     1794 2023-05-15 15:20:36.648239 parse_emails-0.1.9/parse_emails/tests/test_data/eml_with_special_utf_8_chars.eml
+-rw-r--r--   0        0        0     7010 2023-05-15 15:20:36.648239 parse_emails-0.1.9/parse_emails/tests/test_data/file_with_a_long_subject_and_special_characters.eml
+-rw-r--r--   0        0        0    19456 2023-05-15 15:20:36.648239 parse_emails-0.1.9/parse_emails/tests/test_data/html_attachment.msg
+-rw-r--r--   0        0        0   359231 2023-05-15 15:20:36.648239 parse_emails-0.1.9/parse_emails/tests/test_data/image.jpg
+-rw-r--r--   0        0        0      700 2023-05-15 15:20:36.648239 parse_emails-0.1.9/parse_emails/tests/test_data/invalid_message_id.eml
+-rw-r--r--   0        0        0    13312 2023-05-15 15:20:36.648239 parse_emails-0.1.9/parse_emails/tests/test_data/msg_contains_eml.msg
+-rw-r--r--   0        0        0  4063744 2023-05-15 15:20:36.660240 parse_emails-0.1.9/parse_emails/tests/test_data/msg_with_rtf_compressed.msg
+-rw-r--r--   0        0        0     2445 2023-05-15 15:20:36.660240 parse_emails-0.1.9/parse_emails/tests/test_data/multipart_alternative_format.p7m
+-rw-r--r--   0        0        0    44092 2023-05-15 15:20:36.660240 parse_emails-0.1.9/parse_emails/tests/test_data/multipart_mixed_format.p7m
+-rw-r--r--   0        0        0    44094 2023-05-15 15:20:36.660240 parse_emails-0.1.9/parse_emails/tests/test_data/multipart_related_format.p7m
+-rw-r--r--   0        0        0   402039 2023-05-15 15:20:36.664240 parse_emails-0.1.9/parse_emails/tests/test_data/multipart_related_format_old.p7m
+-rw-r--r--   0        0        0    11782 2023-05-15 15:20:36.664240 parse_emails-0.1.9/parse_emails/tests/test_data/multiple_to_cc.eml
+-rw-r--r--   0        0        0    11822 2023-05-15 15:20:36.664240 parse_emails-0.1.9/parse_emails/tests/test_data/multiple_to_cc_from_Cyrillic_characters.eml
+-rw-r--r--   0        0        0     4967 2023-05-15 15:20:36.664240 parse_emails-0.1.9/parse_emails/tests/test_data/new-line-in-parts.eml
+-rw-r--r--   0        0        0        0 2023-05-15 15:20:36.664240 parse_emails-0.1.9/parse_emails/tests/test_data/no_content.eml
+-rw-r--r--   0        0        0      148 2023-05-15 15:20:36.664240 parse_emails-0.1.9/parse_emails/tests/test_data/no_content_type.eml
+-rw-r--r--   0        0        0    17408 2023-05-15 15:20:36.664240 parse_emails-0.1.9/parse_emails/tests/test_data/smime-p7s.msg
+-rw-r--r--   0        0        0     7333 2023-05-15 15:20:36.664240 parse_emails-0.1.9/parse_emails/tests/test_data/smime.p7m
+-rw-r--r--   0        0        0     6804 2023-05-15 15:20:36.664240 parse_emails-0.1.9/parse_emails/tests/test_data/smime2.p7m
+-rw-r--r--   0        0        0     7391 2023-05-15 15:20:36.664240 parse_emails-0.1.9/parse_emails/tests/test_data/smime_mime_entity_ascii_crlf.p7m
+-rw-r--r--   0        0        0      688 2023-05-15 15:20:36.664240 parse_emails-0.1.9/parse_emails/tests/test_data/smtp_email_type.eml
+-rw-r--r--   0        0        0      751 2023-05-15 15:20:36.664240 parse_emails-0.1.9/parse_emails/tests/test_data/smtp_envelope_headers.eml
+-rw-r--r--   0        0        0     9754 2023-05-15 15:20:36.664240 parse_emails-0.1.9/parse_emails/tests/test_data/test-eml-text-html.eml
+-rw-r--r--   0        0        0      965 2023-05-15 15:20:36.664240 parse_emails-0.1.9/parse_emails/tests/test_data/utf_8_email.eml
+-rw-r--r--   0        0        0      969 2023-05-15 15:20:36.664240 parse_emails-0.1.9/parse_emails/tests/test_data/utf_8_with_bom.eml
+-rw-r--r--   0        0        0    42496 2023-05-15 15:20:36.664240 parse_emails-0.1.9/parse_emails/tests/test_data/utf_subject.msg
+-rw-r--r--   0        0        0     1007 2023-05-15 15:20:36.664240 parse_emails-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     3374 1970-01-01 00:00:00.000000 parse_emails-0.1.9/PKG-INFO
```

### Comparing `parse_emails-0.1.8/LICENSE` & `parse_emails-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `parse_emails-0.1.8/README.md` & `parse_emails-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `parse_emails-0.1.8/parse_emails/common.py` & `parse_emails-0.1.9/parse_emails/common.py`

 * *Files identical despite different names*

### Comparing `parse_emails-0.1.8/parse_emails/constants.py` & `parse_emails-0.1.9/parse_emails/constants.py`

 * *Files identical despite different names*

### Comparing `parse_emails-0.1.8/parse_emails/handle_eml.py` & `parse_emails-0.1.9/parse_emails/handle_eml.py`

 * *Files identical despite different names*

### Comparing `parse_emails-0.1.8/parse_emails/handle_msg.py` & `parse_emails-0.1.9/parse_emails/handle_msg.py`

 * *Files identical despite different names*

### Comparing `parse_emails-0.1.8/parse_emails/parse_emails.py` & `parse_emails-0.1.9/parse_emails/parse_emails.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,14 +72,17 @@
         global DEFAULT_ENCODING
 
         USER_ENCODING = self._forced_encoding
         DEFAULT_ENCODING = self._default_encoding
 
         try:
             file_type_lower = self._file_type.lower()
+            is_eml_ext = False
+            if self._file_name and self._file_name.lower().strip().endswith('.eml'):
+                is_eml_ext = True
             if self._is_msg:
                 email_data, attached_emails, attached_eml = handle_msg(self._file_path, self._file_name,
                                                                        self._parse_only_headers,
                                                                        self._max_depth, original_depth=self._max_depth)
                 if attached_eml:
                     attached_eml = parse_inner_eml(attachments=attached_eml, original_depth=self._max_depth)
                     attached_emails += attached_eml
@@ -92,22 +95,22 @@
                     self._bom = True
                 email_data, attached_emails = handle_eml(
                     self._file_path, False, self._file_name, self._parse_only_headers, self._max_depth, bom=self._bom,
                     original_depth=self._max_depth)
                 output = create_email_output(email_data, attached_emails)
 
             elif ('ascii text' in file_type_lower or 'unicode text' in file_type_lower or
-                  ('data' == file_type_lower.strip() and self._file_name and
-                   self._file_name.lower().strip().endswith('.eml'))):
+                  ('data' == file_type_lower.strip() and is_eml_ext)):
                 try:
                     # Try to open the email as-is
                     with open(self._file_path, encoding='utf-8', errors='replace') as f:
                         file_contents = f.read()
 
-                    if file_contents and 'Content-Type:'.lower() in file_contents.lower():
+                    if (file_contents and 'Content-Type:'.lower() in file_contents.lower()) or (is_eml_ext and not
+                                                                                                all(ord(char) < 128 for char in file_contents)):
                         email_data, attached_emails = handle_eml(self._file_path, b64=False, file_name=self._file_name,
                                                                  parse_only_headers=self._parse_only_headers,
                                                                  max_depth=self._max_depth, original_depth=self._max_depth)
                         output = create_email_output(email_data, attached_emails)
                     else:
                         # Try a base64 decode
                         b64decode(file_contents)
```

### Comparing `parse_emails-0.1.8/parse_emails/tests/parse_emails_test.py` & `parse_emails-0.1.9/parse_emails/tests/parse_emails_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,14 +70,25 @@
     results = EmailParser(file_path=test_path, max_depth=3, parse_only_headers=False, file_info=test_type)
     results.parse()
 
     assert isinstance(results.parsed_email, dict)
     assert results.parsed_email['Subject'] == 'Test Smtp Email'
 
 
+def test_eml_non_ascii():
+    test_path = 'parse_emails/tests/test_data/eml_non_ascii.eml'
+    test_type = 'news or mail text, Non-ISO extended-ASCII text, with CRLF line terminators'
+
+    results = EmailParser(file_path=test_path, max_depth=3, parse_only_headers=False, file_info=test_type)
+    results.parse()
+
+    assert isinstance(results.parsed_email, dict)
+    assert results.parsed_email['Subject'] == 'Test Non Ascii'
+
+
 # this is a test for another version of a multipart signed eml file
 def test_smime2():
 
     test_path = 'parse_emails/tests/test_data/smime2.p7m'
     test_type = 'multipart/signed; protocol="application/pkcs7-signature";, ASCII text, with CRLF line terminators'
 
     results = EmailParser(file_path=test_path, max_depth=3, parse_only_headers=False, file_info=test_type)
```

### Comparing `parse_emails-0.1.8/parse_emails/tests/test_data/DONT_OPEN-MALICIOUS.eml` & `parse_emails-0.1.9/parse_emails/tests/test_data/DONT_OPEN-MALICIOUS.eml`

 * *Files identical despite different names*

### Comparing `parse_emails-0.1.8/parse_emails/tests/test_data/DONT_OPEN-MALICIOUS_base64_headers.eml` & `parse_emails-0.1.9/parse_emails/tests/test_data/DONT_OPEN-MALICIOUS_base64_headers.eml`

 * *Files identical despite different names*

### Comparing `parse_emails-0.1.8/parse_emails/tests/test_data/Fwd_test-inner_attachment_eml.eml` & `parse_emails-0.1.9/parse_emails/tests/test_data/Fwd_test-inner_attachment_eml.eml`

 * *Files identical despite different names*

### Comparing `parse_emails-0.1.8/parse_emails/tests/test_data/ParseEmailFiles-test-emls.eml` & `parse_emails-0.1.9/parse_emails/tests/test_data/ParseEmailFiles-test-emls.eml`

 * *Files identical despite different names*

### Comparing `parse_emails-0.1.8/parse_emails/tests/test_data/Phishing_TEST.msg` & `parse_emails-0.1.9/parse_emails/tests/test_data/Phishing_TEST.msg`

 * *Files identical despite different names*

### Comparing `parse_emails-0.1.8/parse_emails/tests/test_data/email_with_signed_attachment.eml` & `parse_emails-0.1.9/parse_emails/tests/test_data/email_with_signed_attachment.eml`

 * *Files identical despite different names*

### Comparing `parse_emails-0.1.8/parse_emails/tests/test_data/email_with_special_char_bytes.eml` & `parse_emails-0.1.9/parse_emails/tests/test_data/email_with_special_char_bytes.eml`

 * *Files identical despite different names*

### Comparing `parse_emails-0.1.8/parse_emails/tests/test_data/eml_contains_base64_eml.eml` & `parse_emails-0.1.9/parse_emails/tests/test_data/eml_contains_base64_eml.eml`

 * *Files identical despite different names*

### Comparing `parse_emails-0.1.8/parse_emails/tests/test_data/eml_contains_base64_eml2.eml` & `parse_emails-0.1.9/parse_emails/tests/test_data/eml_contains_base64_eml2.eml`

 * *Files identical despite different names*

### Comparing `parse_emails-0.1.8/parse_emails/tests/test_data/eml_contains_emptytxt_htm_file.eml` & `parse_emails-0.1.9/parse_emails/tests/test_data/eml_contains_emptytxt_htm_file.eml`

 * *Files identical despite different names*

### Comparing `parse_emails-0.1.8/parse_emails/tests/test_data/eml_contains_htm_attachment.eml` & `parse_emails-0.1.9/parse_emails/tests/test_data/eml_contains_htm_attachment.eml`

 * *Files identical despite different names*

### Comparing `parse_emails-0.1.8/parse_emails/tests/test_data/eml_contains_image_as_cid.eml` & `parse_emails-0.1.9/parse_emails/tests/test_data/eml_contains_image_as_cid.eml`

 * *Files identical despite different names*

### Comparing `parse_emails-0.1.8/parse_emails/tests/test_data/eml_with_special_utf_8_chars.eml` & `parse_emails-0.1.9/parse_emails/tests/test_data/eml_with_special_utf_8_chars.eml`

 * *Files identical despite different names*

### Comparing `parse_emails-0.1.8/parse_emails/tests/test_data/file_with_a_long_subject_and_special_characters.eml` & `parse_emails-0.1.9/parse_emails/tests/test_data/file_with_a_long_subject_and_special_characters.eml`

 * *Files identical despite different names*

### Comparing `parse_emails-0.1.8/parse_emails/tests/test_data/html_attachment.msg` & `parse_emails-0.1.9/parse_emails/tests/test_data/html_attachment.msg`

 * *Files identical despite different names*

### Comparing `parse_emails-0.1.8/parse_emails/tests/test_data/image.jpg` & `parse_emails-0.1.9/parse_emails/tests/test_data/image.jpg`

 * *Files identical despite different names*

### Comparing `parse_emails-0.1.8/parse_emails/tests/test_data/invalid_message_id.eml` & `parse_emails-0.1.9/parse_emails/tests/test_data/invalid_message_id.eml`

 * *Files identical despite different names*

### Comparing `parse_emails-0.1.8/parse_emails/tests/test_data/msg_contains_eml.msg` & `parse_emails-0.1.9/parse_emails/tests/test_data/msg_contains_eml.msg`

 * *Files identical despite different names*

### Comparing `parse_emails-0.1.8/parse_emails/tests/test_data/msg_with_rtf_compressed.msg` & `parse_emails-0.1.9/parse_emails/tests/test_data/msg_with_rtf_compressed.msg`

 * *Files identical despite different names*

### Comparing `parse_emails-0.1.8/parse_emails/tests/test_data/multipart_alternative_format.p7m` & `parse_emails-0.1.9/parse_emails/tests/test_data/multipart_alternative_format.p7m`

 * *Files identical despite different names*

### Comparing `parse_emails-0.1.8/parse_emails/tests/test_data/multipart_mixed_format.p7m` & `parse_emails-0.1.9/parse_emails/tests/test_data/multipart_mixed_format.p7m`

 * *Files identical despite different names*

### Comparing `parse_emails-0.1.8/parse_emails/tests/test_data/multipart_related_format.p7m` & `parse_emails-0.1.9/parse_emails/tests/test_data/multipart_related_format.p7m`

 * *Files identical despite different names*

### Comparing `parse_emails-0.1.8/parse_emails/tests/test_data/multipart_related_format_old.p7m` & `parse_emails-0.1.9/parse_emails/tests/test_data/multipart_related_format_old.p7m`

 * *Files identical despite different names*

### Comparing `parse_emails-0.1.8/parse_emails/tests/test_data/multiple_to_cc.eml` & `parse_emails-0.1.9/parse_emails/tests/test_data/multiple_to_cc.eml`

 * *Files identical despite different names*

### Comparing `parse_emails-0.1.8/parse_emails/tests/test_data/multiple_to_cc_from_Cyrillic_characters.eml` & `parse_emails-0.1.9/parse_emails/tests/test_data/multiple_to_cc_from_Cyrillic_characters.eml`

 * *Files identical despite different names*

### Comparing `parse_emails-0.1.8/parse_emails/tests/test_data/new-line-in-parts.eml` & `parse_emails-0.1.9/parse_emails/tests/test_data/new-line-in-parts.eml`

 * *Files identical despite different names*

### Comparing `parse_emails-0.1.8/parse_emails/tests/test_data/smime-p7s.msg` & `parse_emails-0.1.9/parse_emails/tests/test_data/smime-p7s.msg`

 * *Files identical despite different names*

### Comparing `parse_emails-0.1.8/parse_emails/tests/test_data/smime.p7m` & `parse_emails-0.1.9/parse_emails/tests/test_data/smime.p7m`

 * *Files identical despite different names*

### Comparing `parse_emails-0.1.8/parse_emails/tests/test_data/smime2.p7m` & `parse_emails-0.1.9/parse_emails/tests/test_data/smime2.p7m`

 * *Files identical despite different names*

### Comparing `parse_emails-0.1.8/parse_emails/tests/test_data/smime_mime_entity_ascii_crlf.p7m` & `parse_emails-0.1.9/parse_emails/tests/test_data/smime_mime_entity_ascii_crlf.p7m`

 * *Files identical despite different names*

### Comparing `parse_emails-0.1.8/parse_emails/tests/test_data/smtp_email_type.eml` & `parse_emails-0.1.9/parse_emails/tests/test_data/smtp_email_type.eml`

 * *Files identical despite different names*

### Comparing `parse_emails-0.1.8/parse_emails/tests/test_data/smtp_envelope_headers.eml` & `parse_emails-0.1.9/parse_emails/tests/test_data/smtp_envelope_headers.eml`

 * *Files identical despite different names*

### Comparing `parse_emails-0.1.8/parse_emails/tests/test_data/test-eml-text-html.eml` & `parse_emails-0.1.9/parse_emails/tests/test_data/test-eml-text-html.eml`

 * *Files identical despite different names*

### Comparing `parse_emails-0.1.8/parse_emails/tests/test_data/utf_8_email.eml` & `parse_emails-0.1.9/parse_emails/tests/test_data/utf_8_email.eml`

 * *Files identical despite different names*

### Comparing `parse_emails-0.1.8/parse_emails/tests/test_data/utf_8_with_bom.eml` & `parse_emails-0.1.9/parse_emails/tests/test_data/utf_8_with_bom.eml`

 * *Files identical despite different names*

### Comparing `parse_emails-0.1.8/parse_emails/tests/test_data/utf_subject.msg` & `parse_emails-0.1.9/parse_emails/tests/test_data/utf_subject.msg`

 * *Files identical despite different names*

### Comparing `parse_emails-0.1.8/pyproject.toml` & `parse_emails-0.1.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "parse-emails"
-version = "0.1.8"
+version = "0.1.9"
 description = "Parses an email message file and extracts the data from it."
 authors = ["Demisto"]
 license = "MIT"
 classifiers=[
     'Intended Audience :: Developers',
     'Natural Language :: English',
     'License :: OSI Approved :: MIT License',
```

### Comparing `parse_emails-0.1.8/PKG-INFO` & `parse_emails-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: parse-emails
-Version: 0.1.8
+Version: 0.1.9
 Summary: Parses an email message file and extracts the data from it.
 License: MIT
 Author: Demisto
 Requires-Python: >=3.7,<4.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
```

