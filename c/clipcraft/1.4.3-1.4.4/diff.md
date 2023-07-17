# Comparing `tmp/clipcraft-1.4.3.tar.gz` & `tmp/clipcraft-1.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clipcraft-1.4.3.tar", last modified: Fri Jul 14 17:40:12 2023, max compression
+gzip compressed data, was "clipcraft-1.4.4.tar", last modified: Mon Jul 17 15:41:12 2023, max compression
```

## Comparing `clipcraft-1.4.3.tar` & `clipcraft-1.4.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-14 17:40:12.278205 clipcraft-1.4.3/
--rw-rw-rw-   0        0        0     3769 2023-07-14 17:40:12.274057 clipcraft-1.4.3/PKG-INFO
--rw-rw-rw-   0        0        0     3428 2023-07-14 17:15:39.000000 clipcraft-1.4.3/README.md
-drwxrwxrwx   0        0        0        0 2023-07-14 17:40:12.260294 clipcraft-1.4.3/clipcraft/
--rw-rw-rw-   0        0        0      128 2023-07-14 14:35:14.000000 clipcraft-1.4.3/clipcraft/__init__.py
--rw-rw-rw-   0        0        0     8334 2023-07-14 17:39:39.000000 clipcraft-1.4.3/clipcraft/create_embeddings.py
--rw-rw-rw-   0        0        0     5177 2023-07-14 17:39:42.000000 clipcraft-1.4.3/clipcraft/knn_search.py
-drwxrwxrwx   0        0        0        0 2023-07-14 17:40:12.274057 clipcraft-1.4.3/clipcraft.egg-info/
--rw-rw-rw-   0        0        0     3769 2023-07-14 17:40:12.000000 clipcraft-1.4.3/clipcraft.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      259 2023-07-14 17:40:12.000000 clipcraft-1.4.3/clipcraft.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-14 17:40:12.000000 clipcraft-1.4.3/clipcraft.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       35 2023-07-14 17:40:12.000000 clipcraft-1.4.3/clipcraft.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-07-14 17:40:12.000000 clipcraft-1.4.3/clipcraft.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-14 17:40:12.278205 clipcraft-1.4.3/setup.cfg
--rw-rw-rw-   0        0        0      642 2023-07-14 17:40:00.000000 clipcraft-1.4.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-17 15:41:12.490607 clipcraft-1.4.4/
+-rw-rw-rw-   0        0        0     4197 2023-07-17 15:41:12.490607 clipcraft-1.4.4/PKG-INFO
+-rw-rw-rw-   0        0        0     3855 2023-07-17 15:34:01.000000 clipcraft-1.4.4/README.md
+drwxrwxrwx   0        0        0        0 2023-07-17 15:41:12.470566 clipcraft-1.4.4/clipcraft/
+-rw-rw-rw-   0        0        0      289 2023-07-17 15:33:29.000000 clipcraft-1.4.4/clipcraft/__init__.py
+-rw-rw-rw-   0        0        0     8043 2023-07-17 15:32:38.000000 clipcraft-1.4.4/clipcraft/create_embeddings.py
+-rw-rw-rw-   0        0        0     5177 2023-07-14 17:39:42.000000 clipcraft-1.4.4/clipcraft/knn_search.py
+drwxrwxrwx   0        0        0        0 2023-07-17 15:41:12.489561 clipcraft-1.4.4/clipcraft.egg-info/
+-rw-rw-rw-   0        0        0     4197 2023-07-17 15:41:12.000000 clipcraft-1.4.4/clipcraft.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      259 2023-07-17 15:41:12.000000 clipcraft-1.4.4/clipcraft.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-17 15:41:12.000000 clipcraft-1.4.4/clipcraft.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       35 2023-07-17 15:41:12.000000 clipcraft-1.4.4/clipcraft.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-17 15:41:12.000000 clipcraft-1.4.4/clipcraft.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-17 15:41:12.490607 clipcraft-1.4.4/setup.cfg
+-rw-rw-rw-   0        0        0      642 2023-07-17 15:41:07.000000 clipcraft-1.4.4/setup.py
```

### Comparing `clipcraft-1.4.3/PKG-INFO` & `clipcraft-1.4.4/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clipcraft
-Version: 1.4.3
+Version: 1.4.4
 Summary: A package for CLIP-based image and text processing.
 Home-page: https://github.com/mmckenzieORCEN/CLIPCraft
 Author: Morgan McKenzie
 Author-email: morgancmckenziecs@gmail.com
 Description-Content-Type: text/markdown
 
 # CLIPCraft
@@ -22,44 +22,45 @@
 ```bash
 pip install clipcraft
 ```
 ## Usage
 
 CLIPCraft offers 4 functions for users to interact with; <br>
 <br>
