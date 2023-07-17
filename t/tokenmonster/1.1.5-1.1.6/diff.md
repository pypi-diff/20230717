# Comparing `tmp/tokenmonster-1.1.5.tar.gz` & `tmp/tokenmonster-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tokenmonster-1.1.5.tar", last modified: Thu Jul 13 12:47:52 2023, max compression
+gzip compressed data, was "tokenmonster-1.1.6.tar", last modified: Mon Jul 17 03:36:01 2023, max compression
```

## Comparing `tokenmonster-1.1.5.tar` & `tokenmonster-1.1.6.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 12:47:52.938187 tokenmonster-1.1.5/
--rw-r--r--   0 root         (0) root         (0)    16622 2023-07-13 12:47:52.938187 tokenmonster-1.1.5/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    16887 2023-07-12 14:01:39.000000 tokenmonster-1.1.5/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-13 12:47:52.938187 tokenmonster-1.1.5/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      550 2023-07-13 12:45:02.000000 tokenmonster-1.1.5/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 12:47:52.938187 tokenmonster-1.1.5/tokenmonster.egg-info/
--rw-r--r--   0 root         (0) root         (0)    16622 2023-07-13 12:47:52.000000 tokenmonster-1.1.5/tokenmonster.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      178 2023-07-13 12:47:52.000000 tokenmonster-1.1.5/tokenmonster.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-13 12:47:52.000000 tokenmonster-1.1.5/tokenmonster.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-13 12:47:52.000000 tokenmonster-1.1.5/tokenmonster.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)    49113 2023-07-13 12:41:46.000000 tokenmonster-1.1.5/tokenmonster.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 03:36:01.471752 tokenmonster-1.1.6/
+-rw-r--r--   0 root         (0) root         (0)    15947 2023-07-17 03:36:01.471752 tokenmonster-1.1.6/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    16189 2023-07-17 03:31:00.000000 tokenmonster-1.1.6/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-17 03:36:01.471752 tokenmonster-1.1.6/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      550 2023-07-17 03:30:42.000000 tokenmonster-1.1.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 03:36:01.471752 tokenmonster-1.1.6/tokenmonster.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    15947 2023-07-17 03:36:01.000000 tokenmonster-1.1.6/tokenmonster.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      178 2023-07-17 03:36:01.000000 tokenmonster-1.1.6/tokenmonster.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-17 03:36:01.000000 tokenmonster-1.1.6/tokenmonster.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-17 03:36:01.000000 tokenmonster-1.1.6/tokenmonster.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)    48319 2023-07-17 03:28:52.000000 tokenmonster-1.1.6/tokenmonster.py
```

### Comparing `tokenmonster-1.1.5/PKG-INFO` & `tokenmonster-1.1.6/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tokenmonster
-Version: 1.1.5
+Version: 1.1.6
 Summary: Tokenize and decode text with TokenMonster vocabularies.
 Home-page: https://github.com/alasdairforsythe/tokenmonster
 Author: Alasdair Forsythe
 Author-email: 77910352+alasdairforsythe@users.noreply.github.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
@@ -27,31 +27,29 @@
     - [len(vocab)](#lenvocab)
     - [vocab.get_dictionary()](#vocabget_dictionary)
     - [vocab.charset()](#vocabcharset)
     - [vocab.normalization()](#vocabnormalization)
     - [vocab.capcode()](#vocabcapcode)
     - [vocab.mode()](#vocabmode)
     - [vocab.unk_token_id()](#vocabunk_token_id)
-    - [vocab.convert_ids_to_tokens(ids)](#vocabconvert_ids_to_tokensids)
-    - [vocab.convert_ids_to_tokens_decoded(ids)](#vocabconvert_ids_to_tokens_decodedids)
     - [vocab.id_to_token(id)](#vocabid_to_tokenid)
     - [vocab.id_to_token_decoded(id)](#vocabid_to_token_decodedid)
     - [vocab.token_to_id(token)](#vocabtoken_to_idtoken)
-    - [vocab.convert_tokens_to_ids(tokens)](#vocabconvert_tokens_to_idstokens)
 5. Vocabulary Modification
     - [vocab.modify(add_special_tokens, add_regular_tokens=None, delete_tokens=None, resize=None, change_unk=None)](#vocabmodifyadd_special_tokens-add_regular_tokensnone-delete_tokensnone-resizenone-change_unknone-reset_token_idsfalse)
     - [vocab.add_token(token)](#vocabadd_tokentoken)
     - [vocab.delete_token(token)](#vocabdelete_tokentoken)
     - [vocab.delete_token_by_id(id)](#vocabdelete_token_by_idid)
     - [vocab.add_special_token(token)](#vocabadd_special_tokentoken)
     - [vocab.resize(size)](#vocabresizesize-reset_token_idsfalse)
     - [vocab.reset_token_ids()](#vocabreset_token_ids)
     - [vocab.enable_unk_token()](#vocabenable_unk_token)
     - [vocab.disable_unk_token()](#vocabdisable_unk_token)
 6. Other
+    - [del](#del)
     - [tokenmonster.set_local_directory(dir=None)](#tokenmonsterset_local_directorydirnone)
     - [tokenmonster.disconnect()](#tokenmonsterdisconnect)
     - [vocab.serialize_tokens(integer_list)](#vocabserialize_tokensinteger_list)
     - [vocab.deserialize_tokens(binary_string)](#vocabdeserialize_tokensbinary_string)
 
 ## Usage
 
@@ -156,26 +154,30 @@
 
 #### Parameters
 
 - `text` (string or list of strings): A string or bytes string, or list of strings or bytes strings.
 
 #### Returns
 
-- `tokens` (list of ints or list of list of ints): The tokens IDs
+- `tokens` (numpy array or list of numpy array): The tokens IDs
 
 #### Usage
 
 ```python
 tokens = vocab.tokenize(text)
 ```
 
 ### vocab.tokenize_count(text)
 
 Same as tokenize, but it returns only the number of tokens.
 
+The number of tokens is the same as you would get from `tokenize`. If you want to count any characters
+for which there are no tokens or single byte tokens, you should `enable_unk_token()`. It's okay to
+enable `enable_unk_token()`, run `tokenize_count` and then `disable_unk_token()`.
+
 #### Parameters
 
 - `text` (string or list of strings): A string or bytes string, or list of strings or bytes strings.
 
 #### Returns
 
 - `n_tokens` (int or list of ints): The number of tokens for each input string
@@ -192,15 +194,15 @@
 
 Only use this "decode" method if you are decoding a complete "batch" or complete "conversation" in one go.
 For decoding an incomplete batch sequentially (as the tokens become available) instead
 use the decoder object.
 
 #### Parameters
 
-- `tokens` (int or list of int): The tokens to decode into a string.
+- `tokens` (int, list of int, or numpy array): The tokens to decode into a string.
 
 #### Returns
 
 - `string`: The composed string from the input tokens.
 
 #### Usage
 
@@ -308,38 +310,14 @@
 
 Returns the ID of the UNK token, or 'None' type if there is no UNK token.
 
 #### Returns
 
 - `int or None`: The ID of the UNK token. None if there is no UNK token.
 
-### vocab.convert_ids_to_tokens(ids)
-
-Get the token string from any token ID, in its capcode-encoded form.
-
-#### Parameters
-
-- `ids` (int or list of ints): The token IDs.
-
-#### Returns
-
-- `list of strings`: The token strings corresponding to the input IDs. None type for any IDs that are not in the vocabulary.
-
-### vocab.convert_ids_to_tokens_decoded(ids)
-
-Get the token string from any token IDs, in its capcode-decoded form.
-
-#### Parameters
-
-- `ids` (int or list of ints): The token IDs.
-
-#### Returns
-
-- `list of strings`: The token strings corresponding to the input IDs. None type for any IDs that are not in the vocabulary.
-
 ### vocab.id_to_token(id)
 
 Get the token string from a single token ID, in its capcode-encoded form.
 
 #### Parameters
 
 - `id` (int): The token ID.
@@ -370,28 +348,14 @@
 
 - `token` (string): The token to get the ID for.
 
 #### Returns
 
 - `int or None`: The ID of the token. None if the token is not in the vocabulary.
 
-### vocab.convert_tokens_to_ids(tokens)
-
-Returns the IDs of the corresponding tokens. 'None' for any not in the vocabulary.
-
-This works for both capcode-encoded "raw" tokens and their decoded form.
-
-#### Parameters
-
-- `tokens` (string or list of strings): The tokens to convert to IDs.
-
-#### Returns
-
-- `list of ints`: The token IDs corresponding to the input tokens. None type for any tokens that are not in the vocabulary.
-
 ## Vocabulary Modification
 
 ### vocab.modify(add_special_tokens, add_regular_tokens=None, delete_tokens=None, resize=None, change_unk=None, reset_token_ids=False)
 
 Modifies the vocabulary. Doing so invalidates all decoder objects associated with the
 model before modification.
 
@@ -550,15 +514,15 @@
 decoding tokens in small segments, or one by one, that are part of a longer
 stream of encoded tokens. A new decoder object should be used for each
 stream, then deleted. If you are decoding all tokens in one call, instead of
 in multiple calls, then you can use the vocabulary decode method directly.
 
 #### Parameters
 
-- `tokens` (int or list of ints): A token ID or list of token IDs.
+- `tokens` (int, list of ints, or numpy array): A token ID or list of token IDs.
 
 #### Returns
 
 - `string`: A human-readable string derived from the input tokens.
 
 #### Usage
 
@@ -567,14 +531,27 @@
 decoder = vocab.decoder()
 decoded_string = decoder.decode(tokens)
 decoded_string += decoder.decode(more_tokens)
 ```
 
 ## Other
 
+### del
+
+Once you are finished with a vocab or decoder object, to free it from memory
+use the `del` syntax. This is worthwhile if you are creating many
+temporary decoder objects.
+
+#### Usage
+
+```python
+vocab = tokenmonster.load("english-32000-balanced-v1")
+del vocab
+```
+
 ### tokenmonster.set_local_directory(dir=None)
 
 Sets the local directory for TokenMonster.
 
 If no directory is specified, the default directory is ~/\_tokenmonster
 
 #### Parameters
@@ -593,33 +570,33 @@
 
 #### Returns
 
 - `None`
 
 ### vocab.serialize_tokens(integer_list)
 
-Serializes tokens from a list of ints into a binary string.
+Serializes tokens from a list of ints or numpy array into a binary string.
 The `encoding_length` used is from vocab.encoding_length.
 
 #### Parameters
 
-- `integer_list` (list of ints): The tokens to serialize.
+- `integer_list` (list of ints or numpy array): The tokens to serialize.
 
 #### Returns
 
 - `bytes`: The serialized binary string.
 
 ### vocab.deserialize_tokens(binary_string)
 
-Deserializes a binary string back into a list of ints (tokens).
+Deserializes a binary string into a numpy array of token IDs.
 The `encoding_length` used is from vocab.encoding_length.
 
 #### Parameters
 
 - `binary_string` (bytes): The binary string to deserialize.
 
 #### Returns
 
-- `list of ints`: The deserialized tokens.
+- `np.array`: The deserialized tokens.
 .
```

### Comparing `tokenmonster-1.1.5/README.md` & `tokenmonster-1.1.6/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -16,31 +16,29 @@
     - [len(vocab)](#lenvocab)
     - [vocab.get_dictionary()](#vocabget_dictionary)
     - [vocab.charset()](#vocabcharset)
     - [vocab.normalization()](#vocabnormalization)
     - [vocab.capcode()](#vocabcapcode)
     - [vocab.mode()](#vocabmode)
     - [vocab.unk_token_id()](#vocabunk_token_id)
-    - [vocab.convert_ids_to_tokens(ids)](#vocabconvert_ids_to_tokensids)
-    - [vocab.convert_ids_to_tokens_decoded(ids)](#vocabconvert_ids_to_tokens_decodedids)
     - [vocab.id_to_token(id)](#vocabid_to_tokenid)
     - [vocab.id_to_token_decoded(id)](#vocabid_to_token_decodedid)
     - [vocab.token_to_id(token)](#vocabtoken_to_idtoken)
-    - [vocab.convert_tokens_to_ids(tokens)](#vocabconvert_tokens_to_idstokens)
 5. Vocabulary Modification
     - [vocab.modify(add_special_tokens, add_regular_tokens=None, delete_tokens=None, resize=None, change_unk=None)](#vocabmodifyadd_special_tokens-add_regular_tokensnone-delete_tokensnone-resizenone-change_unknone-reset_token_idsfalse)
     - [vocab.add_token(token)](#vocabadd_tokentoken)
     - [vocab.delete_token(token)](#vocabdelete_tokentoken)
     - [vocab.delete_token_by_id(id)](#vocabdelete_token_by_idid)
     - [vocab.add_special_token(token)](#vocabadd_special_tokentoken)
     - [vocab.resize(size)](#vocabresizesize-reset_token_idsfalse)
     - [vocab.reset_token_ids()](#vocabreset_token_ids)
     - [vocab.enable_unk_token()](#vocabenable_unk_token)
     - [vocab.disable_unk_token()](#vocabdisable_unk_token)
 6. Other
+    - [del](#del)
     - [tokenmonster.set_local_directory(dir=None)](#tokenmonsterset_local_directorydirnone)
     - [tokenmonster.disconnect()](#tokenmonsterdisconnect)
     - [vocab.serialize_tokens(integer_list)](#vocabserialize_tokensinteger_list)
     - [vocab.deserialize_tokens(binary_string)](#vocabdeserialize_tokensbinary_string)
 
 ## Usage
 
@@ -145,26 +143,30 @@
 
 #### Parameters
 
 - `text` (string or list of strings): A string or bytes string, or list of strings or bytes strings.
 
 #### Returns
 
-- `tokens` (list of ints or list of list of ints): The tokens IDs
+- `tokens` (numpy array or list of numpy array): The tokens IDs
 
 #### Usage
 
 ```python
 tokens = vocab.tokenize(text)
 ```
 
 ### vocab.tokenize_count(text)
 
 Same as tokenize, but it returns only the number of tokens.
 
+The number of tokens is the same as you would get from `tokenize`. If you want to count any characters
+for which there are no tokens or single byte tokens, you should `enable_unk_token()`. It's okay to
+enable `enable_unk_token()`, run `tokenize_count` and then `disable_unk_token()`.
+
 #### Parameters
 
 - `text` (string or list of strings): A string or bytes string, or list of strings or bytes strings.
 
 #### Returns
 
 - `n_tokens` (int or list of ints): The number of tokens for each input string
@@ -181,15 +183,15 @@
 
 Only use this "decode" method if you are decoding a complete "batch" or complete "conversation" in one go.
 For decoding an incomplete batch sequentially (as the tokens become available) instead
 use the decoder object.
 
 #### Parameters
 
-- `tokens` (int or list of int): The tokens to decode into a string.
+- `tokens` (int, list of int, or numpy array): The tokens to decode into a string.
 
 #### Returns
 
 - `string`: The composed string from the input tokens.
 
 #### Usage
 
@@ -297,38 +299,14 @@
 
 Returns the ID of the UNK token, or 'None' type if there is no UNK token.
 
 #### Returns
 
 - `int or None`: The ID of the UNK token. None if there is no UNK token.
 
-### vocab.convert_ids_to_tokens(ids)
-
-Get the token string from any token ID, in its capcode-encoded form.
-
-#### Parameters
-
-- `ids` (int or list of ints): The token IDs.
-
-#### Returns
-
-- `list of strings`: The token strings corresponding to the input IDs. None type for any IDs that are not in the vocabulary.
-
-### vocab.convert_ids_to_tokens_decoded(ids)
-
-Get the token string from any token IDs, in its capcode-decoded form.
-
-#### Parameters
-
-- `ids` (int or list of ints): The token IDs.
-
-#### Returns
-
-- `list of strings`: The token strings corresponding to the input IDs. None type for any IDs that are not in the vocabulary.
-
 ### vocab.id_to_token(id)
 
 Get the token string from a single token ID, in its capcode-encoded form.
 
 #### Parameters
 
 - `id` (int): The token ID.
@@ -359,28 +337,14 @@
 
 - `token` (string): The token to get the ID for.
 
 #### Returns
 
 - `int or None`: The ID of the token. None if the token is not in the vocabulary.
 
-### vocab.convert_tokens_to_ids(tokens)
-
-Returns the IDs of the corresponding tokens. 'None' for any not in the vocabulary.
-
-This works for both capcode-encoded "raw" tokens and their decoded form.
-
-#### Parameters
-
-- `tokens` (string or list of strings): The tokens to convert to IDs.
-
-#### Returns
-
-- `list of ints`: The token IDs corresponding to the input tokens. None type for any tokens that are not in the vocabulary.
-
 ## Vocabulary Modification
 
 ### vocab.modify(add_special_tokens, add_regular_tokens=None, delete_tokens=None, resize=None, change_unk=None, reset_token_ids=False)
 
 Modifies the vocabulary. Doing so invalidates all decoder objects associated with the
 model before modification.
 
@@ -539,15 +503,15 @@
 decoding tokens in small segments, or one by one, that are part of a longer
 stream of encoded tokens. A new decoder object should be used for each
 stream, then deleted. If you are decoding all tokens in one call, instead of
 in multiple calls, then you can use the vocabulary decode method directly.
 
 #### Parameters
 
-- `tokens` (int or list of ints): A token ID or list of token IDs.
+- `tokens` (int, list of ints, or numpy array): A token ID or list of token IDs.
 
 #### Returns
 
 - `string`: A human-readable string derived from the input tokens.
 
 #### Usage
 
@@ -556,14 +520,27 @@
 decoder = vocab.decoder()
 decoded_string = decoder.decode(tokens)
 decoded_string += decoder.decode(more_tokens)
 ```
 
 ## Other
 
+### del
+
+Once you are finished with a vocab or decoder object, to free it from memory
+use the `del` syntax. This is worthwhile if you are creating many
+temporary decoder objects.
+
+#### Usage
+
+```python
+vocab = tokenmonster.load("english-32000-balanced-v1")
+del vocab
+```
+
 ### tokenmonster.set_local_directory(dir=None)
 
 Sets the local directory for TokenMonster.
 
 If no directory is specified, the default directory is ~/\_tokenmonster
 
 #### Parameters
@@ -582,31 +559,31 @@
 
 #### Returns
 
 - `None`
 
 ### vocab.serialize_tokens(integer_list)
 
-Serializes tokens from a list of ints into a binary string.
+Serializes tokens from a list of ints or numpy array into a binary string.
 The `encoding_length` used is from vocab.encoding_length.
 
 #### Parameters
 
-- `integer_list` (list of ints): The tokens to serialize.
+- `integer_list` (list of ints or numpy array): The tokens to serialize.
 
 #### Returns
 
 - `bytes`: The serialized binary string.
 
 ### vocab.deserialize_tokens(binary_string)
 
-Deserializes a binary string back into a list of ints (tokens).
+Deserializes a binary string into a numpy array of token IDs.
 The `encoding_length` used is from vocab.encoding_length.
 
 #### Parameters
 
 - `binary_string` (bytes): The binary string to deserialize.
 
 #### Returns
 
-- `list of ints`: The deserialized tokens.
+- `np.array`: The deserialized tokens.
 .
```

### Comparing `tokenmonster-1.1.5/setup.py` & `tokenmonster-1.1.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open('README.md', 'r') as f:
     long_description = f.read()
 
 setup(
     name='tokenmonster',
-    version='1.1.5',
+    version='1.1.6',
     py_modules=['tokenmonster'],
     author='Alasdair Forsythe',
     author_email='77910352+alasdairforsythe@users.noreply.github.com',
     description='Tokenize and decode text with TokenMonster vocabularies.',
     url='https://github.com/alasdairforsythe/tokenmonster',
     license='MIT',
     long_description=long_description,
```

### Comparing `tokenmonster-1.1.5/tokenmonster.egg-info/PKG-INFO` & `tokenmonster-1.1.6/tokenmonster.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tokenmonster
-Version: 1.1.5
+Version: 1.1.6
 Summary: Tokenize and decode text with TokenMonster vocabularies.
 Home-page: https://github.com/alasdairforsythe/tokenmonster
 Author: Alasdair Forsythe
 Author-email: 77910352+alasdairforsythe@users.noreply.github.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
@@ -27,31 +27,29 @@
     - [len(vocab)](#lenvocab)
     - [vocab.get_dictionary()](#vocabget_dictionary)
     - [vocab.charset()](#vocabcharset)
     - [vocab.normalization()](#vocabnormalization)
     - [vocab.capcode()](#vocabcapcode)
     - [vocab.mode()](#vocabmode)
     - [vocab.unk_token_id()](#vocabunk_token_id)
-    - [vocab.convert_ids_to_tokens(ids)](#vocabconvert_ids_to_tokensids)
-    - [vocab.convert_ids_to_tokens_decoded(ids)](#vocabconvert_ids_to_tokens_decodedids)
     - [vocab.id_to_token(id)](#vocabid_to_tokenid)
     - [vocab.id_to_token_decoded(id)](#vocabid_to_token_decodedid)
     - [vocab.token_to_id(token)](#vocabtoken_to_idtoken)
-    - [vocab.convert_tokens_to_ids(tokens)](#vocabconvert_tokens_to_idstokens)
 5. Vocabulary Modification
     - [vocab.modify(add_special_tokens, add_regular_tokens=None, delete_tokens=None, resize=None, change_unk=None)](#vocabmodifyadd_special_tokens-add_regular_tokensnone-delete_tokensnone-resizenone-change_unknone-reset_token_idsfalse)
     - [vocab.add_token(token)](#vocabadd_tokentoken)
     - [vocab.delete_token(token)](#vocabdelete_tokentoken)
     - [vocab.delete_token_by_id(id)](#vocabdelete_token_by_idid)
     - [vocab.add_special_token(token)](#vocabadd_special_tokentoken)
     - [vocab.resize(size)](#vocabresizesize-reset_token_idsfalse)
     - [vocab.reset_token_ids()](#vocabreset_token_ids)
     - [vocab.enable_unk_token()](#vocabenable_unk_token)
     - [vocab.disable_unk_token()](#vocabdisable_unk_token)
 6. Other
+    - [del](#del)
     - [tokenmonster.set_local_directory(dir=None)](#tokenmonsterset_local_directorydirnone)
     - [tokenmonster.disconnect()](#tokenmonsterdisconnect)
     - [vocab.serialize_tokens(integer_list)](#vocabserialize_tokensinteger_list)
     - [vocab.deserialize_tokens(binary_string)](#vocabdeserialize_tokensbinary_string)
 
 ## Usage
 
@@ -156,26 +154,30 @@
 
 #### Parameters
 
 - `text` (string or list of strings): A string or bytes string, or list of strings or bytes strings.
 
 #### Returns
 
-- `tokens` (list of ints or list of list of ints): The tokens IDs
+- `tokens` (numpy array or list of numpy array): The tokens IDs
 
 #### Usage
 
 ```python
 tokens = vocab.tokenize(text)
 ```
 
 ### vocab.tokenize_count(text)
 
 Same as tokenize, but it returns only the number of tokens.
 
+The number of tokens is the same as you would get from `tokenize`. If you want to count any characters
+for which there are no tokens or single byte tokens, you should `enable_unk_token()`. It's okay to
+enable `enable_unk_token()`, run `tokenize_count` and then `disable_unk_token()`.
+
 #### Parameters
 
 - `text` (string or list of strings): A string or bytes string, or list of strings or bytes strings.
 
 #### Returns
 
 - `n_tokens` (int or list of ints): The number of tokens for each input string
@@ -192,15 +194,15 @@
 
 Only use this "decode" method if you are decoding a complete "batch" or complete "conversation" in one go.
 For decoding an incomplete batch sequentially (as the tokens become available) instead
 use the decoder object.
 
 #### Parameters
 
-- `tokens` (int or list of int): The tokens to decode into a string.
+- `tokens` (int, list of int, or numpy array): The tokens to decode into a string.
 
 #### Returns
 
 - `string`: The composed string from the input tokens.
 
 #### Usage
 
@@ -308,38 +310,14 @@
 
 Returns the ID of the UNK token, or 'None' type if there is no UNK token.
 
 #### Returns
 
 - `int or None`: The ID of the UNK token. None if there is no UNK token.
 
-### vocab.convert_ids_to_tokens(ids)
-
-Get the token string from any token ID, in its capcode-encoded form.
-
-#### Parameters
-
-- `ids` (int or list of ints): The token IDs.
-
-#### Returns
-
-- `list of strings`: The token strings corresponding to the input IDs. None type for any IDs that are not in the vocabulary.
-
-### vocab.convert_ids_to_tokens_decoded(ids)
-
-Get the token string from any token IDs, in its capcode-decoded form.
-
-#### Parameters
-
-- `ids` (int or list of ints): The token IDs.
-
-#### Returns
-
-- `list of strings`: The token strings corresponding to the input IDs. None type for any IDs that are not in the vocabulary.
-
 ### vocab.id_to_token(id)
 
 Get the token string from a single token ID, in its capcode-encoded form.
 
 #### Parameters
 
 - `id` (int): The token ID.
@@ -370,28 +348,14 @@
 
 - `token` (string): The token to get the ID for.
 
 #### Returns
 
 - `int or None`: The ID of the token. None if the token is not in the vocabulary.
 
-### vocab.convert_tokens_to_ids(tokens)
-
-Returns the IDs of the corresponding tokens. 'None' for any not in the vocabulary.
-
-This works for both capcode-encoded "raw" tokens and their decoded form.
-
-#### Parameters
-
-- `tokens` (string or list of strings): The tokens to convert to IDs.
-
-#### Returns
-
-- `list of ints`: The token IDs corresponding to the input tokens. None type for any tokens that are not in the vocabulary.
-
 ## Vocabulary Modification
 
 ### vocab.modify(add_special_tokens, add_regular_tokens=None, delete_tokens=None, resize=None, change_unk=None, reset_token_ids=False)
 
 Modifies the vocabulary. Doing so invalidates all decoder objects associated with the
 model before modification.
 
@@ -550,15 +514,15 @@
 decoding tokens in small segments, or one by one, that are part of a longer
 stream of encoded tokens. A new decoder object should be used for each
 stream, then deleted. If you are decoding all tokens in one call, instead of
 in multiple calls, then you can use the vocabulary decode method directly.
 
 #### Parameters
 
-- `tokens` (int or list of ints): A token ID or list of token IDs.
+- `tokens` (int, list of ints, or numpy array): A token ID or list of token IDs.
 
 #### Returns
 
 - `string`: A human-readable string derived from the input tokens.
 
 #### Usage
 
@@ -567,14 +531,27 @@
 decoder = vocab.decoder()
 decoded_string = decoder.decode(tokens)
 decoded_string += decoder.decode(more_tokens)
 ```
 
 ## Other
 
+### del
+
+Once you are finished with a vocab or decoder object, to free it from memory
+use the `del` syntax. This is worthwhile if you are creating many
+temporary decoder objects.
+
+#### Usage
+
+```python
+vocab = tokenmonster.load("english-32000-balanced-v1")
+del vocab
+```
+
 ### tokenmonster.set_local_directory(dir=None)
 
 Sets the local directory for TokenMonster.
 
 If no directory is specified, the default directory is ~/\_tokenmonster
 
 #### Parameters
@@ -593,33 +570,33 @@
 
 #### Returns
 
 - `None`
 
 ### vocab.serialize_tokens(integer_list)
 
-Serializes tokens from a list of ints into a binary string.
+Serializes tokens from a list of ints or numpy array into a binary string.
 The `encoding_length` used is from vocab.encoding_length.
 
 #### Parameters
 
-- `integer_list` (list of ints): The tokens to serialize.
+- `integer_list` (list of ints or numpy array): The tokens to serialize.
 
 #### Returns
 
 - `bytes`: The serialized binary string.
 
 ### vocab.deserialize_tokens(binary_string)
 
-Deserializes a binary string back into a list of ints (tokens).
+Deserializes a binary string into a numpy array of token IDs.
 The `encoding_length` used is from vocab.encoding_length.
 
 #### Parameters
 
 - `binary_string` (bytes): The binary string to deserialize.
 
 #### Returns
 
-- `list of ints`: The deserialized tokens.
+- `np.array`: The deserialized tokens.
 .
```

### Comparing `tokenmonster-1.1.5/tokenmonster.py` & `tokenmonster-1.1.6/tokenmonster.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import numpy as np
 import struct
 import subprocess
 import os
 import urllib.request
 import platform
 import sys
 from collections.abc import Iterable
@@ -121,37 +122,39 @@
             This decoder object is used instead of the vocabulary decode method when you are
             decoding tokens in small segments, or one by one, that are part of a longer
             stream of encoded tokens. A new decoder object should be used for each
             stream, then deleted. If you are decoding all tokens in one call, instead of
             in multiple calls, then you can use the vocabulary decode method directly.
 
             Parameters:
-                tokens (int or list of ints): A token ID or list of token IDs.
+                tokens (int or list of ints or numpy array): A token ID or list of token IDs.
 
             Returns:
                 string: A human-readable string derived from the input tokens.
 
             Usage:
                 vocab = tokenmonster.Load("english-32000-balanced-v1")
                 decoder = vocab.Decoder()
                 decoded_string = decoder.decode(tokens)
                 decoded_string += decoder.decode(more_tokens)
             """
             if self.parent._modified_id != self._modified_id:
                 raise RuntimeError("Access denied to expired tokenmonster.Decoder instance.")
             if is_iterable(tokens):
                 if len(tokens) == 0:
-                    return
+                    return ''
+                if is_iterable(tokens[0]):
+                    raise ValueError("TokenMonster: You can't batch decode on a decoder object, use the vocab decoder for that.")
             else:
                 if isinstance(tokens, int):
                     tokens = [tokens]
+                elif isinstance(tokens, (np.uint16, np.uint32)):
+                    tokens = np.array([tokens])
                 else:
                     raise ValueError("TokenMonster: Decoder decode accepts int or list of ints.")
-            if is_iterable(tokens[0]):
-                raise ValueError("TokenMonster: You can't batch decode on a decoder object, use the vocab decoder for that.")
             payload = self.parent.serialize_tokens(tokens)
             job_type = self.parent.encoding_length + 5
             response = Vocab._communicate(job_type, self.id, len(payload), payload)
             return self.parent._bytes_to_string(response)
         
         def _unload(self):
             if hasattr(self, 'id'):
@@ -313,15 +316,15 @@
         Decodes tokens into a string.
 
         Only use this "decode" method if you are decoding a complete "batch" or complete "conversation".
         For decoding an incomplete batch sequentially (as the tokens become available) instead
         use the decoder object.
 
         Parameters:
-            tokens (int or list of int): The tokens to decode into a string
+            tokens (int or list of int or numpy array): The tokens to decode into a string
 
         Returns:
             string: The composed string from the input tokens.
 
         Usage:
             decoded_string = vocab.decode(tokens)
         """
@@ -333,35 +336,35 @@
         # Parse input
         if is_iterable(tokens):
             if len(tokens) == 0:
                 return
         else:
             if isinstance(tokens, int):
                 tokens = [tokens]
+            elif isinstance(tokens, (np.uint16, np.uint32)):
+                tokens = np.array([tokens])
             else:
-                raise ValueError("TokenMonster: Input to decode must be an int, a list of ints, or a list of list of ints.")
-        if isinstance(tokens[0], int):
+                raise ValueError("TokenMonster: Input to decode must be an int, list of ints, list of lists, or numpy array.")
+        if not is_iterable(tokens[0]):
             data = self.serialize_tokens(tokens)
             payload.append(_write_uint64(len(data)))
             payload.append(data)
             length += len(data) + 8
             single = True
-        elif is_iterable(tokens[0]):
+        else:
             batch_size = len(tokens)
             single = False
             for _, item in enumerate(tokens):
-                if isinstance(item, int):
+                if not is_iterable(item):
                     data = self.serialize_tokens(item)
                     payload.append(_write_uint64(len(data)))
                     payload.append(data)
                     length += len(item) + 8
                 else:
-                    raise ValueError("TokenMonster: Input to decode must be an int, a list of ints, or a list of list of ints.")
-        else:
-            raise ValueError("TokenMonster: Input to decode must be an int, a list of ints, or a list of list of ints.]")
+                    raise ValueError("TokenMonster: Input to decode must be an int, list of ints, list of lists, or numpy array.")
         # Send
         job_type = self.encoding_length
         payload[0] = _write_uint32(batch_size)
         response = Vocab._communicate(job_type, self.id, length, payload)
         batches_reply = _read_uint32(response[0:4])
         if batches_reply != batch_size:
             raise RuntimeError("TokenMonster: batch size from response differs from request")
@@ -386,15 +389,15 @@
         it is converted to a binary string, so if you have binary string in the first place, feel
         free to pass that instead.
 
         Parameters:
             string or list of strings: A string or bytes string, or list of strings or bytes strings.
 
         Returns:
-            tokens (list of ints or list of list of ints): The tokens IDs
+            tokens (numpy array or list of numpy arrays): The tokens IDs
 
         Usage:
             tokens = vocab.tokenize(text)
         """
         if self._modified_id == -1:
             raise RuntimeError("TokenMonster: Access denied to expired Vocab instance.")
         length = 4
@@ -452,14 +455,18 @@
             offset += batch_length
         return tokens
         
     def tokenize_count(self, text):
         """
         Same as tokenize, but it returns only the number of tokens.
 
+        The number of tokens is the same as you would get from `tokenize`. If you want to count any characters
+        for which there are no tokens or single byte tokens, you should `enable_unk_token()`. It's okay to
+        enable `enable_unk_token()`, run `tokenize_count` and then `disable_unk_token()`.
+
         Parameters:
             string or list of strings: A string or bytes string, or list of strings or bytes strings.
 
         Returns:
             n_tokens (int or list of ints): The number of tokens for each input string
 
         Usage:
@@ -519,15 +526,15 @@
         return tokens
 
     def get_dictionary(self):
         """
         Returns a dictionary of all tokens in the vocabulary.
 
         This returns a list of dictionaries with keys "id", "token", "token_decoded", "type" and "score".
-        Note that you should not attempt to use this to interpret tokenized sequences because the capcode
+        Note that you should not attempt to use this to decode tokenized sequences because the capcode
         encoded tokens can change the way the next tokens are decoded. Therefore you should always use
         one of the two "decode" methods.
 
         Parameters:
             string or list of strings: A string or bytes string, or list of strings or bytes strings.
 
         Returns:
@@ -569,34 +576,14 @@
             self.dictionary[id] = {'id': id, 'token': token, 'token_decoded': token_decoded, 'type': types[typ], 'score': score}
             self.token_to_id[token] = id
             self.token_to_id[token_decoded] = id
             if typ == 3:
                 self.unk = id
         return self.dictionary
     
-    def convert_ids_to_tokens(self, ids):
-        """
-        Get the token string from any token ID, in it's capcode-encoded form.
-
-        Parameters:
-            ids: int or list of ints
-
-        Returns:
-            List of strings (None type for any that are not in the vocabulary)
-        """
-        if self.dictionary is None:
-            self.get_dictionary()
-        tokens = []
-        for id in ids:
-            if id >= 0 and id < len(self.dictionary):
-                tokens.append(self.dictionary[id]['token'])
-            else:
-                tokens.append(None)
-        return tokens
-    
     def id_to_token(self, id):
         """
         Get the token string from a single token ID, in it's capcode-encoded form.
 
         Parameters:
             id: int
 
@@ -606,34 +593,14 @@
         if self.dictionary is None:
             self.get_dictionary()
         if id >= 0 and id < len(self.dictionary):
             return self.dictionary[id]['token']
         else:
             return None
     
-    def convert_ids_to_tokens_decoded(self, ids):
-        """
-        Get the token string from any token IDs, in it's capcode-decoded form.
-
-        Parameters:
-            ids: int or list of ints
-
-        Returns:
-            List of strings (None type for any that are not in the vocabulary)
-        """
-        if self.dictionary is None:
-            self.get_dictionary()
-        tokens = []
-        for id in ids:
-            if id >= 0 and id < len(self.dictionary):
-                tokens.append(self.dictionary[id]['token_decoded'])
-            else:
-                tokens.append(None)
-        return tokens
-    
     def id_to_token_decoded(self, id):
         """
         Get the token string from a single token ID, in it's capcode-decoded form.
 
         Parameters:
             id: int
 
@@ -643,33 +610,14 @@
         if self.dictionary is None:
             self.get_dictionary()
         if id >= 0 and id < len(self.dictionary):
             return self.dictionary[id]['token_decoded']
         else:
             return None
     
-    def convert_tokens_to_ids(self, tokens):
-        """
-        Returns the IDs of the corresponding tokens. 'None' for any not in the vocabulary.
-
-        This works for both capcode-encoded "raw" tokens, and their decoded form.
-
-        Parameters:
-            tokens: string or list of strings
-
-        Returns:
-            List of strings (None type for any that are not in the vocabulary)
-        """
-        if self.dictionary is None:
-            self.get_dictionary()
-        ids = []
-        for tok in tokens:
-            ids.append(self.token_to_id.get(tok, None))
-        return ids
-    
     def token_to_id(self, token):
         """
         Returns the ID of a single token.
 
         This works for both capcode-encoded "raw" tokens, and their decoded form.
 
         Parameters:
@@ -811,20 +759,22 @@
         Returns:
             int: The new size of the vocabulary.
         """
         if self._modified_id == -1:
             raise RuntimeError("TokenMonster: Access denied to expired Vocab instance.")
         if isinstance(id, int):
             id = [id]
+        elif isinstance(id, (np.uint16, np.uint32)):
+            id = np.array([id])
         else:
             if not is_iterable(id):
                 raise ValueError("TokenMonster: Input to delete_token_by_id must be int or list of ints.")
             if len(id) == 0:
                 return self.vocab_size
-            if not isinstance(id[0], int):
+            if not is_int(id[0]):
                 raise ValueError("TokenMonster: Input to delete_token_by_id must be int or list of ints.")
         payload = _write_uint32(len(id)) + _pack_32bit_ints(id)
         job_type = 16
         self.vocab_size = Vocab._communicate(job_type, self.id, len(payload), payload)
         self._modified()
         return self.vocab_size
 
@@ -927,29 +877,29 @@
             raise RuntimeError("TokenMonster: Access denied to expired Vocab instance.")
         payload = _write_uint8(int(order_by_score))
         job_type = 19
         return Vocab._communicate(job_type, self.id, 1, payload)
 
     def deserialize_tokens(self, binary_string):
         """
-        Deserializes a binary string back into a list of ints (tokens).
+        Deserializes a binary string into a numpy array of tokens IDs.
         The encoding_length needs to be recorded separetely.
         """
         if self.encoding_length == 2:
             return _unpack_16bit_ints(binary_string)
         elif self.encoding_length == 4:
             return _unpack_32bit_ints(binary_string)
-        elif self.encoding_length == 3:
-            return _unpack_24bit_ints(binary_string)
+        #elif self.encoding_length == 3:
+        #    return _unpack_24bit_ints(binary_string)
         else:
             raise RuntimeError("TokenMonster: Invalid encoding length")
         
     def serialize_tokens(self, integer_list):
         """
-        Serializes tokens from a list of ints into a binary string.
+        Serializes tokens from a numpy array into a binary string.
         The encoding_length needs to be recorded separetely.
         """
         if self.encoding_length == 2:
             return _pack_16bit_ints(integer_list)
         elif self.encoding_length == 4:
             return _pack_32bit_ints(integer_list)
         elif self.encoding_length == 3:
@@ -1226,32 +1176,44 @@
         else:
             raise RuntimeError("Unsupported architecture for macOS: {}".format(arch_name))
     else:
         raise RuntimeError("Unsupported operating system: {}".format(os_name))
 
 def _unpack_16bit_ints(binary_string):
     n = len(binary_string) // 2
-    return struct.unpack('<' + 'H'*n, binary_string)
+    return np.frombuffer(binary_string, dtype='<u2', count=n)
 
-def _unpack_24bit_ints(binary_string):
-    n = len(binary_string) // 3
-    return [int.from_bytes(binary_string[i:i+3], byteorder='little') for i in range(0, 3*n, 3)]
+#def _unpack_24bit_ints(binary_string):
+#    n = len(binary_string) // 3
+#    return [int.from_bytes(binary_string[i:i+3], byteorder='little') for i in range(0, 3*n, 3)]
 
 def _unpack_32bit_ints(binary_string):
     n = len(binary_string) // 4
-    return struct.unpack('<' + 'I'*n, binary_string)
+    return np.frombuffer(binary_string, dtype='<u4', count=n)
 
 def _pack_16bit_ints(integer_list):
-    return struct.pack('<' + 'H'*len(integer_list), *integer_list)
+    if isinstance(integer_list, np.ndarray):
+        if integer_list.dtype.byteorder == '>':
+            return integer_list.byteswap().tobytes()
+        else:
+            return integer_list.tobytes()
+    else:
+        return struct.pack('<' + 'H' * len(integer_list), *integer_list)
 
-def _pack_24bit_ints(integer_list):
-    return b''.join([int(i).to_bytes(3, byteorder='little') for i in integer_list])
+#def _pack_24bit_ints(integer_list):
+#    return b''.join([int(i).to_bytes(3, byteorder='little') for i in integer_list])
 
 def _pack_32bit_ints(integer_list):
-    return struct.pack('<' + 'I'*len(integer_list), *integer_list)
+    if isinstance(integer_list, np.ndarray):
+        if integer_list.dtype.byteorder == '>':
+            return integer_list.byteswap().tobytes()
+        else:
+            return integer_list.tobytes()
+    else:
+        return struct.pack('<' + 'I' * len(integer_list), *integer_list)
 
 def _write_uint32(input):
     return struct.pack('<I', input)
 
 def _write_uint64(input):
     return struct.pack('<Q', input)
 
@@ -1268,9 +1230,14 @@
     return struct.unpack('<f', input)[0]
 
 def is_iterable(obj):
     if isinstance(obj, (str, bytes)):
         return False
     return isinstance(obj, Iterable)
 
+def is_int(obj):
+    if isinstance(obj, (int, np.uint16, np.uint32)):
+        return True
+    return False
+
 _TOKENMONSTER_URL = "https://huggingface.co/alasdairforsythe/tokenmonster/resolve/main/"
 _TMS_VERSION_ID = 2
```