-**createImageEmbeddings(input_urls)** This function creates image embeddings from a file containing URLs, where input_urls is a string of a filename or a list of strings of filenames. It returns a list of tuples, where the 0<sup>th</sup> value is the image URL, and the 1<sup>st</sup> value is the resulting embedding.<br>
+**createImageEmbeddings(input_urls, output_type)** This function creates image embeddings from a file containing URLs, where input_urls is a string of a filename or a list of strings of filenames, and output_type is the type of output desired for the embeddings; "list" or "file". It returns a list of tuples, where the 0<sup>th</sup> value is the image URL, and the 1<sup>st</sup> value is the resulting embedding.<br>
 <br>
 
-**createTextEmbeddings(input_text)** This function creates text embeddings from a user-input string of text or list of strings of text. It returns a list of tuples, where the 0<sup>th</sup> value is the raw text, and the 1<sup>st</sup> value is the resulting embedding. <br>
+**createTextEmbeddings(input_text, output_type)** This function creates text embeddings from a user-input string of text or list of strings of text. output_type is the type of output desired for the embeddings; "list" or "file". It returns a list of tuples, where the 0<sup>th</sup> value is the raw text, and the 1<sup>st</sup> value is the resulting embedding. <br>
 <br>
 
 **KNNSearchImage(text_embeddings, image_embeddings)** This function will find the nearest 10 similar images from given text embedding(s) list using K-Nearest-Neighbors. It is designed for use by providing the list returned from createTextEmbeddings. text_embeddings should be the return value of createTextEmbeddings, while image_embeddings should be the return value for createImageEmbeddings.<br>
 <br>
 
 **KNNSearchText(text_embeddings, image_urls)** This function will find the most similar caption to a given image. It is designed for use by providing the list returned from createTextEmbeddings. text_embeddings should be the return value of createTextEmbeddings, while image_urls should be a single URL or a list of URLs. 
 
 ## Example
 ```python
 import clipcraft as cc
 
 file_urls = "https://upload.wikimedia.org/wikipedia/commons/thumb/6/68/Orange_tabby_cat_sitting_on_fallen_leaves-Hisashi-01A.jpg/800px-Orange_tabby_cat_sitting_on_fallen_leaves-Hisashi-01A.jpg"
 
-image_embeds = cc.createImageEmbeddings(file_urls)
+image_embeds = cc.createImageEmbeddings(file_urls, "list")
 
 text_embed_list = ["a picture of a cat"]
 
-text_embeds = cc.createTextEmbeddings(text_embed_list)
+text_embeds = cc.createTextEmbeddings(text_embed_list, "list")
 
 cc.KNNSearchImage(text_embeds, image_embeds)
 
 cc.KNNSearchText(text_embeds, ["https://upload.wikimedia.org/wikipedia/commons/thumb/6/68/Orange_tabby_cat_sitting_on_fallen_leaves-Hisashi-01A.jpg/800px-Orange_tabby_cat_sitting_on_fallen_leaves-Hisashi-01A.jpg"])
 ```
 Note the arguments taken by the KNN functions are the return values of the previous external functions. <br>
 
 The output of KNNSearchImage will be 5 images with the closest euclidean distance in ascending order; that is, the closest related image being output first. <br>
 The output of KNNSearchText will be a caption of the image based on the lowest euclidean distance between your list of input captions and the input image.
 
 ## Requirements
-
+To run the functions from this package, you must install PyTorch, as the Hugging Face Transformers library is built on top of it. Instructions to do so can be found here: https://pytorch.org/get-started/locally/ <br>
+<br>
 The requirements for the package can be found in requirements.txt. However, note that these dependencies will be automatically installed when invoking the pip command.
```

### Comparing `clipcraft-1.4.3/README.md` & `clipcraft-1.4.4/clipcraft.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,56 +1,66 @@
-# CLIPCraft
-CLIPCraft is a package written in Python for use by Data Scientists/Analysts working with image-to-text and text-to-image implementations.
-
-More specifically, CLIPCraft contains user-friendly functions that are incredibly simple and easy to use, providing a simple and convenient interface for text and image projects.
-
-## Features:
-
-**Embedding Extraction**: Extract embeddings for images and texts using CLIP. <br>
-**Image-to-Text**: Generate textual descriptions (captions) for given images using CLIP. Currently, you must provide your own list of captions. <br>
-**Text-to-Image from Embeddings**: Generate visual representations from embeddings for given texts using CLIP. 
-
-## Installation
-```bash
-pip install clipcraft
-```
-## Usage
-
-CLIPCraft offers 4 functions for users to interact with; <br>
-<br>
-**createImageEmbeddings(input_urls)** This function creates image embeddings from a file containing URLs, where input_urls is a string of a filename or a list of strings of filenames. It returns a list of tuples, where the 0<sup>th</sup> value is the image URL, and the 1<sup>st</sup> value is the resulting embedding.<br>
-<br>
-
-**createTextEmbeddings(input_text)** This function creates text embeddings from a user-input string of text or list of strings of text. It returns a list of tuples, where the 0<sup>th</sup> value is the raw text, and the 1<sup>st</sup> value is the resulting embedding. <br>
-<br>
-
-**KNNSearchImage(text_embeddings, image_embeddings)** This function will find the nearest 10 similar images from given text embedding(s) list using K-Nearest-Neighbors. It is designed for use by providing the list returned from createTextEmbeddings. text_embeddings should be the return value of createTextEmbeddings, while image_embeddings should be the return value for createImageEmbeddings.<br>
-<br>
-
-**KNNSearchText(text_embeddings, image_urls)** This function will find the most similar caption to a given image. It is designed for use by providing the list returned from createTextEmbeddings. text_embeddings should be the return value of createTextEmbeddings, while image_urls should be a single URL or a list of URLs. 
-
-## Example
-```python
-import clipcraft as cc
-
-file_urls = "https://upload.wikimedia.org/wikipedia/commons/thumb/6/68/Orange_tabby_cat_sitting_on_fallen_leaves-Hisashi-01A.jpg/800px-Orange_tabby_cat_sitting_on_fallen_leaves-Hisashi-01A.jpg"
-
-image_embeds = cc.createImageEmbeddings(file_urls)
-
-text_embed_list = ["a picture of a cat"]
-
-text_embeds = cc.createTextEmbeddings(text_embed_list)
-
-cc.KNNSearchImage(text_embeds, image_embeds)
-
-cc.KNNSearchText(text_embeds, ["https://upload.wikimedia.org/wikipedia/commons/thumb/6/68/Orange_tabby_cat_sitting_on_fallen_leaves-Hisashi-01A.jpg/800px-Orange_tabby_cat_sitting_on_fallen_leaves-Hisashi-01A.jpg"])
-```
-Note the arguments taken by the KNN functions are the return values of the previous external functions. <br>
-
-The output of KNNSearchImage will be 5 images with the closest euclidean distance in ascending order; that is, the closest related image being output first. <br>
-The output of KNNSearchText will be a caption of the image based on the lowest euclidean distance between your list of input captions and the input image.
-
-## Requirements
-
-The requirements for the package can be found in requirements.txt. However, note that these dependencies will be automatically installed when invoking the pip command. 
-
-
+Metadata-Version: 2.1
+Name: clipcraft
+Version: 1.4.4
+Summary: A package for CLIP-based image and text processing.
+Home-page: https://github.com/mmckenzieORCEN/CLIPCraft
+Author: Morgan McKenzie
+Author-email: morgancmckenziecs@gmail.com
+Description-Content-Type: text/markdown
+
+# CLIPCraft
+CLIPCraft is a package written in Python for use by Data Scientists/Analysts working with image-to-text and text-to-image implementations.
+
+More specifically, CLIPCraft contains user-friendly functions that are incredibly simple and easy to use, providing a simple and convenient interface for text and image projects.
+
+## Features:
+
+**Embedding Extraction**: Extract embeddings for images and texts using CLIP. <br>
+**Image-to-Text**: Generate textual descriptions (captions) for given images using CLIP. Currently, you must provide your own list of captions. <br>
+**Text-to-Image from Embeddings**: Generate visual representations from embeddings for given texts using CLIP. 
+
+## Installation
+```bash
+pip install clipcraft
+```
+## Usage
+
+CLIPCraft offers 4 functions for users to interact with; <br>
+<br>
+**createImageEmbeddings(input_urls, output_type)** This function creates image embeddings from a file containing URLs, where input_urls is a string of a filename or a list of strings of filenames, and output_type is the type of output desired for the embeddings; "list" or "file". It returns a list of tuples, where the 0<sup>th</sup> value is the image URL, and the 1<sup>st</sup> value is the resulting embedding.<br>
+<br>
+
+**createTextEmbeddings(input_text, output_type)** This function creates text embeddings from a user-input string of text or list of strings of text. output_type is the type of output desired for the embeddings; "list" or "file". It returns a list of tuples, where the 0<sup>th</sup> value is the raw text, and the 1<sup>st</sup> value is the resulting embedding. <br>
+<br>
+
+**KNNSearchImage(text_embeddings, image_embeddings)** This function will find the nearest 10 similar images from given text embedding(s) list using K-Nearest-Neighbors. It is designed for use by providing the list returned from createTextEmbeddings. text_embeddings should be the return value of createTextEmbeddings, while image_embeddings should be the return value for createImageEmbeddings.<br>
+<br>
+
+**KNNSearchText(text_embeddings, image_urls)** This function will find the most similar caption to a given image. It is designed for use by providing the list returned from createTextEmbeddings. text_embeddings should be the return value of createTextEmbeddings, while image_urls should be a single URL or a list of URLs. 
+
+## Example
+```python
+import clipcraft as cc
+
+file_urls = "https://upload.wikimedia.org/wikipedia/commons/thumb/6/68/Orange_tabby_cat_sitting_on_fallen_leaves-Hisashi-01A.jpg/800px-Orange_tabby_cat_sitting_on_fallen_leaves-Hisashi-01A.jpg"
+
+image_embeds = cc.createImageEmbeddings(file_urls, "list")
+
+text_embed_list = ["a picture of a cat"]
+
+text_embeds = cc.createTextEmbeddings(text_embed_list, "list")
+
+cc.KNNSearchImage(text_embeds, image_embeds)
+
+cc.KNNSearchText(text_embeds, ["https://upload.wikimedia.org/wikipedia/commons/thumb/6/68/Orange_tabby_cat_sitting_on_fallen_leaves-Hisashi-01A.jpg/800px-Orange_tabby_cat_sitting_on_fallen_leaves-Hisashi-01A.jpg"])
+```
+Note the arguments taken by the KNN functions are the return values of the previous external functions. <br>
+
+The output of KNNSearchImage will be 5 images with the closest euclidean distance in ascending order; that is, the closest related image being output first. <br>
+The output of KNNSearchText will be a caption of the image based on the lowest euclidean distance between your list of input captions and the input image.
+
+## Requirements
+To run the functions from this package, you must install PyTorch, as the Hugging Face Transformers library is built on top of it. Instructions to do so can be found here: https://pytorch.org/get-started/locally/ <br>
+<br>
+The requirements for the package can be found in requirements.txt. However, note that these dependencies will be automatically installed when invoking the pip command. 
+
+
```

### Comparing `clipcraft-1.4.3/clipcraft/create_embeddings.py` & `clipcraft-1.4.4/clipcraft/create_embeddings.py`

 * *Files 6% similar despite different names*

```diff
@@ -108,23 +108,18 @@
                     if url:  # Skips empty lines
                         urls.append(url)
     _extractURLFromJSON(data, urls)
     return urls
 
 
 # User-callable for users to call to create Image embeddings
-def createImageEmbeddings(input_urls): 
-    while True:
-        output_type = input("Enter the desired output type for the image embeddings (list or file): ")
-
-        if output_type in ["list", "file"]:
-            break
-        else:
-            print("Invalid output type. Expected 'list' or 'file'. Please try again")
-    
+def createImageEmbeddings(input_urls, output_type): 
+    if output_type not in ["list", "file"]:
+        raise ValueError("Invalid output type. Expected 'list' or 'file'")
+            
     embeddings = []
     if isinstance(input_urls, str):
     # Read the file and process its contents
         if input_urls.startswith("http"):
             embeddings.extend(_imageEmbeddings([input_urls]))
         else:
             url_list = _extractURLFromFile(input_urls)
@@ -150,22 +145,17 @@
         _writeEmbeddingsToFile("image",embeddings)
         return "Embeddings successfully written to file."
     return embeddings
 
 
                 
 # User-callable function to generate text embeddings from CLIP
-def createTextEmbeddings(input_text):
-    while True:
-        output_type = input("Enter the desired output type for the text embeddings (list or file): ")
-
-        if output_type in ["list", "file"]:
-            break
-        else:
-            print("Invalid output type. Expected 'list' or 'file'. Please try again")
+def createTextEmbeddings(input_text, output_type):
+    if output_type not in ["list", "file"]:
+        raise ValueError("Invalid output type. Expected 'list' or 'file'")
             
     text_embedding_list = []
     if isinstance(input_text, str):  # Check if user input is a string instead of list
         input_text = [input_text]  # Convert it to a list with a single element for processing
         
     # Initiating the model/tokenizer from HuggingFace/CLIP
     model = CLIPModel.from_pretrained("openai/clip-vit-base-patch32")
```

### Comparing `clipcraft-1.4.3/clipcraft/knn_search.py` & `clipcraft-1.4.4/clipcraft/knn_search.py`

 * *Files identical despite different names*

### Comparing `clipcraft-1.4.3/setup.py` & `clipcraft-1.4.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 with open('README.md', 'r', encoding='utf-8') as readme_file:
     long_description = readme_file.read()
 
 setup(
     name="clipcraft",
-    version="1.4.3",
+    version="1.4.4",
     description="A package for CLIP-based image and text processing.",
     author='Morgan McKenzie',
     author_email='morgancmckenziecs@gmail.com',
     packages=["clipcraft"],
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/mmckenzieORCEN/CLIPCraft',
```

